# System Storage and Communication Protection

Encrypt and protect data: 

- at rest
- in transit
- in use

Protect Systems and Services:

- DoS/DDoS
- Boundary (ingress and egress)
- Key Management

Security Practices: (People and processes)

- Automation of configuration
- Responsibilities for protecting cloud systems and services
- Monitoring and maintenance

Properly securing information systems can be a difficult task due to the sheer number of elements that make up a system. 

Breaking systems down into components and then applying security controls can make the overall task more manageable. 

> One source for controls is [Nist Special Publication 800-53](https://doi.org/10.6028/NIST.SP.800-53r5), "Security and Privacy Controls for Information Systems and Organizations", which contains a family of controls specific to systems and communications

The NIST control family includes 50+ controls, many relevant to system, storage, and communication protection

## Policy and Procedures

Establish requirements for system protection, and define the purpose, scope, roles, and responsibilities needed to achieve it. 

## Separation of System and User Functionality

A basic security principle that ensures that no single person can control all the elements of a critical function of the system. 

Separating user and admin functions can also prevent users from altering processes or misconfiguring systems. 

## Security Function Isolation

Separating security-specific functions from other roles is another example of separation of duties (e.g. configuring data security controls like encryption and logging configuration)

## Denial-of-Service Protection

A Disruptive attack at scale that is more difficult for smaller organizations to combat effectively.

Most CSPs offer DoS/DDoS mitigation as a service, and there are also dedicated providers like Akamai and Cloudflare. 

e.g. Azure DDoS, AWS Shield, Google Cloud Armor

## Boundary Protection

Deals with both ingress and egress protections, including:

- Preventing malicious traffic from entering the network
- Preventing malicious traffic from leaving your network
- Protecting against data loss (exfiltration)
- Configuring rules/policies in routers, gateways, or firewalls

## Cryptographic Key Establishment and Management

