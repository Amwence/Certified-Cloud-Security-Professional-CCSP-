# Edge Computing

- Some compute operations require processing activities to occur locally, far from the cloud.

- Common in various ***Internet of Things*** scenarios, like agricultural, science/space,military.

- All the processing of data storage is closer to the sensors rather than in the cloud data center.

***Note: with large network-connected device counts in varied locations, data encryption, spoofing protection, and Authentication are key.***

# Fog Computing

- Compliments cloud computing by processing data from IOT devices

- Often places ***Gateway Devices*** in the field to collect and correlate data ***Centrally at the edge.***

- Generally, brings cloud computing nearer to the sensor to ***Process data closer to the device***.

***Note: Important to speed processing time and reduce dependence on cloud/interent connectivity mission critical situations (e.g. healthcare)***

# Confidential Computing

*PROBLEM:* Sensitive data must be encrypted in memory before an app can process it, leaving the data vulnerable

- Confidential computing solves for this by ***isolating sensitive data*** in a protected CPU enclave during processing.

- This CPU enclave is called a ***trusted execution environment (TEE)***, secured with embedded encryption keys

- Embedded attestation mechanisms ensure that the keys are ***accessible only to authorized application code***

# DevSecOps

- A portmanteau development, security, and operations

- Integrates ***security as a shared responsibility*** throughout the entire IT lifecycle

- Builds a security foundation into DevOps initiatives. 

- Often includes ***automating*** some of the ***security gates*** in the DevOps process

# Infrastructure as code (IAC)

IAC is the ***management of cloud infrastrucutre***(networks,VMs,load balancers, and connection topology) ::***described in code***::.

Just as the same source code generates the same binary, code in the IaC model results in the same environment __every time it is applied__

IaC is a key DevOps practice and is used in conjuction with ***Continuous Integration and Continuous Delivery(CI/CD)***

***Note: IaC, CI/CD, and DevOps are standard elements of deployment, change, and release in the could DevSecOps is quickly growing in popularity.

# Compute

How does the CSP manage Compute Capacity?

The infrastructure components that deliver compute resources, such as the VMs, disk, processor, memory and network resources

## Reservation

A minimum resource that is guarunteed to a customer

## Limits

maximum utilization of compute resources by a customer (e.g. VM)

Limits are allowed to change dynamically based on current conditions and consumption

## Shares

A weighting given to a particular VM used to calculate percentage-based access to pooled resources when ther is contention. 

In cases of shortage, hosts scoring determins who gets capacity

> In Every Delivery and service model: THe CSP remains responsible for the maintenance and security of the physical components of compute

> The customer remains largely responsible for their data and their users

Between Physical components, there can be a large array of sftware and other components

> Who is responsible for each of the remaining parts varies by service and delivery model and sometimes by the CSP

***THE DETAILS SHOULD BE SPELLED OUT IN THE CONTRACT!***