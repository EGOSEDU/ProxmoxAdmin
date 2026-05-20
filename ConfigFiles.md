# Configuration Files

# Linux
|File|Funktion|
|/etc/hosts|Static host mapping|
|/etc/resolv.conf|DNS Server|
|/etc/network/interfaces|Netzwerk Interface Configuration|

## PVE
### Cluster Wide
|File|Funktion|
|/etc/pve|proxmox Configuration Directory - Cluster Replicated|
|/etc/pve/datacenter.cfg|Cluster-wide settings|
|/etc/pve/storage.cfg|Storage Configuration|
|/mnt/pve/<storage>|Mount Point für Storage|
|/etc/pve/user.cfg|User accounts and permissions|
|/etc/pve/group.cfg|User groups|

### VM & Container
|File|Funktion|
|/etc/pve/qemu-server/<vmid>.conf|Virtual Machine Configuration|
|/etc/pve/lcx/<vmid>.conf|Container Configuration|

