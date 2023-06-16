### Important for Native Installation

  - Set onboard SATA Controller to AHCI Mode
  - Disable Fastboot/Quiet Boot
  - Disable Secure Boot
  - Use USB Stick as first Boot device

### Recommended for Native Installation

  - Use UEFI (if possible)
  - Enable Above 4G Decoding (possible that your Hardware need to disable it)
  - Disable C1E Support (to support higher ACPI states, not on every Board needed)
  - Optional: Disable all unused Devices - DSM only can handle 8 PCI Strings

---

### Recommended for Raid/HBA

  - Disable SATA Controller if you use a Raid or HBA Controller and your SATA Controller has no drives

---

### If you have Problems with boot

  - Disable Serial Console in ILO, IPMI and so on...
  - Disable PXE Boot
  - Disable rBAR
  - Disable SR-IOV

---

### If you have Problems with VMM

  - Disable Intel VT-d or AMD IOMMU
  - Enable Vanderpool / SVM / VT-x / AMD-V