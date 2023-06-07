# Virtualization Focused Attacks

## VM Escape

Where an attacker gains access to a VM, then attacks either the host machine that holds all VMs, the hypervisor, or any of the other VMs.

> ***Protection:*** Ensure patches and hypervisor and VMs are always up to date, gues privileges are low. Server-level redundancy and HIPS/HIDS (Hardware intrusion detection/prevention) also effective.

## VM Sprawl

When ***unmanaged VMs*** have been deployed on your network. Because It doesn't know it is there, it may not be patched and protected, and thus more vulnerable to attack. 

> ***Avoidance***: Enforcement of security policies for adding VMs to the network, as well as periodic scanning to identify new virtualization hosts. 

### All of the above apply to both VM containers and container hosts. 