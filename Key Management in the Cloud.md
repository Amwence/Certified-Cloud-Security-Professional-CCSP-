# Key Management Systems (KMS)

CSPs offer a cloud service for ***centralized secure storage*** and access for ***application secrets*** called a vault.

***(E.G. Azure Key Vault, AWS KMS, GCP Cloud KMS Vault)***

A secret is **anything** that you want to control access to, such as ***API keys, Passwords, Certificates, Tokens, or Cryptographic Keys***.

Service will typically offer ***Programatic Access*** via API to support DevOps and continuous integration/continuous deployment (CI/CD)

Access Control at vault instance-level and to secrets stored within.

***NOTE: Secrets and keys can generally be protected either by software or by FIPS 140-2 level 2 validated HSMs***