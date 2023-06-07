# Encryption and Key managment

# Asymmetric vs. Symmetric Encryption

## Symmetric Encryption

Relies on the use of a ***SINGLE shared secret key*** (NOTE SINGLE). Lacks support for scalability, easy key distribution, and non repudiation

- tends to be faster and is often used for bulk data encryption
- Sender encrypt data with a key, and the Recipient decrypts the data with the same key

Types of Symmetric Encryption:

- Twofish, Serpent, AES, Blowfish, RC4, DES, 3Des, Skipjack, Safer, Idea

## Asymmetric Encryption

Relies on ***Public-Private key pairs*** for communication between parties. Supports scalability, easier key distribution, and nonrepudiation

- Scalable - easy to scale to many parties

- Sender encrypts using the recipients public key, signing with their own private key. The recipient then decrypts the data using their own Private key and verifies the signature using the senders public key. (Private keys are unshared and are the only things that can be used to decrypt things encrypted with public key and vice versa)

Types of Asymmetric Encryption: 

- Diffie Helman (Key Exchange Protocol)
- DSS (digital Signature Standard)
- ElGamal
- Eliptic Curve Cryptography
    - Eliptic Curve Digital Signature Algorithm (ECDSA)
    - Eliptic Curve Diffie-Helman (ECDH)

- RSA
- YAK

***NOTE: Think Certificates***

## Trust Model

A model of how different certification authorities trust each other and how their clients will trust certificates from other certification authorities.

The four main types of trust models used in ***public key infrastructure (PKI)*** are bridge, hierachical, hybrid, and mesh. 

# Key Management

## Key Escrow

Addresses the possibility that a cryptographic key may be lost

The concern is usually with symmetric keys or with the private key in asymmetric cryptography. 

If the private key or symmetric key is unable to be recovered, then there is no way to get the key back , and the user cannot decrypt messages. 

Orginizations establish key escrows to enable recovery of lost keys (copy of keys with a third party)

## Encryption Key Lifecycle

1. Generation
    - Encryption keys should be generated within a trusted, secure cryptographic module
    - Should use strong, random keys using cryptographically sound inputs like random numbers (FIPS 140-2 validated modules provide tamper resistance and key integrity)

2. Distribution
    - Encryption keys should be distributed securely to prevent theft/compromise during transit. 
    - Plan for securely transferring symmetric keys and distributing keys to the key escrow agent
    > ***Best practice:*** Encrypt keys with a separate encryption key while distributing to other parties

3. Storage
    - Encryption keys must be protected at rest and should never be stored in plaintext (this includes keys in volatile and persistent memory)
    - Storing keys ina secure manner, whether encrypted in a key vault or on a physical device
    - Also consider handling in the process of storing copies for retrieval if a key is ever lost (key escrow)

4. Use
    - Using keys securely, primarily focused on access controls and accountability

5. Revocation
    - A process for revoking access at separation, policy breach, device or key compromise
    - A process for archiving keys no longer needed for routine use, in case needed for existing data
    > Example: In PKI, you would revoke the certificate on the issuing Certificate Authority (CA)

6. Destruction
    - **Key Destruction** is the removal of an encrypteion key from its operational location
    - **Key Deletion** goes further and removes any info that could be used to reconstruct that key
    > Example: MDM removes certificates from a device during device wipe or retirement

    # Key managmenet in the cloud

    Know the layers and services where you can enable encryption, and your options for key storage and management (CSP managed or Self managed)

    ## Key storage

    Many CSPs offer FIPS compliant virtualized HSMs to securely generate, store, and control access to cryptographic keys.  (Self managed keys typically are not default and may have cost)

    Orginzations that use multiple cloud providers or need to retain physical control over key management may need to implement a ***bring-your-own-key (BYOK)*** strategy. 

    > Generally to let teh CSP manage keys unless you have requirements that mandate your organization mandate keys (regulatory Compliance)

    # Other Cloud Encryption Scenarios

    ## Storage-Level Encryption

    Provides encryption of data as it is written to storage, utilizing keys that are controlled by the CSP. 

    ## Volume level Encrytpion

    Provides encryption of data written to volumes connected to specific VM instances, utilizing keys controlled by the customer. (Bitlocker and DM-Crypt)

    ## Object Level Encryption

    Encryption of objects as they are written to storage, in which case the CSP likely controls the keys and could potentially access the data. 

    ## File-Level Encryption

    Implemented in client apps, such as word processing apps like Microsoft Word or collaboration apps like sharepoint (will vary by CSP platform)

    ## Application-Level Encryption

    Implemented in an application typically using object storage (data entered by user typically encrypted before storage)

    ## Database-Level Encryption

    Transparent data encryption (Database files, logs, backups), column-level or row-level encryption, or data masking
    (transparent data encryption is a method of encrypting data at rest, where the encryption and decryption )

    - Will vary depending on RDBMS (relational database management platform) (MSSQL, MySQL, PostgresSQL)