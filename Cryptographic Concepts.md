# Cryptographic Concepts

## Digital Signatures

Digital signatures are similar in concept to handwritten signatures on printed documents that identify individuals, but they provide more security benefits. Are an encrypted hash of a message, encrypted with the senders private key in a signed email scenario. 

Provides 3 Key benefits:

1. Authentication - This positively identifies the sender of the email.
    - Ownership of a digital signature secret key is bound to a specific user

2. Non-repudiation - The sender cannot later deny sending the message
     - This is sometimes required with online transactions

3. Integrity - Provides assurances that the message has not been modified or corrupted. 
    - Recipients know that the message was not altered in transit