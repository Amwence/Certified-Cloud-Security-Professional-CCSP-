# Business Continuity

## Business Continuity Plan (BCP)

The overall orgainzational plan for how to continue business

- Focuses on the ***Whole Business*** whereas DRP focuses on the ***technical aspects of recovery***
- Will cover communications and processes more broadly
- BCP is an umbrella policy and DRP is part of it

## Disaster Recovery Plan (DRP)

The plan for recovering from a disaster impacting IT and returning the IT infrastructure to operation.

- Focuses on the ***technical aspects of recovery*** whereas BCP focuses on ***Whole Business****

- Disaster Recovery is built into cloud architecture
    - ***Region Pairs*** addresses site level failure (if a region goes down, it automatically goes up at it's region pair. Region pairs are 300+ miles apart, selected by CSP)

    - ***Availability Zones*** address datacenter failures within a cloud region (A CSP region like East US includes multiple datacenters)

    - ***Availability Sets*** - address rack level failures within a regional datacenter (consists of two or more **fault domains** for power, network, etc.)

## Business Impact Analysis

A business impact analysis (BIA) contains two important items

1. A cost benefit analysis (CBA)
    - A ***Cost-Benefit Analysis*** lists the benefits of the decisions alongside their corresponding costs. 
    - CBA can be strictly quantitative: adding the financial benefits and subtracting the associated costs to determine whether a decision will be profitable. 

    > A thorough cost-benefit analysis will consider intangible benefits (those you cannot calculate directly. "qualitative analysis")

2. A calculation on the return on investment (ROI)

## Functional Security Requirements

- Functional Security requirements define a system or its component and specifies what it must do. Captured in use cases, defined at a component level. 
    - Example: application forms must protect against injection attacks. (writing input validation into our webapp)

- Non-Functional Security Requirements specify the system's quality, characteristics, or attributes.
    - Apply to the whole system (system level)
    - Example: Security certifications are non-functional