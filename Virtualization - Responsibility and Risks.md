# Virtualization - Responsibilities and Risks

The Security of the **Hypervisor** is always the responsibility of the CSP.

The virtual network and virtual machine may be the responsibility of either the CSP or the customer
(Depends on the cloud service model)

## Risks associated with virtualization

- Flawed hypervisor can facilitate inter-vm attacks
- Network traffic between VMs is not necessarily visible
- Resource availability for VMs can be impacted
- VMs and their disk images are simply files, can be portable and movable. 

## Security Recommendation for the hypervisor

- Install all updates to the hypervisor as they are realeased by the vendor

- Restrict administrative access to the management interfaces of the hypervisor.

- Capabilities to monitor the security of activity occuring between guest operating systems (VMs).

> All the responsibility of the CSP

## Security Recommendations for the Guest OS

- Install all updates to the guest OS promptly

- Back up the virtual drives used by the guest OS on a regular basis

> Customer responsibility, though the CSP may provide tools

# Virtualization - Network Security 

## The CSP's Hypervisor security includes:

- preventing physical access to the servers
- limiting both local and remote access to the hypervisor

The virtual network between the hypervisor and the VM is also a potential attack surface. 

Responsibility for security in this layer is often shared between the CSP and the customer.

These components include virtual network, virtual switches, virtual firewalls, and virtual IP addresses, etc. 
(Responsibility varies by model (Iaas, PaaS, SaaS))

# Virtualization Focused Attacks

## VM Escape

Where an attacker gains access to a VM, then attacks either the host machine that holds all VMs, the hypervisor, or any of the other VMs. 

Or a malicious user breaks the isolation between VMs running ona hypervisor by gaining access outside their VM. 

> ***Protection***: Ensure patches on hypervisor and VMs are always up to date. Ensure guest privileges are low, server-level redundancy and IPS/IDS protection. 