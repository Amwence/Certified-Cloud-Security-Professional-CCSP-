# Data types

## Structured

Data contained in rows and columns such as an Excel spreadsheet or relation database (Excel, MSSQL, MySQL, PostgreSQL)

Often includes a description of it's format known as a data model or schema, which is an abstract view of the data's format in a system. 

Data structured as elements, rows, or tuples is given context through the schema
 
>Discovery Methods include:
> **MetaData**, or data that describes data, is a critical part of the discovery of structured data
> **Semantics**, or the meaning of data, is described in the schema or data model and explains relationships expressed in data. 

## Unstructured 

Data that cannot be contained in a row-column database and does not have an associated data model.

Discovery occurs through ***content analysis***, which attemtps parse all data in a storage location and identify sensitive information. 

> Content analysis (discovery) methods incldue:
> **Pattern Matching**, which compares data to known formats like credit card numbers. (DLP tools often have pre-defined 'sensitive data types')
>**Lexical Analysis** attempts to find data meaning and context to discover sensitive info that may not conform to a specific pattern. 
> **Hashing** attempts to identify known data by calculating a hash of files and comparing it to a known set of sensitive file hashes. (Only good for data that does not change frequently)

## Semi-Structured

A combination of structured and unstructured data. (JSON,XML,HTML email messages, NoSQL)

Typically, content is unstructured, but may contain metadata to help organize the data. (Fluid but organizable by properties of metadata)

> This is a mix of data types that will require a combination of discovery methonds and tooling capable of discovery in thes comingled data types. 