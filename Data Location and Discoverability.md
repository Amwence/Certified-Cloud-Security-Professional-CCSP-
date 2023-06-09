# Data Location and Discoverability

The location of data will impact both it's discoverability and the choice of tools used to perform discovery. 

## Impact on tools and discoverability

Tools must be able to access data to perform the scanning and analysis needed in the discovery process. (May require different tools for cloud and on premises discovery)

Not all cloud solutions may offer a local agent for on-premises

Network-based DLP may not analyze all traffic between on-premises endpoints and cloud. 

> An optimal DLP approach will discover data in **on-premises** and **in cloud** repositories, as well as **in transit**.

Tools must be able to scan unstructured data within structured datasources, such as relational databases.
(EXAMPLE: Problem description inside a helpdesk ticket stored in a SQL database) 

***Both unstructured and structured in the same repository will increase tool cost and complexity and may present classification challenges***

> If a single data classification label has to be placed on a large data source the most sensitive classification found will apply!

# Data Discovery

Ensures that data is appropriately classified for protection

## Metadata-Based Discovery

A list of traits and characteristics about specific data elements or sets
Often automatically created at the same time as the data

## Label-Based Discovery

Based on examining labels created by the data owners during the **Create** phase. (or in bulk with a scanning tool)

Can be used with databases (structured data) but is more commonly used with file data.