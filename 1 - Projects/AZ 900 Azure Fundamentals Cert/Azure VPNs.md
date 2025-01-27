
* A virtual private network connects two or more trusted private networks to one another over an untrusted network (typically public internet).
* Traffic is encrypted while traveling to prevent eavesdropping or other attacks.
* Safely share sensitive information

## VPN Gateways

* Deployed on a dedicated subnet
	* Connect on-premises datacenters to virtual networks through a site-site connection
	* Connect individual devices to virtual networks tough a point-to-site connection
	* Connect virtual networks to other virtual networks though a network-to-network connection
* Data transfer is encrypted.
* One VPN Gateway per virtual network
* One gateway can connect multiple locations

* Type of VPN
	* Policy-based
		* IP Address of packets that should be encrypted are specified
	* Route-based
		* IPSec tunnels are modeled as a network interface or virtual tunnel interface.

* High availability Scenarios
	* Active/Standby
	* Active/Active
	* ExpressRoute Failover
	* Zone-redundant Gateways
		* In regions that support availability zones, VPN gateways and ExpressRoute gateways can be deployed in a zone-redundant configuration. This configuration brings resiliency, scalability, and higher availability to virtual network gateways. Deploying gateways in Azure availability zones physically and logically separates gateways within a region while protecting your on-premises network connectivity to Azure from zone-level failures. These gateways require different gateway stock keeping units (SKUs) and use Standard public IP addresses instead of Basic public IP addresses.
Links:
[[Describe Azure Compute and Networking Resources]]
202501232035