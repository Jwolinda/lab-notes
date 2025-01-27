
* Stores multiple copies
* Redundancy
* Data is always replicated 3 times in the primary region
	* LRS
	* ZRS
* LRS is the lowest cost redundancy option
* LRS is 11 nines of durability over a given year
	* Could be gone with fire, flood, etc.
	* Recommend ZRS GZRS GRS
* ZRS replicates data synchronously across 3 availability zoners in the primary region
* Durability of 12 nines over a year
* Still accessible for read and write operations if a zone becomes unavailable
* Azure deals with DNS repointing
* For high durability  you can replicate to a secondary physical region (GRS)
* Region is based on Azure region pairs and cannot be changed
* GRS
	* 16 Nines
	* Like running LRS in two regions
* GZRS
	* 16 nines
	* ZRS in primary region and LRS in secondary
	* Data in second region is not available for read or write unless there is failover. If there is failures in primary you may fail over to the second region data
* RA allows read allowed in the secondary regions at all times for GZRS and GRS
* Remember that the data in your secondary region may not be up-to-date due to RPO (Recovery Point Objective)

Links:

[[Azure Storage Accounts]]
[[Azure Storage Redundancy]]

202501250513