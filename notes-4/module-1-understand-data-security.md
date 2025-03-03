---
description: Domain D5.0, D5.1.1, D5.1.2, D5.1.3
---

# Module 1: Understand Data Security

**Hardening** is the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems and software, including the operating system, web server, application server and applications, etc. This module introduces configuration management practices that will ensure systems are installed and maintained according to industry and organizational security standards.

### Data Handling

Data itself goes through **its own life cycle as users create**, **use**, **share and modify it**. The data security life cycle model is useful because **it can align easily with the different roles that people and organizations perform during the evolution of data from creation to destruction (or disposal)**. It also helps put the different **data states of in use, at rest and in motion, into context**.

All ideas, data, information or knowledge can be thought of as going through six major sets of activities throughout its lifetime. Conceptually, these involve:

1. Creating the knowledge, which is usually tacit knowledge at this point.
2. Storing or recording it in some fashion (which makes it explicit).
3. Using the knowledge, which may cause the information to be modified, supplemented or partially deleted.
4. Sharing the data with other users, whether as a copy or by moving the data from one location to another.
5. Archiving the data when it is temporarily not needed.
6. Destroying the data when it is no longer needed.

### Data Handling Practices

* **Classification**: classifications dictate **rules and restrictions about how that information can be used**, **stored** or **shared with others**. All of this is done to keep the temporary value and importance of that information from leaking away. Classification of data, which asks the question “Is it secret?” determines the labeling, handling and use of all data. **Classification is the process of recognizing the organizational impacts if the information suffers any security compromises related to its characteristics of confidentiality**, **integrity** and **availability**. **Information is then labeled and handled accordingly**. Classifications are derived from laws, regulations, contract-specified standards or other business expectations. One classification might indicate “minor, may disrupt some processes” while a more extreme one might be “grave, could lead to loss of life or threaten ongoing existence of the organization.” These descriptions should reflect the ways in which the organization has chosen (or been mandated) to characterize and manage risks. The immediate benefit of classification is that it can lead to more efficient design and implementation of security processes, if we can treat the protection needs for all similarly classified information with the same controls strategy.
*   **Labeling**: **security labels are part of implementing controls to protect classified information**. It is reasonable to want a simple way of assigning a level of sensitivity to a data asset, such that the higher the level, the greater the presumed harm to the organization, and thus the greater security protection the data asset requires. This spectrum of needs is useful, but it should not be taken to mean that clear and precise boundaries exist between the use of “low sensitivity” and “moderate sensitivity” labeling, for example.

    * **Data Sensitivity Levels and Labels**: unless otherwise mandated, organizations are free to create classification systems that best meet their own needs. In professional practice, it is typically best if the organization has enough classifications to distinguish between sets of assets with differing sensitivity/value, but not so many classifications that the distinction between them is confusing to individuals. Typically, two or three classifications are manageable, and more than four tend to be difficult.

    **Highly restricted**: Compromise of data with this sensitivity label could possibly put the organization’s future existence at risk. Compromise could lead to substantial loss of life, injury or property damage, and the litigation and claims that would follow. **Moderately restricted**: Compromise of data with this sensitivity label could lead to loss of temporary competitive advantage, loss of revenue or disruption of planned investments or activities. **Low sensitivity (sometimes called “internal use only”)**: Compromise of data with this sensitivity label could cause minor disruptions, delays or impacts. Unrestricted public data: As this data is already published, no harm can come from further dissemination or disclosure.
* **Retention**: **Information and data should be kept only for as long as it is beneficial, no more and no less**. Certain industry standards, laws and regulations define retention periods, when such external requirements are not set, it is an organization’s responsibility to define and implement its own data retention policy. **Data retention policies are applicable both for hard copies and for electronic data**, and no data should be kept beyond its required or useful life. **Security professionals should ensure that data destruction is being performed when an asset has reached its retention limit**. For the security professional to succeed in this assignment, an accurate inventory must be maintained, including the asset location, retention period requirement, and destruction requirements. Organizations should conduct a periodic review of retained records in order to reduce the volume of information stored and to ensure that only necessary information is preserved.

Records retention policies indicate how long an organization is required to maintain information and assets. Policies should guarantee that: \* Personnel understand the various retention requirements for data of different types throughout the organization.  \* The organization appropriately documents the retention requirements for each type of information. \* The systems, processes and individuals of the organization retain information in accordance with the required schedule but no longer. \* A common mistake in records retention is applying the longest retention period to all types of information in an organization. This not only wastes storage but also increases risk of data exposure and adds unnecessary “noise” when searching or processing information in search of relevant records. It may also be in violation of externally mandated requirements such as legislation, regulations or contracts (which may result in fines or other judgments). Records and information no longer mandated to be retained should be destroyed in accordance with the policies of the enterprise and any appropriate legal requirements that may need to be considered.

* Destruction: Data that might be left on media after deleting is known as remanence and may be a significant security concern. Steps must be taken to reduce the risk that data remanence could compromise sensitive information to an acceptable level. This can be done by one of several means:
  * Clearing the device or system, which usually involves **writing multiple patterns of random values throughout all storage media**. This is sometimes **called “overwriting” or “zeroizing” the system**, although writing zeros has the risk that a missed block or storage extent may still contain recoverable, sensitive information after the process is completed.
  * Purging the device or system, which eliminates (or greatly reduces) the chance that residual physical effects from the writing of the original data values may still be recovered, even after the system is cleared. Some magnetic disk storage technologies, for example, can still have residual “ghosts” of data on their surfaces even after being overwritten multiple times. Magnetic media, for example, can often be altered sufficiently to meet security requirements; in more stringent cases, degaussing may not be sufficient.
  * Physical destruction of the device or system is the ultimate remedy to data remanence. Magnetic or optical disks and some flash drive technologies may require being mechanically shredded, chopped or broken up, etched in acid or burned; their remains may be buried in protected landfills, in some cases.
  * In many routine operational environments, security considerations may accept that clearing a system is sufficient. But when systems elements are to be removed and replaced, either as part of maintenance upgrades or for disposal, purging or destruction may be required to protect sensitive information from being compromised by an attacker.

### Logging and Monitoring Security Events

Logging is the primary form of instrumentation that attempts to capture signals generated by events. Events are any actions that take place within the systems environment and cause measurable or observable change in one or more elements or resources within the system. **Logging imposes a computational cost but is invaluable when determining accountability**. Proper design of logging environments and regular log reviews remain best practices regardless of the type of computer system.

Major controls frameworks emphasize the importance of organizational logging practices. Information that may be relevant to being recorded and reviewed include (but is not limited to): user IDs, system activities, dates/times of key events (e.g., logon and logoff), device and location identity, successful and rejected system and resource access attempts, system configuration changes and system protection activation and deactivation events.

**Logging and monitoring the health of the information environment is essential to identifying inefficient or improperly performing systems**, detecting compromises and providing a record of how systems are used. **Robust logging practices provide tools to effectively correlate information from diverse systems to fully understand the relationship between one activity and another**.

Log reviews are an essential function not only for security assessment and testing but also **for identifying security incidents, policy violations, fraudulent activities and operational problems near the time of occurrence**. Log reviews support audits – forensic analysis related to internal and external investigations – and provide support for organizational security baselines. Review of historic audit logs can determine if a vulnerability identified in a system has been previously exploited.

It is helpful for an organization to create components of a log management infrastructure and determine how these components interact. This aids in preserving the integrity of log data from accidental or intentional modification or deletion and in maintaining the confidentiality of log data.

Controls are implemented to protect against unauthorized changes to log information. Operational problems with the logging facility are often related to alterations to the messages that are recorded, log files being edited or deleted, and storage capacity of log file media being exceeded. Organizations must maintain adherence to retention policy for logs as prescribed by law, regulations and corporate governance. Since attackers want to hide the evidence of their attack, the organization’s policies and procedures should also address the preservation of original logs. Additionally, the logs contain valuable and sensitive information about the organization. Appropriate measures must be taken to protect the log data from malicious use.

### Event Logging Best Practices

Different tools are used depending on whether the risk from the attack is from traffic coming into or leaving the infrastructure.

**Ingress monitoring refers to surveillance and assessment of all inbound communications traffic and access attempts.** Devices and tools that offer logging and alerting opportunities for ingress monitoring include: Firewalls, Gateways, Remote authentication servers, IDS/IPS tools, SIEM solutions, Anti-malware solutions.

**Egress monitoring is used to regulate data leaving the organization’s IT environment.** The term currently used in conjunction with this effort is **data loss prevention (DLP)** or **data leak protection**. The DLP solution should be deployed so that it can inspect all forms of data leaving the organization, including: Email (content and attachments), Copy to portable media, File Transfer Protocol (FTP), Posting to web pages/websites, Applications/application programming interfaces (APIs).

### Encryption Overview

Almost every action we take in our modern digital world involves cryptography. Encryption protects our personal and business transactions; digitally signed software updates verify their creator’s or supplier’s claim to authenticity. Digitally signed contracts, binding on all parties, are routinely exchanged via email without fear of being repudiated later by the sender. Cryptography is used to protect information by keeping its meaning or content secret and making it unintelligible to someone who does not have a way to decrypt (unlock) that protected information. The objective of every encryption system is to transform an original set of data, called the plaintext, into an otherwise unintelligible encrypted form, called the ciphertext. Properly used, singly or in combination, cryptographic solutions provide a range of services that can help achieve required systems security postures in many ways:

* Confidentiality: Cryptography provides confidentiality by hiding or obscuring a message so that it cannot be understood by anyone except the intended recipient. Confidentiality keeps information secret from those who are not authorized to have it.
* Integrity: hash functions and digital signatures can provide integrity services that allow a recipient to verify that a message has not been altered by malice or error. These include simple message integrity controls. Any changes, deliberate or accidental, will result in the two results (by sender and by recipient) being different.

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/K8tMBWD1StuLTAVg9drbRQ_f4d96e5b1bc44e079f81d05adad794f1_EDU-ELCC-70565-crypto_system_components.svg?expiry=1691280000000&#x26;hmac=GbOa8iaUKsT9HghlQu1egzHOA8I5bQUUVSGZ3QfVPJM" alt="diagram of plaintext input put through a process of encryption and decryption followed by plaintext output"><figcaption></figcaption></figure>

An encryption system is the set of hardware, software, algorithms, control parameters and operational methods that provide a set of encryption services. Plaintext is the data or message in its normal, unencrypted form and format. Its meaning or value to an end user (a person or a process) is immediately available for use. Plaintext can be:

* image, audio or video files in their raw or compressed forms
* human-readable text and numeric data, with or without markup language elements for formatting and metadata
* database files or records and fields within a database
* or anything else that can be represented in digital form for computer processing, transmission and storage

It is important to remember that plaintext can be anything—much of which is not readable to humans in the first place.





### Symmetric Encryption

The central characteristic of a symmetric algorithm is that it uses the same key in both the encryption and the decryption processes. It could be said that the decryption process is just a mirror image of the encryption process. This image displays how symmetric algorithms work. The same key is used for both the encryption and decryption processes. This means that the two parties communicating need to share knowledge of the same key. This type of algorithm protects data, as a person who does not have the correct key would not be able to read the encrypted message. Because the key is shared, however, this can lead to several other challenges:

* If two parties suspect a specific communication path between them is compromised, they obviously can't share key material along that path. Someone who has compromised communications between the parties would also intercept the key.
* Distribution of the key is difficult, because the key cannot be sent in the same channel as the encrypted message, or the man-in-the-middle (MITM) would have access to the key. Sending the key through a different channel (band) than the encrypted message is called out-of-band key distribution. Examples of out-of-band key distribution would include sending the key via courier, fax or phone.
* Any party with knowledge of the key can access (and therefore change) the message.
* Each individual or group of people wishing to communicate would need to use a different key for each individual or group they want to connect with. This raises the challenge of scalability — the number of keys needed grows quickly as the number of different users or groups increases. Under this type of symmetric arrangement, an organization of 1,000 employees would need to manage 499,500 keys if every employee wanted to communicate confidentially with every other employee.

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/FBhmSWYPQoKYZklmD1KCsg_f10a6ef6327347919b7e0a238a8647f1_EDU-ELCC-00553-techart-Use_of_symmetric_algorithms-v07.svg?expiry=1691280000000&#x26;hmac=RoT9ssasKLMgtIQxMx46SZBvKLT_J-opuPGi-aunNwc" alt="Diagram of symmetric encryption process from sender to receiver"><figcaption></figcaption></figure>

Primary uses of symmetric algorithms:

* Encrypting bulk data (backups, hard drives, portable media)
* Encrypting messages traversing communications channels (IPsec, TLS)
* Streaming large-scale, time-sensitive data (audio/video materials, gaming, etc.

Other names for symmetric algorithms, which you may encounter, include:

* Same key
* Single key
* Shared key
* Secret key
* Session key

An example of symmetric encryption is a substitution cipher, which involves the simple process of substituting letters for other letters, or more appropriately, substituting bits for other bits, based upon a cryptovariable. These ciphers involve replacing each letter of the plaintext with another that may be further down the alphabet.

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/XShd_2DgSkyoXf9g4HpMvA_7b962e61cead43eda01b000b252e25f1_EDU-ELCC-70635-techart-Symmetric_Encryption_via_Decoding_Ring-v01.svg?expiry=1691280000000&#x26;hmac=lBTvE3Jtnek8qcp10fO1AHG50_YTj-Eaw-CddLChg-Y" alt="Image of symmetric decoding ring"><figcaption></figcaption></figure>



### Asymmetric Encryption

Asymmetric encryption uses one key to encrypt and a different key to decrypt the input plaintext. This is in stark contrast to symmetric encryption, which uses the same key to encrypt and decrypt. For most security professionals, the math of asymmetric encryption can be left to the cryptanalysts and cryptographers to know. A user wishing to communicate using an asymmetric algorithm would first generate a key pair. To ensure the strength of the key generation process, this is usually done by the cryptographic application or the public key infrastructure (PKI) implementation without user involvement. One half of the key pair is kept secret; only the key holder knows that key. This is why it is called the private key. The other half of the key pair can be given freely to anyone who wants a copy. In many companies, it may be available through the corporate website or access to a key server. Therefore, this second half of the key pair is referred to as the public key. Note that anyone can encrypt something using the recipient’s public key, but only the recipient —with their private key—can decrypt it. Asymmetric key cryptography solves the problem of key distribution by allowing a message to be sent across an untrusted medium in a secure manner without the overhead of prior key exchange or key material distribution. It also allows for several other features not readily available in symmetric cryptography, such as the non-repudiation of origin and delivery, access control and data integrity. Asymmetric key cryptography also solves the problem of scalability. It does scale well as numbers increase, as each party only requires a key pair, the private and public keys. An organization with 100,000 employees would only need a total of 200,000 keys (one private and one public for each employee). This is less than half of the number of keys that would be required for symmetric encryption. The problem, however, has been that asymmetric cryptography is extremely slow compared with its symmetric counterpart. Asymmetric cryptography is impractical for everyday use in encrypting large amounts of data or for frequent transactions where speed is required. This is because asymmetric key cryptography is handling much larger keys and is mathematically intensive, thereby reducing the speed significantly.

Let’s look at an example that illustrates the use of asymmetric cryptography to achieve different security attributes. The two keys (private and public) are a key pair; they must be used together. This means that any message that is encrypted with a public key can only be decrypted with the corresponding other half of the key pair, the private key. Similarly, signing a message with a sender’s private key can only be verified by the recipient decrypting its signature with the sender’s public key. Therefore, as long as the key holder keeps the private key secure, there exists a method of transmitting a message confidentially. The sender would encrypt the message with the public key of the receiver. Only the receiver with the private key would be able to open or read the message, providing confidentiality. This image shows how asymmetric encryption can be used to send a confidential message across an untrusted channel.

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/tA1ZPCQDT22NWTwkA99tnw_6e6d76fa8f4a4adea97bcf31a7e5e8f1_EDU-ELCC-00655-techart-asymmetric_crypto-v03.svg?expiry=1691280000000&#x26;hmac=x7LowvahsoSZTbF5NByz8ZDYvbXOrrflhs0MFgZJPI8" alt="diagram of the asymmetric encryption process"><figcaption></figcaption></figure>

### Encryption Overview - Hashing

###

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/llHUa2RqSp-R1GtkaoqfqQ_660a080f84a74760ba0741fbe2ff97f1_EDU-ELCC-00685-techart-hash_values-v01.svg?expiry=1691280000000&#x26;hmac=VSin2fovXsR48ZRqYL55pKvMxnR-qgPtI8Ssb91NCvM" alt="Diagram showing how slight changes in the input message result in different hash values"><figcaption></figcaption></figure>

As seen in this image, even the slightest change in the input message results in a completely different hash value. Hash functions are very sensitive to any changes in the message. Because the size of the hash digest does not vary according to the size of the message, a person cannot tell the size of the message based on the digest.

<figure><img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Mcaafs2SSbmGmn7Nkum5EQ_b637d592eac94fd08c9f7a025b1774f1_EDU-ELCC-00680-techart-hash_ops-v05.svg?expiry=1691280000000&#x26;hmac=sQC_kfZ7-dutGekowAYFndihfLQ7t6TCCCIRF2HeQ8Q" alt="Diagram of a simple hashing function"><figcaption></figcaption></figure>

variable data input + hashing algorithm = fixed bit size data output (the digest)

Cryptographic hash functions have many applications in information security, including digital signatures, message authentication codes and other forms of authentication. They can also be used for fingerprinting, to detect duplicate data or uniquely identify files, and as checksums to detect accidental data corruption. The operation of a hashing algorithm is demonstrated in this image. This is an example of a simple hashing function. The originator wants to send a message to the receiver and ensure that the message is not altered by noise or lost packets as it is transmitted. The originator runs the message through a hashing algorithm that generates a hash, or a digest of the message. The digest is appended to the message and sent together with the message to the recipient. Once the message is delivered, the receiver will generate their own digest of the received message (using the same hashing algorithm). The digest of the received message is compared with the digest sent by the originator. If the digests are the same, the received message is the same as the sent message. The problem with a simple hash function like this is that it does not protect against a malicious attacker that would be able to change both the message and the hash/digest by intercepting it in transit. The general idea of a cryptographic hash function can be summarized with the following formula:

* Useful: It is easy to compute the hash value for any given message.
* Nonreversible: It is computationally infeasible to reverse the hash process or otherwise derive the original plaintext of a message from its hash value (unlike an encryption process, for which there must be a corresponding decryption process).
* Content integrity assurance: It is computationally infeasible to modify a message such that re-applying the hash function will produce the original hash value. 
* Unique: It is computationally infeasible to find two or more different, sensible messages that hash to the same value.
* Deterministic: The same input will always generate the same hash, when using the same hashing algorithm.

Hashing takes an input set of data (of almost arbitrary size) and returns a fixed-length result called the hash value. A hash function is the algorithm used to perform this transformation. When used with cryptographically strong hash algorithms, this is the most common method of ensuring message integrity today. Hashes have many uses in computing and security, one of which is to create a message digest by applying such a hash function to the plaintext body of a message.  To be useful and secure, a cryptographic hash function must demonstrate five main properties: 

### &#x20;
