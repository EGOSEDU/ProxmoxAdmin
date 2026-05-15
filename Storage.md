[Home](README.md)

# Storage

## Multipathing

### Tools installieren
```
apt install multipath-tools
```

### Multipath Mapping

```
/lib/udev/scsi_id -g -u -d /dev/sdX
multipath -a WWID
```

### Refresh Multipath
```
multipath -rr
```

## Create Storage Objects on Multipath

### LVM
pvcreate /dev/mapper/3600c0ff000144a912145150001000000
vgcreate vg01 /dev/mapper/3600c0ff000144a912145150001000000

### LVM Thin Pool
pvcreate /dev/mapper/3600c0ff000144a919b45150001000000
vgcreate vg02 /dev/mapper/3600c0ff000144a919b45150001000000
vcreate -T vg02/thinpool01 -L 1024G

### ZFS
zpool create zfs01 -f 3600c0ff000144a914645150001000000

### Ceph
ceph-volume lvm create --data /dev/mapper/3600c0ff000144a919b45150001000000
