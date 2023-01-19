### Important

  - Set onboard SATA Controller to AHCI Mode
  - Use UEFI if possible
  - Use USB Stick as first Boot device
  - Disable Fastboot/Quiet Boot
  - Disable Secure Boot
  - Disable C1E Support (to support higher ACPI states)

---

### Settings for Raid/HBA

  - Disable SATA Controller if you use a Raid or HBA Controller and your SATA Controller has no drives

---

### If you have Problems with boot

  - Enable OptionROM/OpROM
  - Disable PXE Boot
  - Disable rBAR