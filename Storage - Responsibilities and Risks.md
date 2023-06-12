# Storage - Responsibility and Risks

Cloud storage has a number of potential security issues. Data spends most of its life at rest, so understand who is responsible for securing cloud storage is key. 

## CSP Responsibilities

**Physical protection** of data centers and the storage infrastructure they contain. 

**Security patches and maintenance**  of underlying data storage technologies and other data services they provide. 

## Customer Responsibilities

**Proper configuration** and usage of the storage tools.

**Logical security and privacy** of data they store in the CSPs environment. 

CSPs provide a set of controls and configuration options customers can use to secure use of their storage platforms. 

Customer is responsible for: 

- Accessing the adequacy of these controls and properly configuring and using the controls available. (Access over public internet, VPN, or internal networks. e.g. Force TLS, Block public internet access, etc.)

- Ensuring adquate protection for the data at rest and in motion based on the capabilities offered by the CSP. (Feature configuration, Key managmenent(if customer managed). e.g. bitlocker/drive encryption, SFTP for file transfers, etc.)

- Configuring secure access, whether private or public. (Identity access control and Access managment. e.g. who has access to what files, can they be changed, and some form of auditing)

> In the cloud, the customer loses some control of the physical medium  where data is stored but retains responsibility for data security, and privacy. 