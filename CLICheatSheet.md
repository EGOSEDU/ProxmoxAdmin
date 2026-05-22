[Home](README.md)
# proxmox CLI Cheat Sheet

## Node Management
|Command|Funktion|
|---|---|
|`pvecm status`|Cluster Status|
|`pvcm nodes`|Show cluster nodes|
|`pvesh set /nodes/nodename/status --offline 1`|Set Cluster Node Offline|
|`pvesh set /nodes/nodename/status --offline 0`|Set Cluster Node Online|
## Storage Management
|Command|Funktion|
|---|---|
|`pvesm status`|Show storage status|
## Network Management
|Command|Funktion|
|---|---|
|`ip a`|Show IP Addresses|
|`pve-firewall status`|Show firewall status|
## Virtual Machines (qm command)
VM Operations
|Command|Funktion|
|---|---|
|`qm list`|List VMs|
|`qm start <vmid>`|Start VM|
|`qm stop <vmid>`|Stop VM|
|`qm shutdown <vmid>`|Shutdown VM|
|`qm destroy <vmid>`|Delete VM|
|`qm resize <vmid> <disk> <size>`|Stop VM|

Backup and Restore
|Command|Funktion|
|---|---|
|`vzdump <vmid>`|Backup VM or Container|
|`qmrestore <backup> <vmid>`|Restore VM|
|`pct restore <vmid>`|Restore Container|
## Linux OS
|Command|Funktion|
|---|---|
|`apt update`|Update package lists|
|`apt upgrade`|Update ohne neue Depencencies|
|`apt dist-upgrade`|Full upgrade inkl. neue Dependencies|
|`pveversion`|Aktuelle proxmox Version|
