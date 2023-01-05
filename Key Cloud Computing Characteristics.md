# Key Cloud Computing Characteristics

The NIST definition of cloud computing describes certain characteristics that clouds share. Not every third-party solution is a cloud solution. 

## On-Demand Self-Service

A service that can be rapidly provisioned and released with minimal management effort or service provider interaction.. this means the user must be able to provision these services simply and easily when thy are needed. 

For example expanding the storage space or creating an account requires the involvement of people other than the customer. This access is automated and provided via a dashboard or other simple interface. 

This can facilitate poor practices often labeled as *shadow IT*. The ease with which a service can be provisioned makes it easy for an individual, team, or department to bypass company policies and procedures that handle the provisioning and control of IT services. A team that wants to collaborate may chose OneDrive, Dropbox, SharePoint, or another service to facilitate collaboration. This can lead to sensitive data being stored in locations that do not adhere to required corporate controls and places the data in locations that do not adhere to required corporate controls and places the data in locations the larger business is unaware of and cannot adequately protect. If this behavior is allowed to proliferate, the organization can lose control of it's sensitive data processes.

## Broad Network Access

Cloud services assume the presence of a network. For public and community clouds, this is the Internet. For a private cloud, it could be the corporate network-Generally an IP-based network. In either case, cloud services are not local solutions that exist on a network in the cloud. Without broad and ubiquitous network access, the cloud becomes inaccessible and is no longer useful. 

Not all protocols and services on IP-based networks are secure. Part of the strategy to implementing a secure cloud solution is to choose secure protocols and services.  For example protocols like HTTPS and SFTP should be used over insecure protcols like HTTP and FTP. If you are able to access the cloud service and obtain access to your data anywhere in the world so can others. The need for identification and authentication becomes more importanin in this public facing environment. 

Securing cloud services can be improved by including improved password requirements, Multifactor Authentication (MFA), Virtual Private Networks (VPNs), etc. The increased security needs where security is shared between the CSP and customer makes these steps more important.

## Multitenancy

One way to get the improved efficiencies of cloud computing is through the sharing of infrastructure. A server may have more than one company purchasing access to its resources. These resources are shared by the tenants. Like an apartment building, these tenants share resources and services but have their own dedicated space. Virtualization allows the appearance of single tenancy in a m