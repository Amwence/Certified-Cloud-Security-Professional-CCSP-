# Network Security

> ***Network Security Groups*** Provide an additional layer of security for cloud resources

Act as a ***Virtual firewall*** for virtual networks and resource instances.(e.g. VMs, databases, subnets)

Carries ***a list of security rules*** (IP and Port Ranges) that allow or deny network traffic to resource instances. (ACL)

Provides a virtual firewall for a ***collection of cloud resources*** with the same security posture.

***NOTE: Exists in multiple CSPs. Details may vary slightly with each***

# Cloud Security Controls - NETWORK

## Segmentation

Restricting services that are permitted to access or be accessible from other zones using rules to control inbound/outbound traffic.

Rules are ***enforced by the IP address ranges*** of each subnet

Within a virtual netowrk, segmentation can be used to acheive isolation (Port filtering through a network security group)

***EXAMPLE: We can put database servers in their own subnet and restrict inbound traffic just to listening database service ports

## API Inspection and Integration

Representation State Transfer (REST) is the modern approach to writing web service APIs.

Enables multi-language support, can handle multiple types of calls, return different data formats. 

APIs published by an organizations should include ***encryptions, authentication, rate limiting, throttling, and quotas. ***

## Traffic Inspection

Packet capture in the cloud generally requires tools designed for this purpose in the environment.

Traffic is often sent direct to resources and promiscuous mode on a VM NIC not possible or effective. 

***EXAMPLE: Network Watcher (Azure), VPC traffic mirroring(AWS)

>CSPs offering tools to facilitate packet capture within customer tenant

## GEOFencing

Uses the ***Global positioning system(GPS)*** or RFID to define ***geographical boundaries.***

Once the device is taken past the defined boundaries, the security team will be alerted. 

***EXAMPLES:***

***Restrict access to system and services based on where the access attempt is being generated from.*** 

***Prevents devices from being removed from the company premises***

***NOTE: Can Identify unusual traffic patterns and prevents misuse.***