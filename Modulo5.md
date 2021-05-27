## Modulo 5 Azure Storage Accounts

* 2 cents per megabyte per month
* Unique Storage Name
* Performance Standard or Premium
* Account Kind v2 is the default, v1 for legacy and blobstorage for blobs
* Replication:
    * LRS 3 Copies of each file, same location
    * GRS 6 Copies of each file, local and other location
    * Read-Acess geo-redundant (read from GRS and WRITE on LRS)
    * ZRS Zone redundant
    * GZRS Global Zone redundant
* Access Tier
    * Cool
    * Hot
* Networking
    * Public all networks
    * Public endpoint selected networks
    * Private endpoint
* Advanced
    * Secure transfer, encrypted trafic
    * Large file shares
    * Blob Soft delete (Recycle bin)
    * Data Lake Storage Gen2

## Access keys

Keys and Connections Strings to connect to Storage

## Shared Access Signature (SAS Token)

Limited and configurable access key. Used to access storage via browser

## Containers

All blob must be in a container

* Access level
    * Private
    * Blob (public blob)
    * Container (public container and blob)

## File shares

Network storage using SMB protocol

## Tables

## Queues