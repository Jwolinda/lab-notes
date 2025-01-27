
Storage Accounts provide a unique namespace for you storage data  that's accessible from anywhere over http or https. 
* Secure
* Highly Available
* Massively Scalable

Redundancy Options
* Locally redundant storage (LRS)
* Geo-redundant Storage (GRS)
* Read-access geo-redundant storage (RA-GRS)
* Zone-redundant Storage (ZRS)
* Geo-zone-redundant Storage (GZRS)
* Read-access geo-zone-redundant storage (RA-GZRS)

Types available
* Standard General Purpose V2
	* Standard storage account type for
		* Blobs
		* File shares
		* queues
		* tables
	* Recommended for most scenarios
* Premium block blobs
	* Premium type for block blobs and append blobs
	* High transaction rates or consistently low storage latency
* Premium File Shares
	* Premium storage for file shares only
	* Enterprise or high-performance scale applications.
	* Supports both SMB and NFS Fileshares
* Premium page blobs
	* Premium storage account for page blobs only 

Endpoint Naming Convention

	|**Storage service**|**Endpoint**|
	|---|----|
	|Blob Storage|https://<storage-account-name>.blob.core.windows.net|
	|Data Lake Storage Gen2|https://<storage-account-name>.dfs.core.windows.net|
	|Azure Files|https://<storage-account-name>.file.core.windows.net|
	|Queue Storage|https://<storage-account-name>.queue.core.windows.net|
	|Table Storage|https://<storage-account-name>.table.core.windows.net|
	


Links:

[[Describe Azure Storage Services]]

202501250503