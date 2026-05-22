[Home](README.md)
# Configuration Files

# Linux
|File|Funktion|
|---|---|
|/etc/hosts|Static host mapping|
|/etc/resolv.conf|DNS Server|
|/etc/network/interfaces|Netzwerk Interface Configuration|

## PVE
### Cluster Wide
|File|Funktion|
|---|---|
|/etc/pve|proxmox Configuration Directory - Cluster Replicated|
|/etc/pve/datacenter.cfg|Cluster-wide settings|
|/etc/pve/storage.cfg|Storage Configuration|
|/mnt/pve/<storage>|Mount Point für Storage|
|/etc/pve/user.cfg|User accounts and permissions|
|/etc/pve/group.cfg|User groups|
|/etc/pve/ceph.conf|CEPH Configuration|
|/etc/pve/corosync.conf|CoroSync Configuration|

### VM & Container
|File|Funktion|
|---|---|
|/etc/pve/qemu-server/&lt;vmid&gt;.conf|Virtual Machine Configuration|
|/etc/pve/lcx/&lt;vmid&gt;.conf|Container Configuration|

### Log Files
|File|Funktion|
|---|---|
