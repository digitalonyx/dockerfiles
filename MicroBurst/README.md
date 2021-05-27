## MicroBurst Dockerfile

Azure Recon tool developed by NetSPI https://github.com/NetSPI/MicroBurst

## Usage
To run the container:
docker run --rm -it microburst 

`--rm`will automatically remove the container upon exiting.

Enumerate against a target:

#Enumerate Services using MicroBurst

`Invoke-EnumerateAzureSubDomains -Base <targetname>`

#Look for Public Blob containers and Objects

`Invoke-EnumerateAzureBlobs -Base <targetname>`

#Web Request to exposed public Azure EnumerateAzureBlobs

`Invoke-WebRequest -Uri "domain found in previous Enumerate" -Outfile "whatever.txt"`

