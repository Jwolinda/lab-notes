
The management infra includes Azure resource and resource groups, subscriptions, and accounts.

## Azure Resources and Resource Groups

* Resource Groups are simply a grouping of resources
* A single resource can only be in one resource group
* Resource * : 1 Resource Group
* Some resources can be moved between groups
* Actions can be applied to entire resource groups
* When provisioning, think about the structure that best suits your needs
* No hard rules about how to use the resource groups, so come up with a plan

## Azure Subscriptions

* account 1  : * subscriptions
* Azure account is an identity in Entra or in a dir that Entra trusts
* Boundaries:
	* Billing
		* Determines how an Azure account is billed for using Azure
	* Access control
		* Access-management policies at the subscription level
* Additional Subscriptions could be for:
	* Environments
	* Org Structures
	* Billing

## Management Groups

* Flexible structure of management groups and subscriptions into a hierarchy
	Hierarchy that applies a policy
	Provide user access to multiple subscriptions

* Important facts about management groups
* 10k management groups can be supported in a single directory
* A management group tree can support 6 levels of depth. Does not include root level or subscription level
* Management group and subscription only supports one parent

Links:

[[AZ 900 Training Overview]]
[[Describe Azure Physical Infrastructure]]


202501222034