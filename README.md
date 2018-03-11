# Certified Information Systems Security Professional (CISSP) notes

## Security and Risk Management
The essence of our work as security professionals is our understanding of two key terms: security and risk.

### Fundamental Principles of Security
The core goals of security, are to provide __availability__, __integrity__, and __confidentiality__ (often referred as CIA triad) protection for critical assets. All risks, threats, and vulnerabilities are measured for their potential capability to compromise one or all of the CIA principles.

<p align="center">
  <img src="https://raw.githubusercontent.com/halenai/cissp-notes/master/images/CIA_triad.jpg" alt="CIA triad">
</p>

#### Availability
Availability protection ensures reliability and timely access to data and resources to _authorized individuals_. Necessary protection mechanisms must be in place to protect against inside and outside threats that could affect the availability and productivity of all business-processing components.
* Redundant array of independent disks (RAID)
* Clustering
* Load balancing
* Redundant data and power lines
* Software and data backups
* Disk shadowing
* Co-location and offsite facilities
* Rollback functions 
* Failover configurations

#### Integrity
Integrity is upheld when the assurance of the accuracy and reliability of information and systems is provided and any unauthorized modification is prevented.
* Hashing (data integrity)
* Configuration management (system integrity)
* Change control (process integrity)
* Access control (physical and technical)
* Software digital signing
* Transmission cyclic redundancy check (CRC) functions

#### Confidentiality
Confidentiality ensures that the necessary level of secrecy is enforced at each junction of data processing and prevents unauthorized disclosure. This level of secrecy should prevail while data resides on systems and devices within the network, as it is transmitted, and once it reaches its destination.
* Encryption for data at rest (whole disk, database encryption)
* Encryption for data in transit (IPSec, TLS, PPTP, SSH)
* Access control (physical and technical)

### Security Definitions
__Vulnerability__ is a weakness in a system that allows a threat source to compromise its security.  
__Threat__ is any potential danger that is associated with the exploitation of a vulnerability. The entity that takes advantage of a vulnerability is referred to as a _threat agent_.  
__Risk__ is the likelihood of a threat source exploiting a vulnerability and the corresponding business impact. Risk ties the vulnerability, threat, and the likelihood of exploitation to the resulting business impact.  
__Exposure__ is an instance of being exposed to losses. A vulnerability exposes an organization to possible damages.  
__Control__ or countermeasure, is put into place to mitigate the potential risk.

Applying the right countermeasure can eliminate the vulnerability and exposure, and thus reduce the risk. The company cannot eliminate the threat agent, but it can protect itself and prevent this threat agent from exploiting vulnerabilities within the environment.

### Control Types
Controls are put into place to reduce the risk an organization faces, and they come in three main flavors: __administrative__, __technical__, and __physical__. Administrative controls are commonly referred to as "soft controls" because they are more management oriented (security documentation, risk management, training). Technical controls (also called logical controls) are software or hardware components (firewalls, IDS, encryption, identification and authentication mechanisms). And physical controls are items put into place to protect facility, personnel, and resources (security guards, locks, fencing)

These controls need to be put into place to provide defense-in-depth, which is the coordinated use of multiple security controls in a layered approach.

<p align="center">
  <img src="https://raw.githubusercontent.com/halenai/cissp-notes/master/images/defense_in_depth.jpg" alt="Defense in Depth">
</p>

The types of controls that are actually implemented must map to the threats the company faces, and the number of layers that are put into place must map to the sensitivity of the asset. The rule of thumb is the more sensitive the asset, the more layers of protection that must be put into place.

The different functionalities of security controls are:
* __Preventive__: intended to avoid an incident from occurring
* __Detective__: Helps identify an incident's activities and potentially an intruder
* __Corrective__: Fixes components or systems after an incident has occurred
* __Deterrent__: Intended to discourage a potential attacker
* __Recovery__: Intended to bring the environment back to regular operations
* __Compensating__: Controls that provide an alternative measure of control that provides similar protection as the original control, but has to be used because it is more affordable or allows specifically required business functionality.

It is not feasible to prevent everything; therefore, what you cannot prevent, you should be able to quickly detect. That's why preventive and detective controls should always be implemented together and should complement each other.

When trying to map the functionality requirement to a control, think of the main reason that control would be put into place.

<p align="center">
  <img src="https://raw.githubusercontent.com/halenai/cissp-notes/master/images/types_of_control.jpg" alt="Types of Control A">
  <img src="https://raw.githubusercontent.com/halenai/cissp-notes/master/images/types_of_control_2.jpg" alt="Types of Control B">
</p>

> Controls should work in harmony to provide healthy, safe, and productive environments.

### Security Frameworks
A security program is a framework made up of many entities: logical, administrative, and physical protection mechanisms; procedures; business processes; and people that all work together to provide a protection level for an environment. Each has an important place in the framework, and if one is missing or incomplete, the whole framework may be affected. The program should work in layers: each layer provides support for the layer above it and protection for the layer below it.

> **What NOT TO DO**: Security through Obscurity

#### Security Program Development
* ISO/IEC 27000 series: International standards on how to develop and maintain an ISMS (Information Security Management System; aka Security Program) developed by ISO and IEC. Serves as industry best practices for the management of security controls in a holistic manner within organizations around the world. The list of standards that makes up this series grows each year. Each standard has a specific focus (such as metrics, governance, auditing, and so on).

#### Enterprise Architecture Development
An architecture is a conceptual construct. It is a tool to help individuals understand a complex item (such as an enterprise) in digestible chunks. An enterprise architecture encompasses the essential and unifying components of an organization. It expresses the enterprise structure (form) and behaviour (function). It embodies the enterprise's components, their relationships to each other, and their relationships to the environment.

> You use the framework as a guideline on how to build and architecture that best fits your company's needs.

An enterprise architecture allows you to not only understand the company from several different views, but also understand how a change that takes place at one level will affect items at other levels. It is used to optimize often fragmented processes (both manual and automated) into an integrated environment that is responsive to change and supportive of the business strategy

* Zachman Framework: Model for the development of enterprise architectures developed by John Zachman. It is a two-dimensional model that uses six basic communication interrogatives (What, How, Where, Who, When, and Why) intersecting with different perspectives (Executives, Business Managers, System Architects, Engineers, Technicians, and Enterprise-wide) to give a holistic understanding of the enterprise. The goal of this framework is to be able to look at the same organization from different viewpoints. Different groups within a company need the same information, but presented in ways that directly relate to their responsibilities. This framework is not security oriented, but it is a good template to work with because it offers direction on how to understand an actual enterprise in a modular fashion.
* TOGAF: Model and methodology for the development of enterprise architectures developed by The Open Group
* DoDAF: US Department of Defense architecture framework that ensures interoperability of systems to meet military mission goals
* MODAF: Architecture framework used mainly in military support missions developed by the British Ministry of Defense
* SABSA model: Model and methodology for the development of information security enterprise architectures

#### Security Controls Development
* COBIT 5: A business framework to allow for IT enterprise management and governance that was developed by ISACA
* NIST SP 800-53: Set of controls to protect US federal systems developed by the National Institute of Standards and Technology
* COSO Internal Control-Integrated Framework: Set of internal corporate controls to help reduce the risk of financial fraud developed by the Committee of Sponsoring Organizations (COSO) of the Treadway Commission

#### Process Management Development
* ITIL: Processess to allow for IT service management developed by the United Kingdom's Office of Government Commerce
* Six Sigma: Business management strategy that can be used to carry out process improvement
* Capability Maturity Model Integration (CMMI) : Organizational development for process improvement developed by Carnegie Mellon University

