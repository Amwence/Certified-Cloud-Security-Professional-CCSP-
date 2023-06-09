# Maintaining Accountability

## Accountability

Is maintained for individual subjects using auditing.

Logs record user activities and users can be held accountable for their logged actions. 

Directly promotes good user behavior and compliance with the organizations security policy. 

## Security Audits and Reviews

Helps ensure that management programs are effective and being followed.

Commonly associated with account management practices to prevent violations with least privilege or need-to-know principles.

Can also be performed to oversee many programs and processes

For example to maintain: Patch management, vulnerability management, change management, and configuration management. 

# Event sources and Event Attributes

**Auditability, Traceability, and Accountability** of data events

OWASP provides a comprehensive set of definitions and guidelines for identifying, labeling, and collecting data events

Ensure events are useful and pertinent to applications and security, whether in a cloud or traditional data center. 


## Definition of Event Sources

Which events are important and available for capture will vary based on cloud service model employed (IaaS, PaaS, or SaaS)

## IaaS Event Sources (Level of Log Access: HIGH)

Within an IaaS environment, the cloud customer has the most access and visibility into the system and infrastucture logs of any cloud service model.

Because the cloud customer has nearly full control over their compute environment, including system and network capabilities, virtually all logs and data events should be exposed and available for capture. 

***NOTE: This is because the customer has more responsibility than in any other cloud model (See Shared Resonsibility Model image in [Cloud Service Models](Cloud%20Service%20Models.md))***

## PaaS Event Sources (Level of Log Access: Medium)

A PaaS environment does not offer or expose the same level of customer access to infrastructure and system logs as IaaS.

However, the same level of detail of logs and events is available at the application level..

***NOTE: Responsibility for system and infrastructure in PaaS belongs to the cloud service provider(CSP)***

## SaaS Event Sources (Level of Log Access: Low)

Because in a SaaS environment the cloud service provider is responsible for the entire infrastructure and application, the amount of log data available to the cloud customer is less.

Customer responsibility is limited to access control, shared responsibility for data recovery, and feature configuration

***NOTE: In this case service responsibility equates to log visibility***

# The **WHO, WHAT, WHERE, and WHEN** of logging from OWASP

Ultimately, logs should be able to answer the question:

"Who did what and when? (and from where)"

Sufficient user ID attribution should be accessible, or it may be impossible to determine who performed a specific action at a specific time. This is called ***Identity Attirbution***(This is a necessity for non-repudation)

## Who

- Source Address
- User Identity (if known)

## What

- Type of Event
- Severity of Event
- Security-Relevant Event Flag (if log contains non-security events)
- Description

## Where

- Application Identifier (name, version, etc.)
- Application Address
- Service
- Geolocation
- Window/for/page (URL and Http method)
- Code Location (Script or Module name)

## When

- Log Date and Time (Internation Format)
- Event Data and Time
- Interaction Identifier

> OWASP maintains concentrated guidance for developers on building application logging mechanisms, especially related to security logging in the [OWASP Logging Cheat Sheets](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html) and Also [OWASP Logging Cheat Sheets Github](https://github.com/OWASP/CheatSheetSeries/tree/master)

***NOTE: LOGS ARE WORTHLESS IF DO NOTHING WITH THE LOG DATA. THEY ARE MADE VALUABLE ONLY BY REVIEW***

That is, they are valuable only if the organization makes use of them to identify activity that is unauthorized or compromising.

SIEM (Security Information Event Monitoring) tools can help to solve some of these problems by offering these key features:

- Log Centralization and Aggregation
- Data Integrity
- Normalization
- Automated or Coninuous Monitoring
- Alerting
- Investigative Monitoring