### List

* **acpid**: ACPI Daemon (allways selected)
* **misc**: Utilities we need (allways selected)
* **cpuinfo**: Adds real CPU Informations to Control Panel <- working after first reboot

### NVMe Addon Options

_you can only use 1 of them - it is only possible to change this option in a clean DSM Installation_

* **nvmecache**: Adds NVMe Disks as Cache <- working after first reboot
* **nvmestorage**: Adds NVMe Disks as Storage <- working after first reboot | EXPERIMENTAL
  (It is possible that you have to fix Storage Pool in Disk Manager)

(working on native/baremetal Installations and on ESXi up to 7.0U3 - not working on ESXi 8!)