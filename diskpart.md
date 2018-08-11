# Diskpart

## Mount VHD

Can be done from Computer Management - be sure not to select Read Only option - it will screw up!

## Unmount VHD from command line

Open CMD as Admin
```
diskpart
select vdisk file="D:\WindowsImageBackup\XONAR\Backup 2018-04-01 133329\myvhd.vhd"
detach vdisk
```

