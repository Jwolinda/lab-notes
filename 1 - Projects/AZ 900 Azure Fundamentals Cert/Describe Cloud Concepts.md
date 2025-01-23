
* Supports hosting
* VMs
* AI
* Sandbox is a temporary environment to do hands on testing
* Module goals:
	* Define cloud computing
	* Describe the shared responsibility model
	* Define cloud models, including public, private, and hybrid
	* Identify appropriate use cases for each cloud model
	* Describe consumption base model
	* Compare cloud pricing models

## Cloud Computing

* Deliver of computing services over the internet.
* Infra
	* Storage
	* VMs
	* Databases
	* Networking
* Expansion
	* IoT
	* ML
	* AI

## Shared Responsibility Model

* Traditional
	* IT Teams are responsible for
		* Security
		* Maintenance
			* Physical space
			* Servers
		* Upgrades and replacements
		* Versioning
* Shared Responsibility
	* Shared between provider and consumer
	* Provider
		* Physical Security
		* Power
		* Cooling
		* Network Connectivity
	* Consumer
		* Data and Information
		* Access Security
* Responsibility is tied to service type:
	* IaaS
	* PaaS
	* SaaS
* Always responsible for
	* The information and data stored in the cloud
	* Devices that are allowed to connect
	* Accounts and identities of the people, services, and devices within your org
* Cloud provider is always responsible for
	* The physical datacenter
	* The physical network
	* The physical hosts
* Service model will determine responsibility for things like
	* Operating Systems
	* Network Controls
	* Applications
	* Identity and infrastructure

## Cloud Models

* The three Main types are private, public, and hybrid
* Private Cloud
	* A private cloud is an evolution of the original datacenter
	* It is used only by one entity
	* Greater control
	* Greater Cost and fewer benefits compared to public
	* This can be hosted from your on site datacenter or offsite by third party (PCB setup)
* Public Cloud
	* Built, controlled, and maintained by a third-party cloud provider
	* Anyone who wants to purchase cloud services can access and use resources
	* General public availability is a key diff between public and private clouds
* Hybrid
	* A computing environment that uses both public and private clouds in an inter-connected environment (also PCB)
	* Can help manage surge in temporary demand
	* Used to provide an extra layer of security

|**Public cloud**|**Private cloud**|**Hybrid cloud**|
|---|---|---|
|No capital expenditures to scale up|Organizations have complete control over resources and security|Provides the most flexibility|
|Applications can be quickly provisioned and deprovisioned|Data is not collocated with other organizations’ data|Organizations determine where to run their applications|
|Organizations pay only for what they use|Hardware must be purchased for startup and maintenance|Organizations control security, compliance, or legal requirements|
|Organizations don’t have complete control over resources and security|Organizations are responsible for hardware maintenance and updates||
* Multi-cloud
	* You can use multiple public cloud providers
* Azure Arc
	* Set of technologies that helps manage cloud env
	* Public, private, or multi-cloud
* Azure VMWare Solution
	* Lets you run you VMWare workloads in Azure with seamless integration/scalability

## Consumption-based Model

* Two types of expenses to consider
	* Capital Expenditure (CapEx)
		* One-time, upfront expenditure
			* New building
			* Repaving Parking Lot
			* Datacenter
	* Operational Expenditure (OpEx)
		* Spending money over time
			* Renting a con center
			* leasing a company vehicle
			* cloud services
* Cloud computing falls under OpEx
* Pay for what you use
* Benefits
	* No upfront costs
	* No need to purchase an manage infra that might not be used fully
	* Pay for more resource at time they're needed
	* Stop paying when no longer needed
* Trad datacenters make you estimate what you'll need and when.
* Cloud computing lets you
	* Plan and manage your operating costs
	* Run infra more efficiently
	* Scale as your business needs change

Links:

[[AZ 900 Training Overview]]

202501220535