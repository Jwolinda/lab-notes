
* Create and use DMs in the cloud.
* VMs act as IaaS
* You can customize all software running on your VM
* Ideal if you need
	* Total Control over the OS
	* Ability to run custom software
	* Use custom hosting configs
* Flexibility of virtualization in the form of IaaS, while still configuring, updating, maintaining the software
* You can use preconfigures images to provision VMs

## Scale VMs in Azure

* You can run single VMs for testing/dev or group to provide scalability, availability, and redundancy.
* Scale and Availability sets can help manage the grouping for you

## Virtual Machine Scale Sets

* These let you create and manage a group of identical, load-balanced VMS.
	* Manual configuration can lead to mistakes and drift over time
	* Have to monitor to see if scaling up or down is needed
* Virtual Machine Scale sets have Azure automate most of the work.
* Automatically increase or decrease depending on demand
* Automatically deploy a load-balancer  to make sure resources are being used efficiently
* Large-scale services:
	* Compute
	* Big Data
	* Container Workloads

## Virtual Machine Availability Sets

* Another tool to help build a more resilient, highly available environment.
* Designed to ensure that vmS STAGGER UPDATES AND HAVE VARIED POWER AND NETWORK CONNECTIVITY.
* Two ways to group VMs
	* Update Domain
		* Groups VMs that can be rebooted at the same time.
		* Allows you to apply updates while knowing that only one update domain grouping is offline at a time.
	* Fault Domain
		* Groups VMs by common power source and network switch
		* By default, split VMs across up to 3 fault domains.

* **There is no additional cost for configuring an availability set. You only pay for the VM instances you create.**

# When to Use VMs

* During testing and development
* When running applications in the cloud
* When extending your datacenter to the cloud
* During disaster recovery

## Move to the cloud with VMs

* Moving from datacenter to the cloud (lift and shift)
* Create an image of the physical server and host it within a VM with little of no changes.
* You're responsible for maintaining the installed OS and software

## VM Resources

* Picking resources associate
	* Size
	* Storage Disks
	* Networking




Links:

[[Describe Azure Virtual Machines]]
[[AZ 900 Training Overview]]

202501230617