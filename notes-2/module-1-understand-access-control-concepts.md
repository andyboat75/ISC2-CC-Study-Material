---
description: Domain D3.1, D3.1.3, D3.1.5, D3.2, D3.2.1, D3.2.2, D3.2.5
---

# Module 1 Understand Access Control Concepts

## What is Security Control?

Access control involves **limiting what objects can be available to what subjects according to what rules**.

## Controls Overview

Earlier in this course we looked at security principles through foundations of risk management, governance, incident response, business continuity and disaster recovery. But in the end, security all comes down to, **“who can get access to organizational assets (buildings, data, systems, etc.) and what can they do when they get access?”**

Access controls **are not just about restricting access** to information systems and data, **but also about allowing access**. It is about granting the appropriate level of access to authorized personnel and processes and denying access to unauthorized functions or individuals.

Access is based on three elements:

### Subjects

### **Subject is any entity that requests access to our assets**. The entity requesting access may be a **user**, a **client**, a **process** or a **program**, for example. A subject is the initiator of a request for service; therefore, a subject is referred to as “active.”

* &#x20;A subject:
  * Is a user, a process, a procedure, a client (or a server), a program, a device such as an endpoint, workstation, smartphone or removable storage device with onboard firmware.
  * Is active: It initiates a request for access to resources or services.
  * Requests a service from an object.
  * Should have a level of clearance (permissions) that relates to its ability to successfully access services or resources.

### Objects

By definition, anything that a subject attempts to access is referred to as an object. An object is a device, process, person, user, program, server, client or other entity that responds to a request for service. Whereas a subject is active in that it initiates a request for a service, an object is passive in that it takes no action until called upon by a subject. When requested, an object will respond to the request it receives, and if the request is wrong, the response will probably not be what the subject really wanted either.

Note that by definition, objects do not contain their own access control logic. Objects are passive, not active (in access control terms), and must be protected from unauthorized access by some other layers of functionality in the system, such as the integrated identity and access management system. An object has an owner, and the owner has the right to determine who or what should be allowed access to their object. Quite often the rules of access are recorded in a rule base or access control list.

An object:

* Is a building, a computer, a file, a database, a printer or scanner, a server, a communications resource, a block of memory, an input/output port, a person, a software task, thread or process.
* Is anything that provides service to a user.
* Is passive.
* Responds to a request.
* May have a classification.



### Rules

An access rule is an instruction developed to allow or deny access to an object by comparing the validated identity of the subject to an access control list. One example of a rule is a firewall access control list. By default, firewalls deny access from any address to any address, on any port. For a firewall to be useful, however, it needs more rules. A rule might be added to allow access from the inside network to the outside network. Here we are describing a rule that allows access to the object “outside network” by the subject having the address “inside network.” In another example, when a user (subject) attempts to access a file (object), a rule validates the level of access, if any, the user should have to that file. To do this, the rule will contain or reference a set of attributes that define what level of access has been determined to be appropriate. A rule can:

* Compare multiple attributes to determine appropriate access.
* Allow access to an object.
* Define how much access is allowed.
* Deny access to an object.
* Apply time-based access.

### Controls Assessments

Risk reduction depends on the effectiveness of the control. It must apply to the current situation and adapt to a changing environment.

## Defense in Depth

We are looking at all access permissions including building access, access to server rooms, access to networks and applications and utilities. These are all implementations of access control and are part of **a layered defense strategy**, **also known as defense in depth**, developed by an organization.

<mark style="color:blue;">**Defense in depth describes an information security strategy that integrates people, technology and operations capabilities to establish variable barriers across multiple layers and missions of the organization**</mark>**.** It applies multiple countermeasures in a layered fashion to fulfill security objectives. Defense in depth should be implemented to prevent or deter a cyberattack, but it cannot guarantee that an attack will not occur.

A technical example of defense in depth, in which multiple layers of technical controls are implemented, **is when a username and password are required for logging in to your account, followed by a code sent to your phone to verify your identity**. **This is a form of multi-factor authentication using methods on two layers, something you have and something you know.** The combination of the two layers is much more difficult for an adversary to obtain than either of the authentication codes individually.

Another example of multiple technical layers is when additional firewalls are used to separate untrusted networks with differing security requirements, such as the internet from trusted networks that house servers with sensitive data in the organization. When a company has information at multiple sensitivity levels, it might require the network traffic to be validated by rules on more than one firewall, with the most sensitive information being stored behind multiple firewalls.

For a non-technical example, consider the multiple layers of access required to get to the actual data in a data center. First, a lock on the door provides a physical barrier to access the data storage devices. Second, a technical access rule prevents access to the data via the network. Finally, a policy, or administrative control defines the rules that assign access to authorized individuals.

### <mark style="color:blue;">Principle of Least Privilege</mark>

The Principle of Least Privilege (NIST SP 800-179) is a standard of permitting only minimum access necessary for users or programs to fulfill their function. Users are provided access only to the systems and programs they need to perform their specific job or tasks.

To preserve the confidentiality of information and ensure that it is only available to personnel who are authorized to see it, **we use privileged access management**, **which is based on the principle of least privilege**. **That means each user is granted access only to the items they need and nothing further**.

For example, only individuals working in billing will be allowed to view consumer financial data, and even fewer individuals will have the authority to change or delete that data. This maintains confidentiality and integrity while also allowing availability by providing administrative access with an appropriate password or sign-on that proves the user has the appropriate permissions to access that data.

Sometimes it is necessary to allow users to access the information via a temporary or limited access, for instance, for a specific time period or just within normal business hours. Or access rules can limit the fields that the individuals can have access to. One example is a healthcare environment. Some workers might have access to patient data but not their medical data. Individual doctors might have access only to data related to their own patients. In some cases, this is regulated by law, such as HIPAA in the United States, and by specific privacy laws in other countries.

Systems often monitor access to private information, and if logs indicate that someone has attempted to access a database without the proper permissions, that will automatically trigger an alarm. The security administrator will then record the incident and alert the appropriate people to take action.

The more critical information a person has access to, the greater the security should be around that access. They should definitely have multi-factor authentication, for instance.

### Privileged Access Management

Privileged access management provides the first and perhaps most familiar use case. Consider a human user identity that is granted various create, read, update, and delete privileges on a database. Without privileged access management, the system’s access control would have those privileges assigned to the administrative user in a static way, effectively “on” 24 hours a day, every day. Security would be dependent upon the login process to prevent misuse of that identity. Just-in-time privileged access management, by contrast, includes role-based specific subsets of privileges that only become active in real time when the identity is requesting the use of a resource or service.

### Privileged Accounts

Privileged accounts are those with permissions beyond those of normal users, such as managers and administrators. Broadly speaking, these accounts have **elevated privileges** and are used by many different classes of users, including:

* Systems administrators, who have the principal responsibilities for operating systems, applications deployment and performance management.
* Help desk or IT support staff, who often need to view or manipulate endpoints, servers and applications platforms by using privileged or restricted operations.
* Security analysts, who may require rapid access to the entire IT infrastructure, systems, endpoints and data environment of the organization.

Other classes of privileged user accounts may be created on a per-client or per-project basis, to allow a member of that project or client service team to have greater control over data and applications. These few examples indicate that organizations often need to delegate the capability to manage and protect information assets to various managerial, supervisory, support or leadership people, with differing levels of authority and responsibility. This delegation, of course, should be contingent upon trustworthiness, since misuse or abuse of these privileges could lead to harm for the organization and its stakeholders.

Typical measures used for moderating the potential for elevated risks from misuse or abuse of privileged accounts include the following:

* More extensive and detailed logging than regular user accounts. The record of privileged actions is vitally important, as both a deterrent (for privileged account holders that might be tempted to engage in untoward activity) and an administrative control (the logs can be audited and reviewed to detect and respond to malicious activity).
* More stringent access control than regular user accounts. As we will see emphasized in this course, even nonprivileged users should be required to use MFA methods to gain access to organizational systems and networks. Privileged users—or more accurately, highly trusted users with access to privileged accounts—should be required to go through additional or more rigorous authentication prior to those privileges. Just-in-time identity should also be considered as a way to restrict the use of these privileges to specific tasks and the times in which the user is executing them.
* Deeper trust verification than regular user accounts. Privileged account holders should be subject to more detailed background checks, stricter nondisclosure agreements and acceptable use policies, and be willing to be subject to financial investigation. Periodic or event-triggered updates to these background checks may also be in order, depending on the nature of the organization’s activities and the risks it faces.
* More auditing than regular user accounts. Privileged account activity should be monitored and audited at a greater rate and extent than regular usage.

### Segregation of Duties

A core element of authorization is the **principle of segregation of duties** (also known as separation of duties). <mark style="color:blue;">**Segregation of duties is based on the security practice that no one person should control an entire high-risk transaction from start to finish**</mark>. **Segregation of duties breaks the transaction into separate parts and requires a different person to execute each part of the transaction**. For example, an employee may submit an invoice for payment to a vendor (or for reimbursement to themselves), but it must be approved by a manager prior to payment; in another instance, almost anyone may submit a proposal for a change to a system configuration, but the request must go through technical and management review and gain approval, before it can be implemented.

These steps can prevent fraud or detect an error in the process before implementation. It could be that the same employee might be authorized to originally submit invoices regarding one set of activities, but not approve them, and yet also have approval authority but not the right to submit invoices on another. It is possible, of course, that two individuals can willfully work together to bypass the segregation of duties, so that they could jointly commit fraud. This is called collusion.

Another implementation of segregation of duties is dual control. This would apply at a bank where there are two separate combination locks on the door of the vault. Some personnel know one of the combinations and some know the other, but no one person knows both combinations. Two people must work together to open the vault; thus, the vault is under dual control.

**The two-person rule is a security strategy that requires a minimum of two people to be in an area together, making it impossible for a person to be in the area alone**. Many access control systems prevent an individual cardholder from entering a selected high-security area unless accompanied by at least one other person. Use of the two-person rule can help reduce insider threats to critical areas by requiring at least two individuals to be present at any time. It is also used for life safety within a security area; if one person has a medical emergency, there will be assistance present.

### How Users Are Provisioned

Other situations that call for provisioning new user accounts or changing privileges include:

* **A new employee**: When a new employee is hired, the hiring manager sends a request to the security administrator to create a new user ID. This request authorizes creation of the new ID and provides instructions on appropriate access levels. Additional authorization may be required by company policy for elevated permissions.
* **Change of position**: When an employee has been promoted, their permissions and access rights might change as defined by the new role, which will dictate any added privileges and updates to access. At the same time, any access that is no longer needed in the new job will be removed.
* **Separation of employment**: When employees leave the company, depending on company policy and procedures, their accounts must be disabled after the termination date and time. It is recommended that accounts be disabled for a period before they are deleted to preserve the integrity of any audit trails or files that may be owned by the user. Since the account will no longer be used, it should be removed from any security roles or additional access profiles. This protects the company, so the separated employee is unable to access company data after separation, and it also protects them because their account cannot be used by others to access data.
