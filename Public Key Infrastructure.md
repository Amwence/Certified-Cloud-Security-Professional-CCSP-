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
    - Usually maintained in an offline state
    - Issues certs to new subordinate CAs

2. Subordinate CA
    - Also called a Policy CA or Intermediate CA
    - Issues certs to new issuing CAs
    - Regularly issue certificates, making it difficult for them to stay offline as often as root CAs
    - Do have the ability to revoke certificates, making it easier to recover from any security breach that does happen
    - if the issuing CA is breached, its certificate can be revoked and a new one issued

    > A single compromise CA does not result in compromise of the root. 


3. Issuing CA
    - Certificates for clients, servers, devices, websites, etc. Issued from here.

(Moving up the chain starting at issuing up to Root is called Chain of Trust)

## Certificate Revocation List (CRL)

Contains information about any certificates that have been revoked by a subordinate CA due to companies to the certificate or PKI hierarchy

CAs are required to publish CRLs, but it's up to the certificate consumers if they check these lists and how they respond if a certificate has been revoked. 

# Certificate Revocation

Revoking (invalidating) a certificate before expiration:

Certificate is effectively cancelled, and certificate serial number added to the certificate revocation list (CRL) mentioned above. 

But, parties checking the certificate to verify identity or authenticity must check with issuing authority on validity

Two potential options for tracking revocations: ask for the CRL or if available, OSCP endpoint/service
(Endpoint to query for CRL or OCSP is on the certificate)

>If the other client/server does not check the CRL or OCSP for certificate validity, they may accept an invald certificate as valid

## Online Certificate Status Protocol (OCSP)

Offers a faster way to check a certificate's status compared to downloading a CRL

With OCSP, the consumer of a certificate can submit a request to the OCSP endpoint to obtain the status of a specific certificate

## Certificate Signing Request (CSR)

Records identifying information for a person or device that owns a private key as well as information on the corresponding public key. 
(It is the message that's sent to the CA in order to get a digital certificate created)

## CN (Common Name)

The Fully Qualified Domain Name (FQDN) of the entity (e.g. Web Server)
