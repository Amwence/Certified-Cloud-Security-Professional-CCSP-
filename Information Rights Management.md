# Information Rights Management (IRM)

IRM programs enforce data rights, provisioning access, and implementing access control models

Often implemented to control access to data designed to be shared but not freely distributed.

Can be used to block specific actions, like print, copy/paste, download, and sharing. 

Provide file expiration so that documents can no longer be viewed after a specified time

(Always includes a cloud service, but may include a local agent)

> may popular SaaS file sharing platforms implement these concepts as sharing options, which allow the document owner to specify which users can view, edit, download, and share

# Objective of Information Rights Management

- **Persistence** - Access control/ability to enforce restrictions must follow the data (Protection must follow the document or data wherever it travels)

- **Dynamic Policy Control** - IRM solution must provide a way to update the restrictions even after a document has been shared

- **Expiration** - IRM tools can enforce time-limited access to data as a form of access control. (Ability to expire/revoke access, require user check-in)

- **Continuous Audit Trail** - IRM solution must ensure that protected documents generate an audit trail when users interact with protected documents (Required for accountability and non-repudiation)

- **Interoperability** - IRM solutions must offer support for users across these different system types. (Support for different OS, device types, and apps is important)

# Appropriate Tools

IRM tools comprise a variety of components necessary to provide policy enforcement and other attributes of the enforcement capability

**Centralized Service** - for identity proofing and certificate issuance, store of revoked certificates, and for unauthorized identity information access. (Enables enforcement from anywhere)

**Secretes Storage** - IRM solutions require local storage of encryption keys, tokens, or digital certificates used to validate users and access authorizations.

Local storage requires protection primarily for data integrity to prevent tampering with the material used to enforce IRM

> Must prevent local modifications of access controls and credentials. Otherwise, a user might modify the permissions granted to extend the access beyond what the data owner originally specified. 

***NOTE: Local changes must never supersede controls implemented by the cloud service!***