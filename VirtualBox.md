# Virtual Box

## Raw Hard Disk

https://www.serverwatch.com/server-tutorials/using-a-physical-hard-drive-with-a-virtualbox-vm.html

1. Command prompt as Admin

2. Create vmdk link to Physical Drive (same number as in Disk Management)
```
cd "C:\Program Files\Oracle\VirtualBox"
VBoxManage internalcommands createrawvmdk -filename "I:\VirtualBox VMs\Ubuntu Iridium\UbuntuIridium.vmdk" -rawdisk \\.\PhysicalDrive3
```

3. Offline the disk

```
DISKPART
LIST DISK
SELECT DISK 3
LIST PARTITION
OFFLINE DISK
ATTRIBUTES DISK
ATTRIBUTES DISK CLEAR READONLY
ATTRIBUTES DISK
```

4. Start VirtualBox as Admininstrator

5. Choose the newly created vmdk file in settings
