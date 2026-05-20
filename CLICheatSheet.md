
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
|Command|Funktion|
|---|---|
|`qm list`|List VMs|
|`qm start <vmid>`|Start VM|
|`qm stop <vmid>`|Stop VM|
