# Identification Authentication and Authorization

## AuthN and AuthZ

**Authentication (AuthN)** is the process of proving that you are who you say you are (IDENTITY)

**Authorization (AuthZ)** is the act of granting an authenticated party permission to do something. (ACCESS)

***Permissions, rights, and privileges*** are granted to users based on their proven identity.

If user has assigned rights to a resource, they are granted ***authorization*** (User's should be granted minimum necessary permissions also known as the principle of least privilege)

## Accountability

Users who perform activities on a system are held accountable for following policies and procedures

**Accountability** is typically enforced with adequate logging and monitoring of system activity

**Cloud challenges in enforcing accountability:**

- SaaS apps used as users travel make identifying anomalous/malicious behavior more difficult

- Bad password practices (reuse across services)

- Use of personal devices in BYOD scenarios

(Modern IDaaS (Identity as a service) tools provide solutions of these challenges.)

## MFA Factors and Attributes

MFA consists of 

- Something you **know** (pin or password)
- Something you **have** (trusted device)
- Something you **are** (biometric)

MFA can consist of Authenticator App(Software OATH), Voice Call, SMS (text message) OATH HW Token (Time-based one time password (TOTP))

### Multifactor Authentication

- includes two or more authentication factors

- more secure than using a single authentication factor

- ***Passwords*** are the weakest form of authentication

- **Password Policies** help increase their security by enforcing complexity and history requirements

- **Smartcards** include microprocessors and cryptographic certificates (Yubikey)

- **Oath tokens** create one-time passwords (OTP)

- **Biometric** methodes identify users based on individual characteristics such as fingerprints and facial recognition

## Conditional Authentication Policies

Looks at signals sent from device trying to authenticate, and makes decisions based on that, such as is it a trusted device signing in from a trusted location, or user behavioral analysis.

# Authentication Methods

## Authentication Applications

Is a software based authentication that implements tow step verification services using the Time based one time password algorithm and HMAC based one time password alogorithm, for authenticating users of software applications. (E.g. Microsoft authenticator and google authenticator)

> Authenticator apps from comapnies like Microsoft and Google generate one-time passcodes using open standards developed by the **Initiative for Open Authentication (OATH).** You'll hear HMAC and TOTP tokens called OATH tokens with some of these providers. 

## Push Notifications

Where the server is pushing down the authentication information to yoru mobile device.

Uses the mobile deviec app to be able to receive the pushed message and display the authentication information.

## Federation

Federation is a collection of domains that have established trust.

The level of trust may vary , but typically includes authentciation and almost always authorization.

Often includes a number of organizations that have established trust for shared access to a set of resources.

Example:

You can federate your on-premises environment with Azure Active Directory (Azure AD) and use this federation for authentication and authorization.

This sign-in method ensures that all users authentication occurs on-premises.

Allows administrators to implement more rigorous levels of access control. (Certificate authentication, key fob, card token)

# Audit Mechanisms

## Log Collection

- Cloud services will offer different controls over what information is logged

- but at a minimum security level of security-relevant events, such as use of or changes to privileged accounts.

- A log aggregator can ingest logs from all on-premises and cloud resources for review.

> ***NIST SP 800-53*** and ***OWASP logging cheat sheet*** offer guidance on specific information to capture in audit records

## Correlation

Refers to the ability to discover relationships between two or more events across logs. (This capability is commonly associated with a SIEM, which correlates events in logs from many sources)

## Packet Capture and Relay

Packet capture tools are also called **Protocol Analyzers**

The cloud enviornment may not provide any facility for capturing packets, particularly in SaaS scenarios

**Wireshare**: a free, open-source protocol analyzer, with CLI and GUI versions, availbable for Windows and Linux.

Some CSPs support wireshark, others have specialized services to perform packet capture on virtual networks. (e.g. Network Watcher(Azure), AWS supports WireShark)

Some CSP protocol analyzers can save the data that they collect to a Wireshark-compatible packet capture file (PCAP)