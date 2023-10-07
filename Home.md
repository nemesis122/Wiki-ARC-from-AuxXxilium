# Welcome to Wiki for Arc Loader

## Important

- It is highly recommended to use a fast USB flash drive (USB 3.0 or better) otherwise you will get a kernel panic
- You must have at least 4GB of RAM, both in Native/Baremetal and VMs
- The DSM kernel is compatible with SATA ports, not SAS/SCSI/etc. For Device-Tree Models (DT) only SATA Controller will work. For the other Models, another Type of Controller (HBA, Raid or SCSI Controller) may work.
- Arc will not run (now and in Future) on every Hardware. Every Module/Driver must be ported to get Support of this Device. Some Vendor(like Realtek) are not well supported by Linux or the Source is very old.

## Use Arc Loader

To use this project, download the latest image available and burn it to a USB stick or SATA disk-on-module. Set the PC to boot from the burned media and follow the informations on the screen. When booting, the user can call the "arc.sh" command from the computer itself, access via SSH. You can also use the virtual terminal (ttyd) by typing the address provided on the screen (http://(ip):7681). The Loader will start "arc.sh" and you can select wich menu you want. The loader will automatically increase the size of the last partition and use this space as cache if it is larger than 2GB.

## Limitations

* Max 8 Drives per Storagecontroller
* Max 26 Drives per System
* Max 8 NIC per System
* If you use "Arc Patch" you can only use each Model once in if you plan to use CMS. If not, you can use once per MAC.