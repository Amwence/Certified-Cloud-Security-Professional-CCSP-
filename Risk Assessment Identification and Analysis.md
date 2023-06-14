# Risk Assessment, Identification, and Analysis

The **risk management process** is fundamental to information security, since the entire practice involves **mitigating and managing risks** to data and information systems.

Careful selection of CSPs and the development of SLAs and other contractual agreements are critical to mitigating risk

Organizations can balance cost savings with risk by building a system on top of IaaS or PaaS, rather than utilizing a SaaS solution. 

***NOTE: IaaS means more control, more responsibilities, and more risks***

> Customers must be proactive in addressing their repsonsibilities under the shared responsibility model, as well as making sure their CSP does the same.

## Step 1: Risk Assessment - Identification

Identifying risks is the first step in managing them and begins with identification of the organization's valuable assets

Once assets are identified, security practitioners and risk managers, can then begin to identify potential causes of disruption to those assets.

Risk Managment Frameworks:

Several exist that provide processes and procedures for designing and implementing a risk management framework.

- [ISO/IEC 31000:2018](https://bambangkesit.files.wordpress.com/2015/12/iso-31000_principles-guidelines-risk-manajemen.pdf), Risk Managment Guidelines
- [NIST SP 800-37](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-37r2.pdf), Guide for applying the Risk Management Framework to Federal Information Systems. 

***Quantitaive Risk Assessment*** Assigns a dollar value to evaluate effectiveness of countermeasures (objective, ensure controls are cost effective)

## Step 2: Risk Assessment - Analysis

Analyzing identified risks continues the conversation started by "What could go wrong?"

Analysis seeks to answer two primary questions: 

1. What will the impact be if that goes wrong?
    - Single Loss Expectancy (SLE) (expressed as a $ value)
    - SLE = Exposure value (%) X Asset Value ($)
2. How likely is that to happen
    - Annualized Rate of Occurance (ARO) (how likely it is to happen usually expressed as a decimal)
    - ARO = How often / Per year(s)

    > An impact that happens **twice** a **year** has an ARO of **2.0**
    > An impact that happens **once** every **two years** has an ARO of **0.5**
    > An impact that happens **once** every **five years** has an ARO of **0.2**

**Anualized Loss Expectancy (ALE)** The possible yearly cost of all instances of a specific realized threat against a specific asset. SLE X ARO = ALE
```
Example: 

Scenario: It is estimated a tornado may strike a branch office once in every 5 years, causing 30% loss to a 1,000,000 building.

SLE = 30% loss EF X 1,000,000 AV = 300,000
ARO = 1 time / 5 years = 0.2
ALE = 0.2 ARO X 300,000 SLE = 60,000
```

## Analysis of CSP Risks

Analysis of a CSP or cloud solution and the associated risks involves many departments and focus areas:

- Business units
- Vendor Management
- Privacy
- Information security

CSP operations should also be considered but most major CSPs are audited for ISO/IEC 27001, 27017,27018:

- **ISO/IEC 27001** - A framework for **policies and procedures** that include legal, physical, and technical rontrols involved in a n  orginizations information risk managment processes

- **ISO/IEC 27017** - A **security standard developed for cloud service providers** and users to make a safer cloud-based environment and reduce the risk of security problems

- **ISO/IEC 27018** - THe first international standard about the **privacy in cloud computing services**


Risks with cloud solutions are mainly associated with data privacy and information security:

**Authentication Risk** Does the CSP provide a solution or is this a customer responsibility?(Customer-managed or CSP-managed?)

**Data Security** How a vendor encrypts data at rest, strength of the cryptography, and access controls that prevent unauthorized access by cloud service personnel or other tenants. (Some controls may be on by default, and some the customer may have to enable)

**Supply Chain Risk Management (SCRM)** Evaluation of vendor security policies and processes. 

Most CSPs do not allow direct auditing of their operations, due to the number of customers they support.  

Instead, they provide standardized reports and assurance material regarding their security practices, such as 

- SOC 2 report
- ISO 27001 certification
- Specialized reports for regulated data

# Common Cloud Risks

One risk that has been discussed is the organization losing ownership and full control over system hardware assets.

Careful selection of CSPs and the development of SLAs and other contractual agreements are critical to limiting risk

Organizations can balance cost savings with risk by building a system on top of IaaS or PaaS, rather than utilizing a SaaS solution.(Remember: ther service model affects the level of control)

> Regardless of which deployment or service model is used, some risks are common to all cloud computing environments. 

## Geographic Dispersion of the CSP data centers

If the cloud service provider is properly architected, a disruption at one data center should not cause a complete outagae (Customers must verify the resilience and continuity controls in place at the CSP)

## Downtime
Resilience for network disruptions can be built in multiple ways, such as mutlivendor connectivity, zones and regions.

## Compliance
Privacy data in some jurisdictions cannot be transferred to other countries, so data dispersion is inappropriate.(Major CSPs have compliance-focused service offerings)

## General Technology Risk

Cloud systems are not immune to standard security issues like cyberattacks. (CSP defenses should be documented and tested, and customers aware of their configuration responsibilities)

# Risk Types

## External

Different threat actors, ranging from competitors and script kiddies to criminal syndicates and state actors. 

Capabilities depend on tools, experience, and funding.

Other external environmental threats, such as fire and floods, and man-made threats, such as the accidental deletion of data or users.

## Internal

A malicious insider, a threat actor who may be a dissatisfied employee (someone overlooked for a promotion).

Another internal threat is human error, which is when data is accidentally deleted. 

> CSPs also face these risks. Customers should verify their CSP has addressed them or provided tools to help customers address it. (Customer should know who is responsible for configuration)

# Cloud Specific Risks

The cloud security alliance details the top cloud-specific security threats in their list titled "THE CSA EGREGIOUS 11"

1. Data breaches
    - Loss of sensitive data (PII, PHI, IP intellectual property) due to a security breach
    - Unintentional loss/oversharing is a "data leak"

2. Misconfiguration and inadequate change control
    - Software can offer the most secure configuration options, but if it is not properly set up, then the resulting system will have security issues
    - Remediate this risk through change and configuration management

3. Lack of cloud security architecture and strategy
    - As organizations migrate to the cloud, some overlook security, or fail to consider their obligations in the shared responsibility model

4. Insufficient identity, credential access and key management
    - The public cloud offers benefits over legacy on-premises environments but can also bring additional complexities.
    - Well architected identity and access management (IAM), encryption, secret and key managment are different than on-prem and essential

5. Account hijacking
    - Credential theft, abuse, and/or elevation to carry out an attack. 
    - Phishing is the most common approach

6. Insider threat
    - Disgruntled employees, employee mistakes, and unintentional oversharing
    - Job rotation, privileged access management, auditing, security training

7. Insecure interfaces and APIs
    - Customers failing to secure access to systems gated by APIs, web consoles, etc.
    - Controls include MFA, RBAC, and key-based API access

8. Weak control plane
    - Weakness in the elements of a cloud system that enable cloud environment configuration and management (Web console, CLS, and APIs)
    - Most CSPs offer reference architectures to ensure customers secure and isolate their dev/test/prod environments and data

9. "Metastructure" and "Applistructure" failures
    - Vulnerabilites in the operational capabilities that CSPs make available, like APIs for accessing various cloud services
    - If the CSP has inadequately secured these interfaces, any resulting solutions built on top of thos services will inherit these weaknesses
    - **Metastructure** - the protocols and mechanisms that provide the interface betweenn the cloud layers, enabling managment and configuration.
    - **Applistructure** - Applications deployed in the cloud and the underlying application services used to build them. (e.g. PaaS feature like message queues, functions, and message services)
    - Mitigating risks in this area is the responsibility of the CSP. Customer should verify the CSP has implmented thier own SSDLC to ensure service security

10. Limited cloud usage visibility
    - Refers to when organizations experience significant reduction in visibility over their information technology stack
    - This is because in some models the CSP own the stack!

11. Abuse and nefarious use of cloud services 
    - While the low cost and high scale of compute in the cloud is an advantage to enterprises, it is an opportunity for attackers to execute disruptive attacks at scale. 
    - Makes executing DDoS and phishing attacks easier, so CSPs must implement mitigating security controls for these risks