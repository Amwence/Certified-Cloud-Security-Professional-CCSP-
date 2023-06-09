# Data and Media Sanitization

## Less Secure Data Destruction

- **Erasing** - Performing a delete operation against a file, files, or media.

- **Clearing (overwriting)** - Preparing media for reuse and ensuring data cannot be recovered using traditional recovery tools. (May use random data or zeroes, one or multiple passes)

- **Purging** - a more intense form of clearing that prepares media for reuse in less secure environments.

> Media is reusable with any of these methods
> Data may be recoverable with fornesic tools

## More Secure Data Destruction

**Crypto-Shredding** (cryptographic erasure) 

1. Data is encrypted with a strong encryption engine. 
2. The keys used to encrypt the data are then encyrpted using a different encryption engine. 
3. Then, keys form the second round of encryption are destroyed.

    - Pro: Data cannot be recovered from any remnants. 
    - Con: High CPU and performance overhead

    ***NOTE: If the exam poses a question on "Secure Data Destruction" this is almost certainly the answer!***

# Destroying Media Data

> Destorying data on Media such as hard drive or DVD/CD Rom

- **Degaussing** - creates a strong magnetic field that erases data on some media and destroys electronics.

- **Shredding** - You can shred a metal hard drive into powder.

- **Pulverizing** - Use a hammer and smash drive into pieces, or drill through all the platters.

***NOTE: **Media is not reusable** with any of these methods and **Data is not Recoverable** by any means***