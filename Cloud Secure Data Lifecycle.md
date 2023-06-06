# Cloud Secure Data Lifecycle

1. Create
- Can be created by users
    - A user creates a file
- Can be created by systems
    - A system logs access

2. Store
- To ensure data is handled properly, it's important to ensure data is ***classified*** as soon as possible.
- Ideally, data is encrypted at rest

3. Use
- Data should be ***protected*** by adequate security controls based on it's classification.

4. Share
- Refers to anytime data is in use or in transit over a network
- Should be Secured and preferrably encrypted

5. Archive
- Archival is sometimes needed to ***comply*** with laws or regulations requiring the retention of data.

6. Destroy
- When data is no longer needed it should be destroyed in such a way that it is ***not readable nor recoverable***.
    - Crypto Shredding


![Secure Data Lifecycle](https://www.researchgate.net/profile/Abdulkadir-Ibrahim-3/publication/317820477/figure/fig3/AS:508256658833408@1498189238065/The-data-security-lifecycle-phases.png)


# Data States

## In Transit

- Data on the wire, in flight
    - Commonly protected with TLS or tunneled through a VPN

## At Rest

- In storage(on disk, in database, etc.)
    - Protected through encryption

## In Use

- In Memory (RAM, CPU, cache, etc.)
    - Should be flushed from memory when transaction is complete or system is powered down (sensitive data should always be encrypted in memory)

# Protecting Data at Rest

- ***Storage Service Encryption*** - CSP storage providers usually protect data at rest by automatically encrypting before persisting it to managed disks, object, file, or queue storage. 

- ***Full Disk Encryption*** - helps you encrypt Windows and Linux IaaS VMs disks using Bitlocker(Windows) and dm-crypt feature of Linux to encrypt OS and data disks

- ***Transparent Data Encryptions (TDE)*** -  Helps protect SQL databases and data warehouses against threat of malicious activity with real-time encryption and decryption of database, backups, and transaction log files at rest **without** requiring app changes.

> Some database platforms also provide row-level encryption, column-level encryption, or data masking

# Data Roles

## Data Owner

Holds the legal rights and complete control over a single piece of data.

Usually a member of ***senior managment***. Can delegate some day-to-day duties.(**CANNOT** delegate total responsibility!)

## Data Custodian

Responsible for safe custody, transport, and storage of data, and implementation of business rules, technical controls. (CIA, Audit Trails, etc.)

# Other Data Roles

## Data Subject

Rers to any individual person who can identivied, directly or indirectly, via an identifier

Identifiers may include anem, and ID number, location data, or via factors specific to the person's physical, physiological, genetic, mental, economic, cultural, or social identity.

## Data Steward

Ensure the data's context and meaning are understood, and business rules governing the data's usage are in place.

Use that knowledge to ensure the data they are responsible for is used as intended. 