# Network Attacks

## Denial of Service (DoS)

Is a resource consumption attack intended to prevent activity on a victimized system. 

## Distributed Denail of Service Attack (DDoS)

A DoS attack utilizing multiple compromised computer systems as sources of attack traffic.

> ***Countermeasures:*** Firewalls, routers, intrusion detection (IDS), SIEM (Security Information and Event Management), disable broadcast packets entering/leaving, disable echo replies, patching.

# Types of DDoS Attacks

## Network

Volume based attacks targeting flaws in network protocols, often using botnets, using techniques such as UDP, ICMP flooding, or SYN flooding (TCP-based).

## Application

Exploit weakness in the application layer(Layer 7) by opening connections and initiating process and transaction requests that consume finite resources like disk space and available memory.

## Operational Technology (OT)

Targets the weaknesses of software and hardware devices that control systems in factories, power plants, and other industries, such as IoT devices.

***Often target weaknesses using the network and application techniques described above***

> ***Countermeasures:*** IDS,IPS, rate-limiting, firewall ingress/egress filters