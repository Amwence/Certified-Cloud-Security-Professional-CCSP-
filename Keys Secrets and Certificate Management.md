# Keys Secrets and Certificate Management

## Keys

Are most often used for encryption operations and can be used to uniquely identify a user or system

Keys should be stored in a tool that implements encryption and requires a strong passphrase or MFA to access.

> In the cloud, typically consists of a key vault

## Secrets

Often a secondary authentication mechanism used to verify that a communication has not been hijacked or intercepted.

## Certificates 

Are used to verify the identity of a communication party and also for asymmetric encryption by providing a trusted public key. 

# Key Management Services (KMS)

CSPS offer a cloud service for centralized secure storage and access for application secrets called a vault (e.g. Azure Key Vault, AWS KMS, GCP cloud KMS Vault)

A secret is anything that you want to control access to, such as ***API keys, passwords, certificates, tokens, or Cryptographic keys.*** 

Service will typically offer programatic access via API to support DevOps and continuous integration/continuous deployment (CI/CD)

Access Control at vault instance-level and to secrets stored within. 

> Secrets and Keys can generally be protected either by software or by FIPS 140-2 Level 2 validated HSMs