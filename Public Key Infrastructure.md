# Public Key Infrastructure

## Key Management

Management of cryptographic keys in a cryptosystem.

Operational considerations include dealing with the generation, exchange, storage, use, crypto-shredding (destruction) and replacement of keys. 

Design considerations include cryptographical protocol design, key servers, user procedures, and other relevant protocols. 

## Certificate Authority (CA)

Certification Authorities create digital certificates and own the policies.

PKI hierarchy can incldue a single CA that serves as root and issuing, but this is not recommended 

> In a single-layer PKI hierarchy, if the server is breached no certificate, including the root, can be trusted!

# Types of Certificates

## User Certificate

Used to represent a user's digital identity.

## Root Certificate

A trust anchor in a PKI environment is the root certificate from which the whole chain of trust is derived (This is the Root CA)

## Domain Validation Certificate

A Domain-Validated (DV) certificate is an X.509 certificate that proves the onwership of a domain name

## Extended Validation

Extended validation certificates provide a higher level of trust in identifying the entity that is using the certificate (Commonly used in the financial services sector)

Hierarchy:

1. Root CA
2. Subordinate CA
3. Issuing CA

(Moving up the chain starting at issuing up to Root)