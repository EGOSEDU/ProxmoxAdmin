[Home](README.md)

# Node Installation

## Disable Enterprise Repositories

sudo sed -i "s/^deb/#deb/" /etc/apt/sources.list.d/pve-enterprise.list
sudo sed -i "s/^deb/#deb/" /etc/apt/sources.list.d/ceph.list

## Add "no-subscription" Repository

echo "deb http://download.proxmox.com/debian/pve bookworm pve-no-subscription" | sudo tee /etc/apt/sources.list.d/pve-no-subscription.list

- first
- second
- third

> quote

---

1. a
2. b
3. c

