### Generic Addons

* **acpid**: ACPI Daemon (allways selected)
* **misc**: Utilities we need (allways selected)
* **cpuinfo**: Adds real CPU Informations to Control Panel <- working after first reboot

### NVMe Addons

_you can only use 1 of them - it is only possible to change this option in a clean DSM Installation_

* **nvmecache**: Adds NVMe Disks as Cache <- working after first reboot
* **nvmestorage**: Adds NVMe Disks as Storage <- EXPERIMENTAL

`Add nvmestorage after DSM installation and Volume creation, else it will not work and creation will fail. We need another Bootvolume because of DSM can't boot from NVMe. It is possible that you have to fix Storage Pool in Storage Manager.`