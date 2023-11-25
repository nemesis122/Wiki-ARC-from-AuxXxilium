<html>
<body>
<!--StartFragment--><h2 id="b_8" style="box-sizing: border-box; margin: 0px 10px 0.5em 0px; color: rgb(60, 70, 80); background-color: rgb(255, 255, 255); border-bottom: 1px dashed rgb(215, 225, 235); padding-top: 1em; font-weight: 700; font-size: 20px; line-height: 1.5; font-family: Inter, Arial, Helvetica, Verdana, sans-serif; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">Supported RAID Types</h2><p id="b_10" style="box-sizing: border-box; line-height: 1.5; margin: 0px; padding: 0px 0px 6px; border-collapse: collapse; font-size: 16px; color: rgb(80, 90, 100); font-family: Inter, Arial, Helvetica, Verdana, sans-serif; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">This table provides a brief overview of different RAID types supported by Synology NAS, including storage capacity, the minimum number of drives required for the RAID type, and the number of drive failures that can be tolerated before data loss occurs.</p><div class="kb_detail_table" style="box-sizing: border-box; width: 1050px; overflow: auto; padding-bottom: 20px !important; color: rgb(46, 55, 66); font-family: Inter, Arial, Helvetica, Verdana, sans-serif; font-size: 18px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">
RAID Type | Number of Drives | Tolerable Drive Failures | Description | Storage Capacity
-- | -- | -- | -- | --
SHR | 1 | 0 | Optimizes the volume size when combining drives of different sizes.Provides data redundancy if the volume is composed of two or more drives.Recommended for beginner users. | 1 x (Drive size)
2-3 | 1 | Optimized by the system.
≧4 | 1-2
Basic | 1 | 0 | Composed of one drive as an independent unit.Does not provide data redundancy. | 1 x (Drive size)
JBOD | ≧1 | 0 | Combines a collection of drives into a single storage space, with a capacity equal to the sum of all drives' capacity.Does not provide data redundancy. | Sum of all Drive sizes
RAID 0 | ≧2 | 0 | Features "striping," a process of dividing data into blocks and spreading the data blocks across several drives to enhance performance.Does not provide data redundancy. | Sum of all drive sizes
RAID 1 | 2 | 1 | Writes identical data to all the drives simultaneously.Provides data redundancy. | Smallest drive size
3 | 2
4 | 3
RAID 5 | ≧3 | 1 | Implements block-level striping with parity data distributed across all member drives, thus providing data redundancy more efficiently than RAID 1. | (N – 1) x (Smallest drive size)
RAID 6 | ≧4 | 2 | Implements two layers of data parity to store redundant data equal to the size of two drives, providing a greater degree of data redundancy than RAID 5.Supports creating a Btrfs volume of up to 1 PB in size, which is only available on certain Synology NAS models and under specific conditions. | (N – 2) x (Smallest drive size)
RAID 10 | ≧4(even number) | Half of the total drives | Provides the performance of RAID 0 and data protection level of RAID 1, combining drives into groups of two in which data is mirrored. | (N / 2) x (Smallest drive size)
RAID F1 | ≧3 | 1 | Implements block-level striping with parity data distributed across all member drives.Writes more parity information on a certain drive.Recommended for an all-flash array. | (N – 1) x (Smallest SSD size)

</div><!--EndFragment-->
</body>
</html>Supported RAID Types
This table provides a brief overview of different RAID types supported by Synology NAS, including storage capacity, the minimum number of drives required for the RAID type, and the number of drive failures that can be tolerated before data loss occurs.

RAID Type	Number of Drives	Tolerable Drive Failures	Description	Storage Capacity
SHR	1	0	
Optimizes the volume size when combining drives of different sizes.
Provides data redundancy if the volume is composed of two or more drives.
Recommended for beginner users.
1 x (Drive size)
2-3	1	Optimized by the system.
≧4	1-2
Basic	1	0	
Composed of one drive as an independent unit.
Does not provide data redundancy.
1 x (Drive size)
JBOD	≧1	0	
Combines a collection of drives into a single storage space, with a capacity equal to the sum of all drives' capacity.
Does not provide data redundancy.
Sum of all Drive sizes
RAID 0	≧2	0	
Features "striping," a process of dividing data into blocks and spreading the data blocks across several drives to enhance performance.
Does not provide data redundancy.
Sum of all drive sizes
RAID 1	2	1	
Writes identical data to all the drives simultaneously.
Provides data redundancy.
Smallest drive size
3	2
4	3
RAID 5	≧3	1	
Implements block-level striping with parity data distributed across all member drives, thus providing data redundancy more efficiently than RAID 1.
(N – 1) x (Smallest drive size)
RAID 6	≧4	2	
Implements two layers of data parity to store redundant data equal to the size of two drives, providing a greater degree of data redundancy than RAID 5.
Supports creating [a Btrfs volume of up to 1 PB in size](https://kb.synology.com/en-id/DSM/tutorial/What_is_Btrfs_Peta_Volume), which is only available on certain Synology NAS models and under specific conditions.
(N – 2) x (Smallest drive size)
RAID 10	≧4
(even number)	Half of the total drives	
Provides the performance of RAID 0 and data protection level of RAID 1, combining drives into groups of two in which data is mirrored.
(N / 2) x (Smallest drive size)
RAID F1	≧3	1	
Implements block-level striping with parity data distributed across all member drives.
Writes more parity information on a certain drive.
Recommended for an all-flash array.
(N – 1) x (Smallest SSD size)