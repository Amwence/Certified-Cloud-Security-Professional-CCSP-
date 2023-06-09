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