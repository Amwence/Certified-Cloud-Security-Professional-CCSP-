# Data Archiving Procedures and Mechanisms

## Data Archiving

Refers to placing data in long-term storage for a variety of purposes. (The optimal approach in the cloud differs in several respects from on-premises equivalent)

Key elements of data archiving in the cloud

- Data Encryption
- Data Monitoring
- eDiscovery and Retrieval
- Backup and DR Options (disaster recovery)
- Data Format
- Media Type

## Data Encryption

Encryption policy should consider which media is used, and data search and restoration needs, and regulatory obligations. 

What threats should be mitigated by the encryption?

How will encryption keys be managed? Long-term archiving with encryption can present key management challenges.
(Access Controls and encryption are important to protect data integrity by preventing unauthorized access)

## Data Monitoring

Data stored in the cloud tends to be replicated as part of storage resiliency or BC/DR (Business continuity/Disaster Recovery)

To maintain data governance, it is required that all data access and movements be tracked and logged. 

Monitoring to ensure all security controls are being applied properly throughout the data lifecycle

(Accountability, traceability, auditability should be maintained at all times)

## eDiscovery and Retrieval

Archive data may be subject to retrieval according to certain parameters such as dates, subjects, and authors. 

The archiving platform should provide the ability to perform eDiscovery on the data to determine which data should be retrieved.

> Data that is subject to more frequent search should be kept in a service that enables eDiscovery with manageable level of effort (Ensure staff can manage the eDiscovery support burden)

## Backup and Disaster Recovery Options

All requirements for data backups and resotre should be specified and clearly documented

Business Continuity and Disaster Recovery (BCDR) plans are updated and aligned with whatever procedures are implemented.

(Both resiliency to disaster, ensuring archive data availabliity, and knowledge of control of data replication are important)

## Data Format and Media Type

This is an important consideration because it may be kept for an extended period.

Format needs to be ***secure, accessible and affordable.***

Media type should support the other data archiving requirements, but physical media concerns fall to the CSP

>AWS S3 and Azure Storage both offer cool tier (infrequent access) storage for low-cost archiving and immutability to ensure integrity
***NOTE: Often cloud storage is billed by the Gigabyte, so cost is a factor! However, it needs to be balanced with access needs