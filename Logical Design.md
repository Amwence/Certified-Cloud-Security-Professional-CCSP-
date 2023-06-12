# Logical Design

The design of a data center is an abstraction.

In the now legacy co-location (colo) scenario, customers were separated at the server rack or cage-level.

In logical data center design in the cloud, customers utilize software and services provided by the CSP. 

The Logical design of the cloud infrastructure should:

- Create Tenant Partitioning or Isolation
- Limit and Secure Remote Access
- Monitor the cloud infrastructure
- Allow for the patching and updating of systems

(CCSP exam focuses on Tenant partitioning and Access control)

# Tenant Partitioning

Logical Isolation in the CSP multitenancy makes cloud computing more affordable but creates some security and privacy concerns.
(If isolation between tenants is breached customer data is at risk)

Multitenacy:
- business centers physically housed multiple tenants
- colocation data centers supported multiple customers

The risk in these scenarios is largely physical (server, rack, cage)

In the public cloud, tenant partitioning is largely logical. 

Customers are sharing capacity across the CSP datacenter, including physical components. 

> CSP and Tenant share responsibility for implementing and enforcing controls that address the unique multitenant risks of the public cloud

## Access Control

When creating a logical data center, access control is a primary concern.

A single point of access makes access control simpler and facilitates monitoring, but any single point can become a failure point as well. 

**Hybrid Identity** (Singl login for on-premises and cloud can simplify identity and access management)

- One method of access control is to **federate** a customers existing IAM system with their CPS tenant

- Another method to facilitate IAM between cloud and on-premises resources is **Identity as a Service (IDaaS)
(Azure Active Directory (used with office 365) or Googles Cloud Identity (used with Google Workspace))

## Local and Remote Access Controls

**Remote Desktop Protocol (RDP)**: The native remote access protocol for Windows operating systems.

**Secure Shell (SSH)**: The native remote access control protocol for Linux operating systems, and common for remote management of network devices. 
(RDP and SSH both support encryption and MFA)

**Secure Terminal/Console-Based Access:** a system for secure local access. (A KVM(Keyboard Video Mouse) system with access controls)

**Jumpboxes:** a bastion host at the boundary of lower and higher security zones. (CSPs offer services for this: Azure Bastion, AWS Transit Gateway)

**Virtual Clients:** Software tools that allow remote connection to a VM for use as if it is your local machine. (e.g. Virtual Desktop Infrastructure (VDI) for contractors)

