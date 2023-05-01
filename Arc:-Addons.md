### Generic Addons

* **acpid**: ACPI Daemon (allways selected)
* **misc**: Utilities we need (allways selected)
* **cpuinfo**: Adds real CPU Informations to Control Panel
* **powersched**: Allows Disks to go to sleep
* **nvmestorage**: Adds NVMe Disks as Storage (Will take some time (up to 60 minutes at first boot, because of resync drives and you need a working Datastore in DSM to use this)

`We need another Bootvolume because of DSM can't boot from NVMe. It is possible that you have to fix Storage Pool in Storage Manager.`