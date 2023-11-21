### Addons

`>>>Make sure you only select these additional Addons you need.<<<`

* **acpid**: ACPI Daemon - to use ACPI Features (always selected)
* **bootwait**: Checks if all Device are ready before proceed to Boot
* **console**: Add Console Output for DSM
* **disks**: Patches Syno Storage Map to match your Config (always selected)
* **eudev**: Eudev Daemon - to get your Devices working (always selected)
* **i915**: Patch i915 Modul for some Intel iGPU (For Apollolake & Geminilake Models)
* **localrss**: Local RSS Server for DSM Installation (always selected)
* **misc**: Utilities we need (always selected)
* **wol**: WOL enable Wake on LAN (always selected)

* **amepatch**: Patch for Syno AME
* **codecpatch**: Patch for Synocodectool
* **cpufreqscaling**: Enable CPU Frequency Scaling Function (removed for now, only optical effect)
* **cpuinfo**: Adds real CPU Informations to Control Panel
* **drivedbpatch**: Adds your Drives to DriveDB
* **nvmecache**: Allow the User to create NVMe Cache on DS918+, DS419+, DS719+, DS1019+, DS1621xs+ and RS1619xs+
* **nvmestorage**: Allow the User to create NVMe Storage
* **powersched**: Allows to use Timed Power Feature
* **surveillancepatch**: Patch Surveillance Station on all non DVA Models (Feed will reload every hour, needed to bypass security in dsm)

`We need another Bootvolume because of DSM can't boot from NVMe.`

`To remove an Addon or Extension you need to deselect it in List, rebuild Loader and select "Force Reinstall DSM" in Grub`