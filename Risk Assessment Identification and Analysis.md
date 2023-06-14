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

**Authentication Risk** Does the CSP provide a solution or is this a customer responsibility?

