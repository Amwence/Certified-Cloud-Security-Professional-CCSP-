# Virtualization Security

## Containerization

A lightweight, granular, and portable way to package applications for multiple platforms.

Reduces overhead of server virtualization by enabling containerized apps to run on a shared OS kernel.(Containers do not have their own OS!)

***EXAMPLE: Docker and Kubernetes***

***NOTE: Can be used in some cases to isolate existing applications developed to run in a VM with a dedicated operating system***

- Type 1 Hypervisor = Bare metal (VMware ESXI, Microsoft Hyper V, KVM)
    - Each VM has its own OS kernal and memory resulting in more overhead

- Containers are isolated, but share a single OS kernel, as well as bins/libs

### Core components in a container platform (Docker, Kubernetes):

- Orchestration/scheduling controller
- Network, storage
- Container images (VM Template)
- Container registry (Where container images are stored)

The isolation is logical, isolating process, compute, storage, network, secrets, and management plane.

## Serverless Technology

- Is a cloud-native development model that allows developers to build and run applications withou having to manage servers. There are still servers in serverless, but they are abstracted away from app developement. (a way to build and run things without managing infrastructure)
- Use API gateways as security buffers (to avoid DDoS attacks)
- Configure secur authentication (Oauth, SAML, OpenID Connect, MFA)
- Separate deve and prod environments, implement least privelege

## Ephemeral Computing

- The practice of creating a virtual computing environment as a need arises.
- environment is destroyed once needs are met, and resources are no longer needed.  (Used in autoscaling (Elasticity))