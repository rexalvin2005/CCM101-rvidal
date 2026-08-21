# Cloud Infrastructure Report

## Operating System
PRETTY_NAME="Ubuntu 24.04.4 LTS"

## Kernel Version
PRETTY_NAME="Ubuntu 24.04.4 LTS"

## CPU Model
Model name:                              Intel Xeon E312xx (Sandy Bridge, IBRS update)
BIOS Model name:                         RHEL-9.6.0 PC (Q35 + ICH9, 2009)  CPU @ 2.0GHz

## Number of CPU Cores

1


## Total RAM

  total        used        free      shared  buff/cache   available
Mem:           1.9Gi       407Mi       865Mi       1.1Mi       798Mi       1.5Gi
Swap:          1.0Gi          0B       1.0Gi

## Disk Capacity

NAME    MAJ:MIN RM  SIZE RO TYPE MOUNTPOINTS
vda     253:0    0   20G  0 disk 
|-vda1  253:1    0   19G  0 part /
|-vda14 253:14   0    4M  0 part 
|-vda15 253:15   0  106M  0 part /boot/efi
`-vda16 259:0    0  913M  0 part /boot


## Mounted File Systems


Filesystem     Type   Size  Used Avail Use% Mounted on
tmpfs          tmpfs  191M  996K  190M   1% /run
/dev/vda1      ext4    19G  5.4G   13G  30% /
tmpfs          tmpfs  952M   84K  952M   1% /dev/shm
tmpfs          tmpfs  5.0M     0  5.0M   0% /run/lock
/dev/vda16     ext4   881M  117M  703M  15% /boot
/dev/vda15     vfat   105M  6.2M   99M   6% /boot/efi
## Hostname

ubuntu

The IP address of the server was identified using the `hostname -I` command.
172.30.1.2 172.17.0.1

## Linux Commands Used

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
lsblk
df -hT
hostname
hostname -I
