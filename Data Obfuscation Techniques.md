# Data Obfuscation Techniques

Reducing GDPR Exposure or steps to help reduce or eliminate GDPR requirements

## Anonymization

The process of removing all relevant data so that it is impossible to identify original subject or person. 

If done effectively, then GDPR is no longer relevant for the anonymized ata. (Good only if you don't need the data)

> Anonymization is sometimes called de-identification

## Pseudonymization

De-Identifion procdure using pseudonyms(aliases) to represent other data.

Can result in less stringent requirements than would otherwise apply under GDPR. 
(Use if you need the data and want to reduce exposure)

# Hashing VS. Encryption
## Encryption
Encryption is a two-way function; what is encrypted can be decrypted with the proper key. 
## Hashing 
A one way function that scrambles plain text to produce a unique message digest. 

Conversion of a string of characters into a hsorter fixed-lenghth value

Common Uses

- Verification of digital signatures
- Generation of qsuedo-random numbers
- Integrity services

## Hashing Function Requirements

1. They must allow input of any length
2. provide fixed-length output
3. Make it relatively easy to compute the has function for any input
4. Provide one-way functionality
5. Must be collision free

## Data Masking

When only partial data is left in a data field. for example a credit card may be shown as **** **** **** 1234. 

(Commonly impleneted in databases, but can be implemented in code as well)

## Tokenization

Where meaningful data is replaced with a token that is generated randomly, and the original data is held in a vault. 

>Stateless, stronger than encryption, keys are not local

> Tokenization goes further than pseudonymization, replacing your pseudonym with an unrecognizable token