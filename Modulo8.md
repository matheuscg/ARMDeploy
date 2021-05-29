# Modulo 8 Blob Container

* Part of Azure Storage
* access Level
    * Private
    * blob (can access a blob)
    * container (can browser through entire container)
* virtual folder structure
* Acquire lease: lock the file
* Access Policy
    * Hot - optimized for access
    * Cool - cheaper storage, but higher access price, stored for at least 30 days
    * Archive - even cheaper to storage, hard to access,  stored for at least 180 days

# AzCopy

* Cli to manipulate file on azure storage
    * /SyncCopy make the copy localy

'''
az login

AzCopy /Source:<blob_container_source> /Dest:<blob_container_target> /Pattern:<file_pattern> /SourceKey:<blob_source_key> /DestKey:<blob_target_key> /SyncCopy
'''