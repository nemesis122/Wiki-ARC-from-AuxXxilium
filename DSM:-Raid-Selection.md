I would prefer a classic Raid (Raid 1 or Raid 10) because of Datarescue Options. SHR is also possible but we have no Way to restore the Data if something will went wrong.

<table id="b_12">
	<tbody><tr>
		<th>RAID Type</th>
		<th>Number of Drives</th>
		<th>Tolerable Drive Failures</th>
		<th>Description</th>
		<th>Storage Capacity</th>
	</tr>
	<tr>
		<td rowspan="3">SHR</td>
		<td>1</td>
		<td>0</td>
		<td rowspan="3">
			<ul>
				<li>Optimizes the volume size when combining drives of different sizes.</li>
				<li>Provides data redundancy if the volume is composed of two or more drives.</li>
				<li>Recommended for beginner users.</li>
			</ul>
		</td>
		<td>1 x (Drive size)</td>
	</tr>
	<tr>
		<td>2-3</td>
		<td>1</td>
		<td rowspan="2">Optimized by the system.</td>
	</tr>
	<tr>
		<td>≧4</td>
		<td>1-2</td>
	</tr>
	<tr>
		<td>Basic</td>
		<td>1</td>
		<td>0</td>
		<td>
			<ul>
				<li>Composed of one drive as an independent unit.</li>
				<li>Does not provide data redundancy.</li>
			</ul>
		</td>
		<td>1 x (Drive size)</td>
	</tr>
	<tr>
		<td>JBOD</td>
		<td>≧1</td>
		<td>0</td>
		<td>
			<ul>
				<li>Combines a collection of drives into a single storage space, with a capacity equal to the sum of all drives' capacity.</li>
				<li>Does not provide data redundancy.</li>
			</ul>
		</td>
		<td>Sum of all Drive sizes</td>
	</tr>
	<tr>
		<td>RAID 0</td>
		<td>≧2</td>
		<td>0</td>
		<td>
			<ul>
				<li>Features "striping," a process of dividing data into blocks and spreading the data blocks across several drives to enhance performance.</li>
				<li>Does not provide data redundancy.</li>
			</ul>
	    </td>
		<td>Sum of all drive sizes</td>
	</tr>
	<tr>
		<td rowspan="3">RAID 1</td>
		<td>2</td>
		<td>1</td>
		<td rowspan="3">
			<ul>
				<li>Writes identical data to all the drives simultaneously.</li>
				<li>Provides data redundancy.</li>
			</ul>
		</td>
		<td rowspan="3">Smallest drive size</td>
	</tr>
	<tr>
		<td>3</td>
		<td>2</td>
	</tr>
	<tr>
		<td>4</td>
		<td>3</td>
	</tr>
	<tr>
		<td>RAID 5</td>
		<td>≧3</td>
		<td>1</td>
		<td>
			<ul>
				<li>Implements block-level striping with parity data distributed across all member drives, thus providing data redundancy more efficiently than RAID 1.</li>
			</ul>
		</td>
		<td>(N – 1) x (Smallest drive size)</td>
	</tr>
	<tr>
		<td>RAID 6</td>
		<td>≧4</td>
		<td>2</td>
		<td>
			<ul>
				<li>Implements two layers of data parity to store redundant data equal to the size of two drives, providing a greater degree of data redundancy than RAID 5.</li>
				<li>Supports creating <a href="https://kb.synology.com/en-id/DSM/tutorial/What_is_Btrfs_Peta_Volume" target="_blank">a Btrfs volume of up to 1 PB in size</a>, which is only available on certain Synology NAS models and under specific conditions.</li>
			</ul>
		</td>
		<td>(N – 2) x (Smallest drive size)</td>
	</tr>
	<tr>
		<td>RAID 10</td>
		<td>≧4<br>(even number)</td>
		<td>Half of the total drives</td>
		<td>
			<ul>
				<li>Provides the performance of RAID 0 and data protection level of RAID 1, combining  drives into groups of two in which data is mirrored.</li>
			</ul>
		</td>
		<td>(N / 2) x (Smallest drive size)</td>
	</tr>
	<tr>
		<td>RAID F1</td>
		<td>≧3</td>
		<td>1</td>
		<td>
			<ul>
				<li>Implements block-level striping with parity data distributed across all member drives.</li>
				<li>Writes more parity information on a certain drive.</li>
				<li>Recommended for an all-flash array.</li>
			</ul>
		</td>
		<td>(N – 1) x (Smallest SSD size)</td>
	</tr>
</tbody></table>