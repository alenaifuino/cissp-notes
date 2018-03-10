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
