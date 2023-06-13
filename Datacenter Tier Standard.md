# DataCenter Tier Standard

Tier IV: Fault-tolerant site infrastructure

Tier III: Concurrently maintainable site infrastructure

Tier II: Redundant Site Infrastructure

Tier I: Basic Site Infastructure

(Higher Tier Higher availability)

Availablity and uptime are often used interchangeably but there is a difference. 

**Uptime** simply measures the amount of time a system is running.

**Availability** encompasses availability of the infrastructure, applications, and services

Generally expressed as a number of 9's, such as five nines or 99.999% availability

> Should be measured by the cloud customer to ensure the CSP is meeting their SLA agreements

The **Uptime Institute** publishes specifications for physical and environmental redundancy, expressed as tiers, that organizations can implement to achieve high availability (HA). 

## Tier 1: Basic Site Infrastructure

Involves no redundancy and the most amount of downtime in the event of an unplanned maintenance or an interruption

Must have an uninterruptible power supply that can handle brief power outages, as well as sags and spikes

Must have dedicated cooling equipment that can run on 24/7, and a generator to handle extended power outages 

Expected availablility is 99.671% 

## Tier 2: Redundant Site Infrastructure

Provides partial redundancy, meaning an unplanned interruption will not necessarily cause an outage

Adds redundant components for important cooling and power systems

Facilities must also have the ability to store additional fuel to support the generator

expected to provide 99.741% availability

## Tier 3: Concurrently Maintainable Site Infrastructure

Adds even more redundant components

Has a major advantage in that it never needs to be shut down for maintenance

Enough redundant components that any component can be taken offline for maintenance and data center continues to run

Expected to provide 99.982% availability

## Tier 4: Fault-Tolerant Site Infrastructure

Can withstand either planned or unplanned activity without affecting availability

This achieved by eliminating all single points of failure

Requires a fully redundant infrastructure, including dual commercail power feeds, dual backup generators

Expected availability 99.995%
