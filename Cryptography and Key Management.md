# Cryptography and Key management

## Trusted Platform Module (TPM)

A ***chip*** that resides on the motherboard of the device.

Multipurpose, like storage and management of keys used for full disk encryption (FDE) solutions (e.g. Bitlocker)

Provides the operating system with ***Access to keys***, but prevents drive removal and data access

## Hardware Security Module (HSM)

A ***Physical computing device*** that safeguards and ***manages digital keys***, performs encryption and decryption functions for digital signatures, strong authentication, and other cryptographic functions.

***Note: Like a TPM, but are often removable or external devices***

# Key management Strategy

1. Generation
    - Encryption keys should be generated with a trusted, secure cryptographic module
    - FIPS 140-2 validated modules provide tamper resistance and key integrity

2. Distribution
    - Encryption keys should be ***distributed securely*** to prevent theft/compromise during transit
    - ***BEST PRACTICE: Encrypt keys with a separate encryption key while distributing to other parties***

3. Storage
    - Encryption keys must be ***protected at rest*** and should never be stored in plaintext
    - This includes keys in volatile and persistent memory

4. Use
    - Clients (users + trusted devices) will use keys for resources asaccess controls allow
    - Acceptable use policy sets guardrails for data usage

5. Revocation
    - A process for revoking access at separation, policy breach, device or key compromise
    - ***EXAMPLE: In PKI, you would revoke the certificate of the issuing Certificate Authority (CA)***

6. Destruction
    - ***Key Destruction*** is the removal of an encryption key from its operational location.
    - ***EXAMPLE: MDM systems remove certificates from a device during device wipe or retirement (MS Intune, Airwatch)***
# Other Key management terms and concepts

## Level of protection

Encryption keys must be ***secured at the same level*** of control or higher ***as the data*** they protect.

Sensitivity of the data dictates this level of protection, as defined in the organization's data security policies

## Key Recovery

Circumstances where you need to **recover a key for a particular users**, ***without that user's cooperation***, such as in termination or key loss. 

## Key Escrow

Copies of ***keys held by a trusted third party*** in a secure environment, which can aid in many of the other areas of key managment.