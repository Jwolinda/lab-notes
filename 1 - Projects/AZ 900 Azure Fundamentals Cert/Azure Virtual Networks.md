Extension of your on-prem network with resources that link other Azure Resources.

Following Network Capabilities
* Isolation and Segmentation
* Internet communications
* Communication between Azure resources
* Communicate with on-premises resources
* Route network traffic
* filter network traffic
* Connect virtual networks

Endpoint
* Public
* Private
## Isolation and Segmentation

* Allows for multiple isolated virtual networks
* Name resolution can be used built in
* Can use internal or external DNS

## Internet Communication
You can enable incoming connections by assigning a public IP or putting the resource behind a public load balancer

## Communicate between Azure resources
You want to enable Azure resources to communicate securely with each other.
* Virtual Networks can connect not only VMs but other resources
	* App service Environment
	* Power Apps
	* Azure Kubernetes Service
	* Virtual Machine scale sets
* Service endpoints can connect to other Azure resource types
	* SQL databases
	* Storage Accounts

## Communicate with on-prem resources

Azure virtual networks enable you to link resources together in on-premises and within azure subscriptions:
*  Point to point virtual private network connections. Client computer to corporate network
* Site-to-site private networks link on-premises VPN device or gateway to Azure VPN gateway in a virtual network. Devices appear as being on the local network
* Azure ExpressRoute is a dedicated private connectivity to Azure that doesn't travel over the internet. Useful for greater bandwidth and higher levels of security.

## Route Network Traffic

* Route tables
* Border Gateway Protocol

## Filter network traffic

* Network Security Groups
* Network Virtual appliances

## Connect Virtual Networks

* Virtual network peering. 
* Peering travels on the Microsoft backbone network instead of public internet.
* UDR allows for control over routing tables between subnets within a virtual network.


Links:

[[Describe Azure Compute and Networking Resources]]

202501232000