# cybersecurity_audit_writeup
Internal Audit for Botium Toys

## Table of Contents
1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Scope](#scope)
4. [Goal](#goal)
5. [Current Assets](#current-assets)
6. [Risk Assessment](#risk-assessment)
7. [Controls Checklist](#controls-checklist)
8. [Compliance Checklist](#compliance-checklist)
    - [Payment Card Industry Data Security Standard (PCI DSS)](#payment-card-industry-data-security-standard-pci-dss)
    - [General Data Protection Regulation (GDPR)](#general-data-protection-regulation-gdpr)
    - [System and Organizations Controls (SOC type 1, SOC type 2)](#system-and-organizations-controls-soc-type-1-soc-type-2)
9. [Recommendations for Improving Botium Toys’ Security Posture](#recommendations-for-improving-botium-toys-security-posture)
10. [Compliance Specific Recommendations](#compliance-specific-recommendations)

# Introduction:
As part of my Google Cybersecurity Professional Certificate, I conducted an internal security audit assessment for Botium Toys, a fictitious toy company.

The purpose of this audit is to evaluate Botium Toys’ security program, ensuring that current business practices are aligned with industry standards and best practices. The audit aims to identify vulnerabilities and provide mitigation recommendations. Additionally, the audit develops a comprehensive strategy to enhance the organization's overall security posture.

# Scenario:
Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy’s online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide. 

The manager of the IT department has decided that an internal IT audit needs to be conducted. She's worried about maintaining compliance and business operations as the company grows without a clear plan. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.).   

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.

**Scope:**
The scope of this audit is defined as the entire security program at Botium Toys. This includes their assets like employee equipment and devices, their internal network, and their systems. You will need to review the assets Botium Toys has and the controls and compliance practices they have in place.

**Goal:**
Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices that need to be implemented to  improve Botium Toys’ security posture.

**Current Assets:**

Assets managed by the IT Department include: 
- On-premises equipment for in-office business needs  
- Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
- Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
- Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
- Internet access
- Internal network
- Data retention and storage
- Legacy system maintenance: end-of-life systems that require human monitoring

**Risk assessment:**

Risk Description:
Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards. 

Control Best Practices:
The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

Risk score
On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

Additional Comments:
The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:

- Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.
- Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database. 
- Access controls pertaining to least privilege and separation of duties have not been implemented.
- The IT department has ensured availability and integrated controls to ensure data integrity.
- The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
- Antivirus software is installed and monitored regularly by the IT department. 
- The IT department has not installed an intrusion detection system (IDS).
- There are no disaster recovery plans currently in place, and the company does not have backups of critical data. 
- The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
- Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters). 
- There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
- While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
- The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.

# Controls Checklist:

|   Yes    |    No    |  Control |
|----------|----------|----------|
|          | x        | Least Privilege  |
|          | x        | Disaster recovery plans   |
|          | x        | Password policies  |
|          | x        | Separation of duties |
| x        |          | Firewall  |
|          | x        | Intrusion detection system (IDS)  |
|          | x        | Backups   |
| x        |          | Antivirus Software   |
|          | x        | Manual monitoring, maintenance, and intervention for legacy systems  |
|          | x        | Encryption  |
|          | x        | Password management system  |
| x        |          | Locks (offices, storefront, warehouse)  |
| x        |          | Closed-circuit television (CCTV) surveillance |
| x        |          | Fire detection/prevention (fire alarm, sprinkler system, etc.) |

# Compliance Checklist:

**Payment Card Industry Data Security Standard (PCI DSS):**

|   Yes    |    No    |  Control |
|----------|----------|----------|
|          | x        | Only authorized users have access to customers’ credit card information.   |
|          | x        | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment.   |
|          | x        | Implement data encryption procedures to better secure credit card transaction touchpoints and data.  |
|          | x        | Adopt secure password management policies. |

**General Data Protection Regulation (GDPR):**

|   Yes    |    No    |  Control |
|----------|----------|----------|
|          | x        | E.U. customers’ data is kept private/secured.  |
|    x     |          | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach.  |
|          | x        | Ensure data is properly classified and inventoried.  |
|    x     |          | Enforce privacy policies, procedures, and processes to properly document and maintain data. |

**System and Organizations Controls (SOC type 1, SOC type 2):**

|   Yes    |    No    |  Control |
|----------|----------|----------|
|          | x        | User access policies are established.  |
|          | x        | Sensitive data (PII/SPII) is confidential/private.  |
|    x     |          | Data integrity ensures the data is consistent, complete, accurate, and has been validated.  |
|          | x        | Data is available to individuals authorized to access it.  |

# Recommendations for Improving Botium Toys’ Security Posture:

To reduce risks to assets and improve Botium Toys’ security posture, several controls and compliance measures need to be implemented or enhanced. The following recommendations should be communicated to stakeholders:

1. **Encryption of Sensitive Data**
   - **Implementation**: Implement robust encryption protocols for all sensitive data, both retained and moved.
   - **Impact**: Protects against data breaches and unauthorized access.

2. **Intrusion Detection System (IDS)**
   - **Implementation**: Implement an IDS to monitor network traffic for suspicious activities and potential security breaches.
   - **Impact**: Allows the ability to detect and respond to threats in real-time.

3. **Disaster Recovery and Backups**
   - **Implementation**: Develop and test a comprehensive disaster recovery plan while maintaining regular, encrypted backups and ensuring they are stored correctly.
   - **Impact**: Minimizes downtime and data loss during and after an incident.

4. **Legacy System Policies**
   - **Implementation**: Establish and enforce policies for managing and securing legacy systems, including regular updates and destruction plans for outdated technology.
   - **Impact**: Reduces vulnerabilities associated with unsupported and outdated systems.

5. **Centralized Password Management/Password Policies**
   - **Implementation**: Utilize a centralized password management system to simplify user experience and enforce improved password complexity requirements.
   - **Impact**: Reduces the likelihood of password-related breaches by ensuring strong, frequently updated passwords.

6. **Least Privilege**
   - **Implementation**: Enforce the principle of least privilege to ensure that users have only the minimum access necessary to perform their job functions.
   - **Impact**: Minimizes potential damage from compromised accounts and improves overall security posture.

7. **Separation of Duties**
   - **Implementation**: Implement separation of duties to prevent conflicts of interest and reduce the risk of insider threats.
   - **Impact**: Ensures accountability and enhances internal controls.

## Compliance Specific Recommendations:

To adhere to U.S. and international regulations, Botium Toys must implement the following compliance measures:

1. **Proper Encryption**
   - **Requirement**: Ensure all sensitive data is encrypted in compliance with standards such as GDPR, PCI DSS, and SOC type 1/type 2.

2. **Separation of Duties**
   - **Requirement**: Implement a clear separation of duties to comply with regulatory requirements and reduce the risk of fraud and error.

3. **Principle of Least Privilege**
   - **Requirement**: Enforce the principle of least privilege to comply with various regulations and best practices.

4. **Asset Identification and Classification**
   - **Requirement**: Properly identify and classify all assets to determine appropriate controls and protections.

By implementing these controls and compliance measures, and holding regular security training for employees, Botium Toys will significantly enhance its security posture, reduce risks to its assets, and ensure adherence to relevant U.S. and international regulations.




