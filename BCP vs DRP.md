# BCP vs DRP

Business continuity planning vs Disaster Recovery planning what is the difference?

BCP focuses on the whole business

DRP focuses more on the technical aspects of recovery. 

BCP will cover communications and process more broadly

BCP is an umbrella policy and DRP is part of it. 

# Goals of DRP and BCP

Minimizing the effects of a disaster by:

**Improving responsiveness** by employees in different situations.

**Easing confusion** by providng written procedures and participation in drills

Helping **make logical decisions** during a crisis

# BCP Definitions

## BRP (Business Resumption Plan)

THe plan to move from disaster recovery site back to your business environment or back to normal operations. 

## MTBF (Meant Time Between Failures)

a time determination for how long a piece of IT infrastructure will continue to work before it fails

## MTTR (Mean Time to Repair)

a time determination for how long it will take to get a piece of hardware/software repaired and back on-line

## MTD (Max Tolerable Downtime)

The amount of time we can be without the asset that is unavailable BEFORE we must declare a disaster and initiate our disaster recovery plan. 

# BCDR Strategy

## BCP (Business Continuity Plan)

The overall organization plan for "how-to" continue business after an event has occured.

A proactive risk mitigation strategy that contains likely scenarios that could affect the organization and guidance on how the organization should respond
(Sometimes called a continuity of operations plan (COOP))

## DRP (Disaster Recovery Plan)

the plan for recovering from an IT disaster and having the IT infrastructure back in operation. 

# Business Impact Analysis

The Business Impact Analysis (BIA) is used to determine which processes are critical and which are not.

Measures the impact of specific systems and processes.

Any that are deemed critical to the organization's functioning must be prioritized in an emergency situation.

A BIA typically contains a cost-benefit analysis (CBA) and a calculation of the return on investment(ROI)

# BCP/DRP from a CSP Perspective

> A cloud data center that is affected by a natural disaster will likely activate multiple BCPs and DRPs.

CSP will activate both plans to deal with the interruption to their service.

One key element of the BCP is communicating incident status to relevant parties. 

> The customer is responsible for determining how to recover in the case of a disaster in the cloud. 

Customers may choose to implement backups, or utilize multiple availability zones, load balancers, or other techniques. 

CSPs can further protect customers by not allowing two availability zones within a single physical datacenter within a cloud region.

# Communication Plan

The plan that details how relevant stakeholders will be informed in event of an incident. (like a security breach)

Would include plan to maintain confidentiality such as encryption to ensure that the event does not become public knowledge.

Contact list should be maintained that includes stakeholders from the government, police, customers, suppliers, and internal staff. 

> Compliance regulations, like GDPR, include notification requirements, relevant parties and timelines. 

> Confidentiality among internal stakeholders is desirable so external stakeholders can be informed in accordance with the plan. 

When we have an incident, there are multiple groups of relelvant stakeholders that we need to inform and manage, and may include:

- Internal Stakeholders
- Cyber insurance providers
- Business partners
- Customers
- Law enforcement

A **stakeholder** is a party with an interest in an enterprise: corporate stakeholders include investors, employees, customers, and suppliers

> Regulated industries, such as banking and healthcare will have requirements driven by the regulations governing their industries. 

# Business Requirements

## Recovery Point Objective (RPO)

is the age of data that must be recovered from backup storage for normal operations to resume if a system or network goes down

## Recovery Time Objective (RTO)

is the duration of time and a service level within which a business process must be restored after a disaster in order to avoid unacceptable consequences associated with a break in continuity. 

(SLAs between a company and customers will influence RPO and RTO)

## Recovery Service Level (RSL)

Measures the computer resources needed to keep production environments running during a disaster.

is a percentage measure (0-100%) of how much computing power you will need during a disaster

based upon a percentage of computing used by production environments versus others, such as development, test, and QA
(Answers what needs to be migrated to keep production running?)

> **EXAMPLE:** a 10 web server environment that uses 8 for dev, test, and QA, only 2 would need to be migrated for production

# BCDR Plan Creation, Implementation, and Testing

1. Design
    - Based on the priorities from the business impact analysis(BIA)
    - FEMA and Infragard can advise us on likely disasters for a region
2. Implement the Plan
    - Implement the plan to protect critical business functions
    - Identifying key personnel is a crucial implementation step
3. Test the Plan
    - Testing ensures both the BCP/DRP function as expected
    - AND that the people involved know their roles and responsibilities
    - Testing both BCP and DRP plans is essential
4. Report and Revise
    - BCP/DRP should be revised as necessary based on test results
    - BCP/DRP plans evolve and need refinement over time

    # DRP Test Scenarios

    A BCP and DRP should be tested **ATLEAST ANNUALLY**

    Common Disaster scenarios include the following: 

    - Data Breach
    - Data Loss
    - Power outage or loss of other utilities
    - Network Failure
    - Natural Disasters (e.g., fire, flooding, tornado, hurricane, or earthquake)
    - Civil unrest or terrorism
    - Pandemics

    > The plan should test the most likely scenarios first and can be tested in a number of ways

    # Disaster Recovery Tests

    ## Tabletop Testing
    
    Members of the disaster recovery team gather in a large conference room and role-play a disaster scenario

    Usually, the exact scenario is known only to the test moderator, who presents the details to the team at the meeting. 

    The team members refer to the document and discuss the appropriate responses to that particular type of disaster. (Role play only minimal impact on productivity)

    ## Dry Run

    In this test some of the response measures are tested (on non-critical functions)

    ## Full Test

    Involves actually shutting down operations at the primary site and shifting them to the recovery site. 

    When the entire organization takes part in an unscheduled unannounced practice scenario, or full BC/DR activities. 

    # BC/DR Plan Implementation

    Implementing BCP or DRP processes may necessitate utilizing cloud computing for critical services.

    Customers can take advantage of the cloud's high availability features like:

    - Multiple availablity zones
    - Automatic failover to backup region(s)
    - Direct connection to a CSP

    These choices come with cost that must be considered. 

    > The cost of high availablity in the cloud is generally less than a company trying to achieve high availablity on their own

    > The cost of building Resilliency should be less than the cost of business interruption