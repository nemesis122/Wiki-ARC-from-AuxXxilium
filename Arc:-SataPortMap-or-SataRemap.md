### Only necessary for nonDT Models

* First: If you don't know anything about SataPortMap, SataRemap or AhciRemap. Look at Sysinfo in Arc and look at your Drive Mapping. Now you can choose an Option.

### Use SataPortMap (controller active Ports)

* Normally you can select this. If you have empty Ports after used Sata Ports, this will remove the unused Ports.

### Use SataPortMap (controller max Ports)

* This sets the SataPortMap to max Portcount of your Controller.

### Use SataRemap (remove blank drives)

* This Option removes empty Ports, if you see some empty or dummy Ports of your Controller.
* It removes the Drive 1 empty Slot while using ESXi. (You have to Map all Drives to SATA Controller, SAS/SCSI Ports will not be usable.)

### Use AhciRemap (remove blank drives) <- (experimental)

* This Option removes empty Ports, if you see some empty or dummy Ports of your Controller.
* It removes the Drive 1 empty Slot while using ESXi. (You have to Map all Drives to SATA Controller, SAS/SCSI Ports will not be usable.)