# Virtualiztion

- Host Machines run on physical hardware

- Host Machine provides services to several virtualized guest machines

- The Hypervisor tricks each guest into thinking it is running on dedicated hardware

- Type 1 Hypervisor - Runs on physical hardware and is bare-metal. The Virtual machines are running directly off of the hypervisor and is most commonly found in data centers.

- Type 2 Hypervisor - Runs in an Operating system. So there needs to be an operating system installed between the machine and the hypervisor runs as a program on that operating system. Is most commonly found on personal computers. Things like vmware workstation, Parallels, and VirtualBox. 

# Virtualization Security

- Virtual Machine Isolation is Critical

- Each Server must have access to only it's own memory and storage. 

- VM escape attacks attempt to break out of the guest environment

***VM Escape Attack - is the process of a program breaking out of the virtual machine on which it is running and interacting with the host operating system. 

Virtualization platforms must be patched against security vunlerabilities. 

- VM Sprawl - Leads to unused and unmaintained servers. 

- Ephemeral Computing - Resources allocated for a short time. 