# Welcome to Wiki for Arc Loader

## Important

- It is highly recommended to use a fast USB flash drive (USB 3.0 or better) otherwise you will get a kernel panic
- You must have at least 4GB of RAM, both in baremetal and VMs
- The DSM kernel is compatible with SATA ports, not SAS/SCSI/etc. For device-tree models (DT) only SATA Controller will work. For the other models, another type of controller (HBA, Raid or SCSI Controller) may work.

## Use Arc Redpill Loader

To use this project, download the latest image available and burn it to a USB stick or SATA disk-on-module. Set the PC to boot from the burned media and follow the informations on the screen. When booting, the user can call the "arc.sh" command from the computer itself, access via SSH. You can also use the virtual terminal (ttyd) by typing the address provided on the screen (http://(ip):7681). The Loader will start "arc.sh" and you can select wich menu you want. The loader will automatically increase the size of the last partition and use this space as cache if it is larger than 2GiB.