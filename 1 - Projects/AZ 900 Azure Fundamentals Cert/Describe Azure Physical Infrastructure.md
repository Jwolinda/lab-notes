
## Physical Infrastructure

* Datacenters
	* Conceptually these are the same as large corporate datacenters.
	* Datacenters are grouped into Azure Regioans

## Regions

* A geographical area on the planet the contains at least one, but potentially multiple datacenters.
* Will need to decide on region where deployed
* Some services are not available depending on the Region

## Availability Zones

* Physically separate 
* Isolation Boundary
* Independent Power, Cooling, networking
* Connected via high-speed fiber optic
* A minimum of three availability zones are present in all availability zone regions.
* USe these in your apps
	* Redundancy
	* Replicate across zones
	* There is a cost associated
	Primarily for
		VMs
		Managed Disks 
		Load Balancers
		SQL Databases
* Supported services
	* Zonal Services
	* Zone-redundant Services
	* Non-regional Services
* Even with additional resiliency from availability zones, events can still be large enough to affect multiple. That's why azure has Region Pairs
## Region Pairs

* Most Regions are paired with another region within the same geography at least 300 miles away.
* Services will automatically failover to the other region in its region pair
* Not all Azure Services automatically replicate data or automatically fail back from a filed region to cross-replicate. In these scenarios, recover and replication must be configured by the customer.
* Data continues to reside within the same geography as its pair for tax and law enforcement jurisdiction purposes

## Sovereign Regions

* These are instances of Azure that are isolated from the main instance of Azure. May be needed for compliance or legal reasons.
* Regions include:
	* US DoD Central
	* US Gov Virginia
	* US Gov Iowa
	* Screened by US personnel and include additional compliance certifications
* China Region is available through a partnership with 21Vianet whereby Microsoft does not directly manage the datacenters.

Links:

[[AZ 900 Training Overview]]
[[Describe Core Architectural Components of Azure]]

202501222008