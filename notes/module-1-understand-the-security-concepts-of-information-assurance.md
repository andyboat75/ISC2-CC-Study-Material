---
description: Domain D1.1.1, D1.1.2, D1.1.3, D1.1.4, D1.1.5, D1.1.6
---

# Module 1 Understand the Security Concepts of Information Assurance

### Confidentiality

It relates to permitting authorized access to information, while at the same time protecting information from improper disclosure. Difficulties to achieve confidentiality are related to: **many users are guests or customers**, and it is not clear if the access comes from a compromised machine or vulnerable mobile application. To avoid those difficulties, security professionals must regulate access, permitting access to authorized individuals, for that protecting the data that needs protection.

Data that needs protections is also known **as PII or PHI**. **PII** stands for Personally Identifiable Information and it is related to the area of confidentiality and it means any data that could be used to identify an individual. **PHI** stands for Protected Health Information and it comprehends information about one's health status, and classified or sensitive information, which includes trade secrets, research, business plans and intellectual property.

Related to confidentiality is **the concept sensitivity a measure of the importance assigned to information by its owner**, or the purpose of denoting its need for protection. **Sensitive information** is information that if improperly disclosed (confidentiality) or modified (integrity) would harm an organization or individual. In many cases, sensitivity is related to the harm to external stakeholders; that is, people or organizations that may not be a part of the organization that processes or uses the information.

Threat related to confidentiality are:

1. Snooping involves gathering information that is left out in the open. Clean desk policies protect against snooping.
2. Dumpster diving also looking for sensitive materials, but in the dumpster, a paper shredding protects against it.
3. Eavesdropping occurs when someone secretly listen to a conversation, and it can be prevent with rules about sensitive conversations
4. Wiretapping is the electronic version of eavesdropping, the best way against that is using encryption to protect the communication.
5. Social Engineering, the best defense is educate users to protect them against social engineering.

### Integrity

It is the property of information whereby it is recorded, used and maintained in a way that ensures its completeness, accuracy, internal consistency and usefulness for a stated purpose, which can be applied **to information or data**, **system and process for business operations**, **organizations**, **people and their actions**. Furthermore, restrict to data integrity, it is an assurance that data has not been altered in an unauthorized manner, covering data **in storage**, during **processing**, and while **in transit**.

**Consistency** is another concept related to integrity and requires that all instances of the data be identical in form, content and meaning. When related to system integrity, it refers to the maintenance of a known good configuration and expected operational function as the system processes the information. Ensuring integrity begins with an awareness of state, which is the current condition of the system. Specifically, this awareness concerns the ability to document and understand the state of data or a system at a certain point, **creating a baseline**. A baseline, which means a documented, lowest level of security configuration allowed by a standard or organization, can refer to the current state of the information—whether it is protected.

To preserve that state, the information must always continue to be protected through a transaction. Going forward from that baseline, the integrity of the data or the system can always be ascertained by comparing the baseline with the current state. If the two match, then the integrity of the data or the system is intact; if the two do not match, then the integrity of the data or the system has been compromised. Integrity is a primary factor in the reliability of information and systems. The need to safeguard information and system integrity may be dictated by laws and regulations. Often, it is dictated by the needs of the organization to access and use reliable, accurate information.

1. Unauthorized modification attacks make changes without permission. The best way to protect against that is the least privilege principle.
2. Impersonation attacks pretend to be someone else. User education protects against impersonation attack.
3. Man-In-The-Middle (MITM) attacks place the attacker in the middle of a communication session, monitoring everything that's occurring.
4. Replay attacks eavesdrop on logins and reuse the captured credentials.

To both MiTM and Replay attacks the best approach is encryption.

### Availability

It means that systems and data are accessible at the time users need them. It can be defined as timely and reliable access to information and the ability to use it, and for authorized users, timely and reliable access to data and information services. The core concept of availability is that data is accessible **to authorized users when and where it is needed and in the form and format required**. This does not mean that data or systems are available 100% of the time. Instead, the systems and data meet the requirements of the business for timely and reliable access. **Some systems and data are far more critical than others**, so the security professional **must ensure that the appropriate levels of availability are provided**. This requires consultation with the involved business to ensure that critical systems are identified and available. Availability is often associated with the term **criticality**, which means a measure of the degree to which an organization depends on the information or information system for the success of a mission or of a business function (NIST SP 800-60), because it represents the importance an organization gives to data or an information system in performing its operations or achieving its mission

1. Denial of Service can be mitigated using firewalls to block unauthorized connections
2. Power outages can be mitigated using redundant power and generators
3. Hardware failures can be mitigated using redundant components
4. Destruction can be mitigated using backups
5. Service outages

### Three steps to gain access, known as triple A, which means Authentication, Authorization, Accounting

#### Identification

Consist of making a claim of identity

#### Authentication

When users have stated their identity, it is necessary **to validate that they are the rightful owners of that identity**. This process of verifying or proving the user’s identification is known as authentication, which means in another terms access control process validating that the identity being claimed by a user or entity is known to the system, by comparing one (single-factor or SFA) or more (multi-factor authentication or MFA) factors of authentication. Simply put, authentication is a process to prove the identity of the requestor.

There are three common methods of authentication:

* Something you know: Passwords or paraphrases
* Something you have: Tokens (NISTIR 7711), memory cards, smart cards
* Something you are: Biometrics , measurable characteristics

#### Methods of Authentication

There are two types of authentication. Using only one of the methods of authentication stated previously is **known as single-factor authentication (SFA)**. Granting users access only after successfully demonstrating or displaying two or more of these methods is **known as multi-factor authentication (MFA)**.

**Common best practice is to implement at least two of the three common techniques for authentication**:

* Knowledge-based 
* Token-based 
* Characteristic-based 

Knowledge-based authentication uses a passphrase or secret code to differentiate between an authorized and unauthorized user. If you have selected a personal identification number (PIN), created a password or some other secret value that only you know, then you have experienced knowledge-based authentication. The problem with using this type of authentication alone is that it is often vulnerable to a variety of attacks. For example, the help desk might receive a call to reset a user’s password. The challenge is ensuring that the password is reset only for the correct user and not someone else pretending to be that user. For better security, a second or third form of authentication that is based on a token or characteristic would be required prior to resetting the password. The combined use of a user ID and a password consists of two things that are known, and because it does not meet the requirement of using two or more of the authentication methods stated, it is not considered MFA.

#### Password

* Password length requirements set a minimum number of chars
* Password complexity requirements describe the types of characters that must be included
* Password expiration requirements force password changes. Nowadays, that requirement isn't used, companies change to an approach where force password change is required when there is any evidence that the password has been compromised.
* Password history requirements prevent password reuse.
* Provide a way to change the password quickly and easily.
* Encourage users to not reuse the same password across multiple sites
* Password managers facilitate the use of strong, unique passwords

#### Authorization

Ensuring that an action is allowed.

#### Accounting

Its maintains logs of activity

### Non-repudiation

Non-repudiation is a legal term and is defined as the protection against an individual falsely denying having performed a particular action. It provides the capability to determine whether a given individual took a particular action, such as created information, approved information or sent or received a message.

In today’s world of e-commerce and electronic transactions, **there are opportunities for the impersonation of others or denial of an action, such as making a purchase online and later denying it**. It is important that all participants trust online transactions. **Non-repudiation methodologies ensure that people are held responsible for transactions they conducted**.

### Base Concepts

1. Authorization: the right or a permission that is granted to a system entity to access a system resource
2. Integrity: the property that data has not been altered in an unauthorized manner
3. Confidentiality: the characteristic of data or information when it is not made available or disclosed to unauthorized persons or process
4. Privacy: the right of an individual to control the distribution of information about themselves
5. Availability: Ensuring timely and reliable access to and use of information by authorized users
6. Non-repudiation: The inability to deny taking an action, such as sending an email message
7. Authentication: Access control process that compares one or more factors of identification to validate that the identity claimed by a user or entity is known to the system

### Privacy

Privacy is **the right of an individual to control the distribution of information about themselves**. While security and privacy both focus on the protection of personal and sensitive data, there is a difference between them. With the increasing rate at which data is collected and digitally stored across all industries, the push for privacy legislation and compliance with existing policies steadily grows. In today’s global economy, privacy legislation and regulations on privacy and data protection can impact corporations and industries regardless of physical location. **Global privacy is an especially crucial issue when considering requirements regarding the collection and security of personal information**. There are several laws that define privacy and data protection, which periodically change. Ensuring that protective security measures are in place is not enough to meet privacy regulations or to protect a company from incurring penalties or fines from mishandling, misuse, or improper protection of personal or private information. An example of a law with multinational implications is the European Union’s General Data Protection Regulation (GDPR) which applies to all organizations, foreign or domestic, doing business in the EU or any persons in the EU. Companies operating or doing business within the United States may also fall under several state legislations that regulate the collection and use of consumer data and privacy. Likewise, member nations of the EU enact laws to put GDPR into practice and sometimes add more stringent requirements. These laws, including national- and state-level laws, dictate that any entity anywhere in the world handling the private data of people in a particular legal jurisdiction must abide by its privacy requirements. As a member of an organization's data protection team, you will not be required to interpret these laws, but you will need an understanding of how they apply to your organization.
