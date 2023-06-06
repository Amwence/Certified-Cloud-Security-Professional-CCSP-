# Common Threats

## Data Breach

When sensitive data is stolen, incuding Personally Identifiable Information(PII), and Protected Health Information (PHI).

Often due to poor application or database security design or configuration, whereby data is exposed without proper authorization. (Often the result of a cyber attack)

> Preventable by following secure development practices and adhering to recommendations in the ***Secure Data Lifecyle***

## Data Loss

When sensitive data is ***unknowingly exposed to the public***. Often through a system misconfiguration or oversharing. (Sometimes called a data leak)

# Insecure Interfaces and APIs

## APIs (SOAP or REST)

Is a set of exposed interfaces that allow programatic interaction between services. 

An avenue for security breach if not properly implemented. 

REST uses the ***HTTPS*** Protocol for web communications to offer API endpoints. (Makes it a target for DDOS attacks)

***Security mechanisms*** include API gateway, authentication, IP filtering, throttling, quotas, data validation

> Also ensure that storage, distribution, and transmission of ***access keys*** is performed in a secure fashion

## Malicious Insiders

Disgruntled employees can wreak havoc on a system. 

Internal acts of disruption include ***theft*** and ***Sabotage***.

## Traffic Hijacking

When attacks are designed to steal or wedge themselves into the middle of a conversation in order to gain control. (MITM Man-In-The-Middle)

## Abuse of Cloud Services

Consumers sometimes misuse their cloud services for illegal or immoral activities.

## Insufficeint due diligence

Process/effort to collect and analyze information before making a decision or conducting a transaction

Failure to perform due diligence can result in a due care violation (Knowing the difference and due care is important for your career)

# Due Diligence VS. Due Care

## Due Diligance 

- Process/effort to collect and analyze information before making a decision or conducting a transaction.

Example: 
- Decision
    - Research
    - Planning
    - Evaluation
    - Often comes before a decision
    
    > Increases understanding and reduces risk
    > think before you act
    > Do Detect
    
- Knowledge and research of: 
    - Laws and regulations
    - Industry standards
    - Best practices


## Due Care

- Doing what a reasonable person would do in a given situation. It is sometimes called the "Prudent person rule". 

Example:
- Decision
    - Implementation
    - Operation (upkeep)
    - Reasonable measures
    - Often comes after the decision is made
    
    > Prudent person rule that implementing reasonable measures
    > Actions speak louder than words
    > Do Correct

- Delivery or Execution including:
    - Reporting security incidents
    - Security Awareness training
    - Disabling access in a timely way

> Together will reduce senior management's ***culpability & (downstream) laibility*** when a loss occurs. 


## Shared Technology Vulnerabilites

The underlying infrastructure of the public cloud was not originally designed for the types of multitenancy in the public cloud

Modern Virtualizatino software bridges most of the gaps

- What Threats Reamin in a shared public cloud infrastructure?
    - Cloud infrastructure can still be vulnerable to insider threats
    - Unintentional misconfigurations are a concern
    - To a lesser degree, disruptive attacks of scale (DoS, DDoS) and "noisy neighbors"

    > For regulatory compliance and high-criticality scenarios, CSPs have some higher isolation and flexible scale-out options.