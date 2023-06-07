# Threats to Storage Types

There are universal threats to data at rest (in storage) regardless of the location, on-premises or in the cloud

## Universal threats from the perspective of the CIA Triad:

- ***Unauthorized Access*** - threatens Confidentiality

- ***Improper Modification*** - Threatens Integrity

- ***Loss of Connectivity*** - Threatens Availability

## Other Threats

- Jurisdictional issues
- Denail of Service - Availability
- Data Corruption/Destruction - Integrity
- Theft or media loss
- Malware and Ransomware
- Improper Disposal

> All of these can happen in the cloud, it is largely a question of "who is responsible?"

## Unauthorized Access

User accessing data storage without proper authorization presents security concerns

Customer must implement proper access control, CSP must provide adequate logical separation

## Unauthorized Provisioning

Primariy a cost and operational concern

Ease of use can lead to unofficial use, unapproved deployment, and unexpected costs (Shado IT)

## Loss of Connectivity

Loss of connectivity for any reason, whether network connectivity, access controls, authentication services, etc.

## Jurisdictional Issues

Data between countries can run afoul of legal requirements

Privacy legislation bars data transfers to countries without adequate privacy protections (customer bears some responsibility)(GDPR)

## Denail of Service

In the event a network connection is severed between the user and the CSP. CSPs are better prepared to defend against DDoS attacks.

## Data Corruption or Destruction

Human error in data entry, malicious insiders, hardware and software failures, natural disasters rendering data or storage media unusuable. 

>***Defenses:*** least privilege, RBAC (Role Based Access Control), offsite data backups

## Theft or Media Loss

In the cloud, CSPs retain responsibility for preventing the loss of physical media through appropriate physical security controls

## Malware and Ransomware

Ransomware not only encrypts data stored on local drives but also seeks common cloud storage locations like SaaS apps. (Responsibility will vary by cloud category)

## Improper Disposal

Ensuring that hardware that has reached the end of its life is properly disposed of in such a way that data cannot be recovered. (CSP responsible for hardware disposal)

# Regulatory Compliance

Certain cloud service offerings may not meet all the organizations compliance requirements, which leads to two main security concerns. (Customer bears responsibility verifiying that CSP meets regulatory complaince terms for the business)

## Consequences of NonCompliance

Could be fines or suspension of business operations. (e.g. GDPR,SOX,PCI DSS)

## Data Protection

requirements may include specific encryption standards, handling, retention. (HIPAA/PCI DSS requires specific data retention and data handling)