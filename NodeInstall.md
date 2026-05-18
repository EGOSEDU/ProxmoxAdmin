[Home](README.md)

# Node Installation

## Time Configuration
Config File
> /etc/chrony/chrony.conf

*Service Restart and Logging*
```
systemctl restart chronyd
journalctl –since -1h –u u chrony
```

## IP Stack
Verwendet DHCP Server für initiale IP

## Disable Enterprise Repositories


Old:
```
sudo sed -i "s/^deb/#deb/" /etc/apt/sources.list.d/pve-enterprise.list
sudo sed -i "s/^deb/#deb/" /etc/apt/sources.list.d/ceph.list
```
## Add "no-subscription" Repository
Create file /etc/apt/sources.list.d/pve-no-subscription.sources
```
Types: deb
URIs: http://download.proxmox.com/debian/pve
Suites: bookworm
Components: pve-no-subscription
Signed-By: /usr/share/keyrings/proxmox-archive-keyring.gpg
```
Old:
```
echo "deb http://download.proxmox.com/debian/pve bookworm pve-no-subscription" | sudo tee /etc/apt/sources.list.d/pve-no-subscription.list
```

- first
- second
- third

> quote

---

1. a
2. b
3. c

