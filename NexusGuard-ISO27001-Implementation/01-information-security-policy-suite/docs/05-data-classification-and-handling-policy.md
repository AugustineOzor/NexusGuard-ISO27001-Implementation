# NexusGuard Technologies Ltd. | Data Classification and Handling Policy | POL-DCH-001

| Field | Detail |
|---|---|
| **Document Title** | Data Classification and Handling Policy |
| **Document ID** | POL-DCH-001 |
| **Version** | 1.0 |
| **Classification** | Internal |
| **Author** | Augustine Ozor, GRC Analyst |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Executive Leadership Team (approval pending) |
| **Approval Date** | Pending (DD/MM/YYYY to be entered on approval) |
| **Effective Date** | Upon approval, and before the first HIPAA client goes live |
| **Next Review Date** | 12 months from approval date |
| **Applicable Regulations** | ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0, UAE NESA |

# Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 0.1 | 13/10/2026 | Augustine Ozor, GRC Analyst | Initial draft, requested by Michael Chen (Head of Compliance) for approval before the first HIPAA client goes live in 30 days. Responds to the DPO's GDPR Article 32 requirement. Replaces the absence of any classification scheme in the 2021 policy. |
| 1.0 | Pending | Executive Leadership Team | Approval and publication. |

# 1. Purpose

This Data Classification and Handling Policy (the "Policy") tells everyone at NexusGuard Technologies Ltd. ("NexusGuard") how to decide how sensitive a piece of information is, how to label it, and how to store, send, keep and destroy it. It makes sure information gets the protection its sensitivity and legal status demand, and no more or less.

NexusGuard handles four fundamentally different kinds of data: patient health records (PHI), payment card data, employee personal data, and proprietary source code. Each carries different regulatory duties and risks. The 2021 Information Security Policy had no classification scheme at all, and staff have had no formal guidance. This Policy fills that gap, supports the "appropriate technical and organizational measures" required by GDPR Article 32, and meets HIPAA and PCI DSS expectations ahead of the first HIPAA client go-live.

This Policy shall:

- define a four-tier scheme (Public, Internal, Confidential, Restricted) with handling, labeling, storage, transmission and disposal rules for each tier;
- assign responsibility for classifying data and set a process to reclassify it;
- set specific rules for PHI, payment card data, personal data and source code;
- control cross-border transfers of data; and
- set retention and disposal requirements.

# 2. Scope

This Policy applies to all information owned, processed or held by NexusGuard or on its behalf, in any form (electronic, paper, verbal, audio or video) and in any location, including on-premises systems, cloud services, endpoints, backups and removable media. It applies to all employees, contractors, consultants, temporary staff and third parties, in Dubai, London and New York, and to **PayStream Analytics**. It covers client data that NexusGuard holds as a processor or business associate, as well as NexusGuard's own data.

Where a law, regulation or client contract demands a higher level of protection than this Policy, the stricter requirement shall apply.

# 3. Definitions

| Term | Definition |
|---|---|
| Data owner | The manager accountable for a set of information, who decides its classification and who may access it. |
| Data custodian | The team that operates the systems holding the data (IT, Engineering, DBAs, cloud operations) and applies the required controls. |
| Classification | The tier (Public, Internal, Confidential or Restricted) assigned to information based on its sensitivity and legal status. |
| Label | A visible or technical marking showing the classification of a document, file, message, system or medium. |
| PHI | Protected health information under HIPAA: individually identifiable health information held by NexusGuard for healthcare clients. |
| Cardholder data (CHD) | The primary account number (PAN) and, if stored with it, the cardholder name, expiry date and service code. |
| Sensitive authentication data (SAD) | Full track data, card verification codes and PINs. SAD shall never be stored after authorization. |
| Personal data | Information relating to an identified or identifiable person (GDPR Art. 4). **Special category data** (for example health, biometric and union membership data) needs extra protection. |
| Employee PII | Personal data about employees, contractors and applicants, such as identity, contact, payroll, performance and HR records. |
| Source code | Software code, scripts, configuration and related design documents developed by or for NexusGuard. |
| Reclassification | A change to the tier assigned to information. Moving to a lower tier is **declassification**. |
| De-identification | Removing identifiers so data can no longer be linked to a person, to the standard in HIPAA 164.514(b) or equivalent. |
| Cross-border transfer | Moving, or giving access to, data in a different country from where it is held or collected. |
| Retention schedule | The approved list of how long each category of record is kept, and how it is destroyed. |
| Legal hold | An instruction from Legal to preserve information that would otherwise be destroyed. |
| shall / should / may | **shall** denotes a mandatory requirement; **should** a recommendation; **may** an optional action. |

# 4. Roles and Responsibilities

| Role | Responsibilities |
|---|---|
| Executive Leadership Team | Shall approve this Policy and resource its implementation. |
| CISO (Policy Owner) | Shall own this Policy, set technical controls, approve reclassification of Restricted data and exceptions, and report on compliance. |
| Data Protection Officer (DPO) | Shall advise on personal data classification, retention and cross-border transfers, and approve transfer mechanisms with Legal. |
| Head of Compliance | Shall map this Policy to HIPAA, PCI DSS, GDPR and ISO 27001, and audit classification and handling. |
| Data owners | Shall classify their data, approve access, review classifications annually and approve reclassification (Section 5.7). |
| Data custodians (IT, Engineering, DBAs) | Shall implement labeling, encryption, access control, backup, retention and disposal controls for the data they host. |
| HR Director | Shall own employee personal data and its retention. |
| CTO and Engineering leads | Shall own source code and client platform data. PayStream's Head of Engineering owns the PayStream cardholder data environment. |
| Legal | Shall advise on contracts, retention periods, legal holds, export controls and cross-border transfers. |
| Security Operations | Shall run DLP, discovery scans and monitoring, and investigate mishandling. |
| All users | Shall apply labels, handle data according to its tier, ask when unsure, and report mishandling within 1 hour. |
| Third parties | Shall handle NexusGuard and client data to the standard in their contracts, which shall reflect this Policy. |

# 5. Policy Statements

## 5.1 Classification Principles

**5.1.1** All information shall be classified into one of four tiers: Public, Internal, Confidential or Restricted. The tier shall reflect the sensitivity of the content, not its format or location.

**5.1.2** Information shall be classified at creation or receipt. Information that has not been classified shall be treated as Internal, unless it meets the criteria for a higher tier, in which case the higher tier applies whether or not it is labeled.

**5.1.3** Where a collection holds information of mixed tiers, the whole collection shall be handled at the highest tier present. Combining data can raise its tier.

**5.1.4** Information received from clients or third parties shall be classified according to its content and the contract. A contract that requires stricter handling prevails.

**5.1.5** When in doubt, users shall classify one tier higher and ask the data owner or the DPO.

**5.1.6** Classification is separate from business criticality in the Information Asset Register (IAR). Each asset in the IAR shall record both its data classification and criticality. As a guide, Restricted data usually sits in Critical systems, but each is assessed on its own.

## 5.2 Classification Responsibilities

**5.2.1** Data owners shall classify the information they own, using Table 1 as the default. Authors and users who create or receive information shall apply the owner's classification or, for new content, the default tier.

**5.2.2** Data owners shall record the classification of each system and data store in the IAR and review it at least annually.

**Table 1: Who Classifies What**

| Data | Data owner | Default tier | May reclassify |
|---|---|---|---|
| Client PHI | CTO (client platform data) | Restricted | CISO and DPO |
| Payment card data (PAN, SAD) | CFO; PayStream Head of Engineering for the PayStream environment | Restricted | CISO |
| Employee PII | HR Director | Confidential. Special category data, government ID and bank details: Restricted | HR Director and DPO |
| Source code | CTO and Engineering leads | Confidential. Restricted if it contains secrets or keys | CTO |
| Credentials, keys and secrets | CISO | Restricted | CISO |
| Client contracts and pricing | Legal and Sales Director | Confidential | Legal |
| Security reports, audit reports, network diagrams | CISO | Confidential | CISO |
| Marketing and published content | Marketing and Communications | Public once approved | Head of Marketing |
| General internal documents | Author's line manager | Internal | Data owner |

## 5.3 The Four-Tier Scheme

**5.3.1** The tiers, definitions and minimum handling rules are set out below. The definitions of each tier follow the classification guide in the Information Asset Register. The requirements are minimums, and a stricter control may be applied.

### Tier 1: Public

| Field | Detail |
|---|---|
| **Definition** | Approved for unrestricted public release. Disclosure causes no harm. |
| **NexusGuard examples** | Website content, published datasheets, press releases, job adverts, published blog posts, public documentation. |
| **Handling** | Release only after approval by Marketing and Communications. Control write access so content cannot be altered. Remove author names, comments and tracked changes before release. |
| **Labeling** | No label needed. A "Public" footer is recommended before release. |
| **Storage** | Any approved NexusGuard system, with write access restricted. |
| **Transmission** | No restriction. |
| **Disposal** | Normal deletion or recycling. |

### Tier 2: Internal

| Field | Detail |
|---|---|
| **Definition** | For NexusGuard personnel and authorized third parties. Unauthorized disclosure causes limited harm. |
| **NexusGuard examples** | Internal policies and procedures, org charts, staff directory, meeting notes, project plans without client details, intranet content, general IT guidance. |
| **Handling** | Share only within NexusGuard and with authorized contractors. Do not post on social media or place in personal accounts. Access through single sign-on. This is the default tier. |
| **Labeling** | "Internal" label recommended. Unlabeled information is treated as Internal. |
| **Storage** | Approved NexusGuard systems only (Microsoft 365 and approved SaaS). Not on personal devices or accounts. |
| **Transmission** | Company email and approved collaboration tools. External sharing only to authorized recipients with a business need. No public links. |
| **Disposal** | Delete from systems. Paper goes into secure shred bins, not general waste. |

### Tier 3: Confidential

| Field | Detail |
|---|---|
| **Definition** | Sensitive business, customer, security or employee information requiring controlled access. Disclosure causes serious harm. |
| **NexusGuard examples** | Client contracts and pricing, pre-release financials, employee PII (payroll, performance, HR records), source code, security assessments, network diagrams, vulnerability scans, audit reports, board papers, incident reports, client project data that contains no PHI or card data. |
| **Handling** | Need-to-know access approved by the data owner (ACP 5.1.2). Do not discuss in public places. Do not copy to personal devices, accounts or unapproved AI tools. Share externally only under a contract or NDA. |
| **Labeling** | Mandatory. "NexusGuard Confidential" in the header or footer, a Microsoft 365 sensitivity label, an email subject tag [CONFIDENTIAL], and a classification tag on cloud resources and repositories. |
| **Storage** | Approved systems with access control and AES-256 encryption at rest (ISP 5.6.4). Laptops use full-disk encryption. Removable media only under an approved exception (ISP 5.7.7). Paper locked away when not in use. |
| **Transmission** | Encrypted with TLS 1.2 or higher. Email only to authorized recipients. External sharing through encrypted email or a secure share with named access and an expiry date. No public or anonymous links. Check recipients before sending. |
| **Disposal** | Secure deletion. Media sanitized to NIST SP 800-88 with a certificate of destruction. Paper cross-cut shredded (DIN 66399 level P-4 or higher). |

### Tier 4: Restricted

| Field | Detail |
|---|---|
| **Definition** | Highly sensitive or regulated information requiring the strongest access and handling controls. Disclosure causes severe harm and legal consequences. |
| **NexusGuard examples** | PHI held for healthcare clients; payment card data (PAN and SAD) in the PayStream cardholder data environment and the finance system; special category employee data (health, biometric, union membership), government ID and bank account numbers; credentials, API keys, private keys and secrets; source code that contains secrets; forensic images from investigations. |
| **Handling** | Named individuals only, approved by the data owner and CISO delegate, with MFA and logged access (ACP 5.4.7, 5.8). Minimum necessary use. Never on personal devices, personal email or cloud, removable media (without exception) or unapproved AI tools. Production Restricted data is not used in non-production unless masked (ISP 5.9.8). DLP monitors and blocks transfers. |
| **Labeling** | Mandatory. "NexusGuard Restricted" on every file and medium, an email subject tag [RESTRICTED], and cloud and database tags showing the tier and the regulation (PHI, PCI, PII). Physical media carries a red label and is logged in a register. |
| **Storage** | Only in systems approved for Restricted data, such as the segmented PHI network and the CDE (ISP 5.4.3). AES-256 encryption with keys in the vault or HSM (ISP 5.6.6). Encrypted backups. Region as set by client contract. No local copies. No printing except where approved. |
| **Transmission** | Only over encrypted channels between approved systems (TLS 1.2 or higher, TLS 1.3 preferred), by SFTP, API or private connectivity. Never by chat, SMS or unencrypted email. PHI and PAN shall not appear in email subjects or bodies. Recipients verified. Transfers logged. |
| **Disposal** | Cryptographic erase, or NIST SP 800-88 purge or destroy, with a certificate retained. Paper cross-cut shredded to DIN 66399 level P-5, or witnessed destruction. Backups included. Disposal logged and confirmed by the custodian. |

## 5.4 Labeling and Marking

**5.4.1** Confidential and Restricted information shall be labeled as set out in Section 5.3. Public and Internal labels are recommended but not mandatory.

**5.4.2** Microsoft 365 sensitivity labels (or an equivalent tool) shall be used for documents and email so that labels travel with the file and drive DLP and encryption rules. IT shall make the labels available to all users before go-live.

**5.4.3** Cloud resources, databases, storage buckets and repositories shall carry a classification tag, and a regulation tag (PHI, PCI, PII) where relevant. IAM and Security shall check tags during access reviews.

**5.4.4** Printed documents shall show the classification on every page. Removable media, where approved, shall carry a physical label and be recorded in the media register.

**5.4.5** Labels shall not be removed or lowered except through reclassification under Section 5.7. Where a label is missing or wrong, a user who notices it shall tell the data owner.

**5.4.6** The label shall not itself reveal sensitive information. Use "Restricted", not "Restricted: Client X patient data".

## 5.5 Handling Rules for Specific Data Types

**5.5.1** The rules in Table 2 are in addition to the tier rules in Section 5.3.

**Table 2: Summary of Data-Type Rules**

| Data type | Tier | Governing requirements | Key rules |
|---|---|---|---|
| PHI | Restricted | HIPAA Security and Privacy Rules; client BAAs | Minimum necessary; BAA before access; no personal devices; masked or de-identified in non-production |
| Payment card data | Restricted | PCI DSS v4.0 | PAN unreadable; no SAD after authorization; CDE segmentation; masked display |
| Employee PII | Confidential (Restricted for special category data) | GDPR / UK GDPR; UAE data law; employment law | HR systems only; need-to-know; retention schedule; data subject rights |
| Source code | Confidential (Restricted with secrets) | ISP; client contracts; licenses | Approved repository only; no secrets; code review; no unapproved AI tools |

### PHI (HIPAA)

**5.5.2** PHI shall be classified Restricted, accessed only for purposes permitted by HIPAA and the client's Business Associate Agreement (BAA), and limited to the minimum necessary for the task.

**5.5.3** PHI shall not be disclosed to any third party, including a subcontractor, unless a BAA is in place. PHI shall not be stored or sent through personal devices, personal accounts, removable media or unapproved AI tools.

**5.5.4** PHI shall not be placed in email subject lines, chat, tickets or logs. Where it must appear in a ticket or log, it shall be masked.

**5.5.5** PHI shall not be used in development, test or training unless de-identified under HIPAA 164.514(b) or masked and approved by the data owner and CISO.

**5.5.6** Access to PHI shall be logged and reviewed at least monthly, and quarterly access reviews apply (ACP 5.7.1, 5.8.5). Suspected unauthorized access or disclosure shall be reported within 1 hour and handled under ISP 5.12.

**5.5.7** Records required by HIPAA shall be kept for six years, and PHI shall be returned or destroyed at the end of a client contract as the BAA requires.

### Payment card data (PCI DSS)

**5.5.8** Cardholder data shall be classified Restricted and stored only where a documented business need exists. Systems that store, process or transmit it form the CDE and shall be segmented from other networks.

**5.5.9** Sensitive authentication data shall never be stored after authorization, even if encrypted.

**5.5.10** PAN shall be unreadable wherever stored, by strong cryptography, truncation, tokenization or keyed hashing. Where displayed, it shall be masked so that only people with a business need see more than the first six and last four digits.

**5.5.11** PAN shall not be sent through email, chat or other end-user messaging unless strong cryptography protects it. PAN shall not be copied to endpoints, removable media or non-production systems.

**5.5.12** Cryptographic keys protecting card data shall be managed under ISP 5.6.6, with split knowledge and dual control. Security shall run discovery scans at least quarterly to find unprotected PAN, and any found shall be securely deleted or protected. PCI scope shall be confirmed at least annually.

### Personal data (GDPR, UK GDPR and UAE law) and employee PII

**5.5.13** Personal data shall be processed only with a documented lawful basis (GDPR Art. 6, and Art. 9 for special category data), for specified purposes, minimized to what is necessary, kept accurate and kept no longer than needed. The DPO shall maintain records of processing (Art. 30).

**5.5.14** Employee PII shall be classified Confidential and held in HR systems only. Special category data, government ID numbers and bank details shall be classified Restricted. Access is limited to HR and to managers with a need to know.

**5.5.15** Personal data shall be protected by pseudonymization and encryption where appropriate (Art. 32(1)(a)). A data protection impact assessment shall be completed before any high-risk processing starts (Art. 35).

**5.5.16** Data subject requests shall be recorded and answered within one month under the DPO's direction. Processors shall be bound by a data processing agreement (Art. 28).

**5.5.17** Personal data breaches shall be reported to the DPO and Security within 1 hour of discovery so that notification within 72 hours can be assessed (Art. 33).

### Source code

**5.5.18** Source code shall be classified Confidential and held only in the approved repository platform under a company-managed organization, with single sign-on, MFA, branch protection and code review.

**5.5.19** Source code shall not be stored in personal repositories, personal email or cloud storage, or entered into unapproved AI tools. Local clones shall sit on encrypted, managed devices.

**5.5.20** Secrets, keys and credentials shall never be in code (ISP 5.6.6). Repositories shall be scanned for secrets, and a repository that holds a secret shall be handled as Restricted until it is removed and the secret rotated.

**5.5.21** Production PHI and card data shall never be placed in repositories or test data. Sharing code outside NexusGuard requires data owner approval and a contract or NDA. Use of open-source code shall follow license terms.

## 5.6 Storage, Transmission and Disposal

**5.6.1** Information shall be stored only in systems approved for its tier. IT shall maintain a register of approved storage locations for each tier, and Restricted data shall be held only where ISP 5.4.3 allows.

**5.6.2** Removable media is blocked by default (ISP 5.7.7). Where an exception is approved, the device shall be company-issued, encrypted and registered, and the data owner shall confirm the classification.

**5.6.3** Information shall be transmitted using the channels set for its tier. Users shall check recipients, attachments and any sharing links before sending.

**5.6.4** Data shall be encrypted at rest and in transit as set in Section 5.3, using keys managed under ISP 5.6.6.

**5.6.5** Disposal shall use the method for the tier. Data custodians shall delete cloud data by deleting or destroying the encryption key (cryptographic erase) where the platform supports it, and shall confirm that backups and replicas have expired or been deleted.

**5.6.6** Third parties that hold NexusGuard or client data shall return or destroy it at the end of the contract and provide a certificate of destruction.

## 5.7 Reclassification and Declassification

**5.7.1** Any user may ask a data owner to reclassify information. Any user who finds information at a lower tier than its content warrants shall handle it at the higher tier at once and tell the data owner.

**5.7.2** The data owner shall decide a request within 5 business days. Raising the tier takes effect immediately. Lowering a tier shall be approved as shown in Table 3.

**5.7.3** Every approved change shall be recorded in ITSM, with the reason and approver. All copies shall be relabeled, and the IAR updated if a system or data store is affected.

**5.7.4** Data owners shall review classifications when the purpose, content or legal status of the data changes, when it is aggregated or released, when a contract ends, and at least annually for Confidential and Restricted data.

**Table 3: Reclassification Approvals**

| Change | Approver | Conditions |
|---|---|---|
| Any increase in tier | Data owner (any user may apply a higher tier at once) | Notify the data owner; record in ITSM |
| Restricted to Confidential | Data owner and CISO; DPO where personal data is involved | Verified de-identification or removal of regulated elements |
| Confidential to Internal | Data owner | Written reason; Legal if a contract or NDA applies |
| Internal to Public | Data owner and Marketing and Communications | Content approved for release; metadata removed |

## 5.8 Cross-Border Data Transfers

**5.8.1** Data shall not be transferred to, or accessed from, another country except as set out in Table 4. The DPO and Legal shall approve any new transfer route, and a record of approved transfers shall be kept.

**5.8.2** Personal data of EU and UK data subjects shall leave the EEA or the UK only under a lawful mechanism (adequacy decision, standard contractual clauses, the UK IDTA or Addendum, or other safeguards), after a transfer risk assessment.

**5.8.3** PHI and other client data shall stay in the regions agreed in the client contract and BAA. Remote access from other countries needs approval (ACP 5.5.6).

**5.8.4** Sharing data between NexusGuard entities, including PayStream Analytics, shall follow an intra-group data transfer agreement and shall be limited to defined purposes.

**5.8.5** Sub-processors and cloud regions shall be checked for location before use, and data shall be encrypted in transit and at rest for all transfers.

**Table 4: Cross-Border Transfer Restrictions**

| Data | Restriction | Mechanism | Approver |
|---|---|---|---|
| PHI and client data | Stay in contractual regions; no offshore access unless the contract allows | BAA and client written approval | CISO, Legal and client |
| Cardholder data | Handled only in the CDE; moved only over approved encrypted channels | PCI scope review | CISO |
| EU and UK personal data | Outside the EEA or UK only with safeguards | Adequacy, SCCs or UK IDTA, plus transfer risk assessment | DPO and Legal |
| UAE and DIFC personal data | Transfer conditions of the applicable UAE or DIFC law | Adequacy or approved safeguards | DPO and Legal |
| Employee PII between entities | Only for HR purposes | Intra-group data transfer agreement | HR Director and DPO |
| Source code | No storage in unapproved regions; check export controls and client terms | Legal review | CTO and Legal |

## 5.9 Retention and Disposal

**5.9.1** Information shall be kept only as long as there is a business, legal or contractual need, and then destroyed under Table 5. Legal shall maintain the retention schedule and validate the periods for each jurisdiction.

**5.9.2** Retention periods shall not be extended without a legal hold or documented reason. When a legal hold applies, destruction shall stop until Legal lifts it.

**5.9.3** Destruction shall follow the disposal rules for the tier, and custodians shall keep a disposal log and certificates. Data owners shall review stored data against the schedule at least annually.

**Table 5: Retention Schedule (to be validated by Legal)**

| Data | Retention | Basis | Disposal on expiry |
|---|---|---|---|
| PHI held for clients | As the client contract or BAA states; return or destroy on termination | HIPAA; BAA | Cryptographic erase or NIST SP 800-88; certificate |
| HIPAA compliance records | 6 years | HIPAA 164.316(b)(2) | Secure deletion |
| Cardholder data | Only as long as a documented business need; SAD not after authorization | PCI DSS Req. 3 | Cryptographic erase; quarterly check for excess data |
| Employee PII | Employment plus the period in the HR schedule, subject to local law | Employment and data protection law | Secure deletion; paper shredded |
| Unsuccessful applicant data | No longer than 6 months unless consent is given | Data protection law | Secure deletion |
| Security and access logs | 12 months (3 months online) | ISP 5.9.4; ACP 5.8.3 | Automated deletion |
| Access requests and reviews; incident records; training records | 6 years | ACP 5.7.7; ISP 5.12.7, 5.14.6 | Secure deletion |
| Source code and repositories | Life of the product, then archive per contract; delete forks and clones | Contract; IP policy | Delete; remove from backups on expiry |
| Contracts and financial records | Per the Legal retention schedule | Law and contract | Secure deletion; paper shredded |

## 5.10 Monitoring, Incidents and Training

**5.10.1** DLP rules shall be built on classification labels and data patterns (PHI, PAN, national IDs, secrets) and shall monitor and block unauthorized transfers (ISP 5.6.7).

**5.10.2** Misclassification, mishandling, loss or disclosure of Confidential or Restricted data shall be reported within 1 hour of discovery and handled under ISP 5.12. Reports made in good faith shall not lead to retaliation.

**5.10.3** All staff shall complete data handling training on joining and every year. Staff who handle PHI, card data or personal data shall also complete role-based training (ISP 5.14.4).

**5.10.4** Compliance shall audit classification and handling at least annually, sampling systems, repositories and shared drives, and report findings to the CISO.

## 5.11 Implementation Before Go-Live

**5.11.1** Before the first HIPAA client goes live, the following shall be completed and evidenced to the Head of Compliance: classification recorded for every asset in the IAR; Microsoft 365 sensitivity labels and DLP rules deployed for PHI and PAN; a discovery scan to locate PHI and cardholder data outside approved systems; data handling training delivered to all staff with access to client data; and the approved storage register published.

**5.11.2** PayStream Analytics shall classify its assets and apply this Policy within 90 days of the Effective Date.

# 6. Compliance

This Policy supports the requirements in Table 6. References are paraphrased pointers; the source text of each requirement prevails.

**Table 6: Compliance Basis**

| Regime | Key provisions supported | Policy sections |
|---|---|---|
| ISO/IEC 27001:2022 | A.5.10 acceptable use; A.5.12 classification; A.5.13 labelling; A.5.14 information transfer; A.5.33 protection of records; A.5.34 privacy and PII; A.7.10 storage media; A.7.14 disposal of equipment; A.8.10 information deletion; A.8.11 data masking; A.8.12 data leakage prevention; A.8.24 cryptography | 5.1 to 5.10 |
| HIPAA | 164.502(b) and 164.514(d) minimum necessary; 164.514(b) de-identification; 164.308(b) business associates; 164.310(d) device and media controls; 164.312(a)(2)(iv) encryption; 164.312(e) transmission security; 164.316(b)(2) six-year retention | 5.3, 5.5, 5.6, 5.9 |
| PCI DSS v4.0 | Req. 3 (retention, SAD, masking, unreadable PAN, keys); Req. 4 (PAN in transit and messaging); Req. 9.4 media; Req. 12.5 scope | 5.3, 5.5, 5.6 |
| GDPR / UK GDPR | Art. 5 principles; Art. 6 and 9 lawful basis; Art. 25 by design; Art. 28 processors; Art. 30 records; Art. 32 security including encryption and pseudonymization; Art. 33 breach notification; Art. 35 DPIA; Art. 44 to 49 transfers | 5.5, 5.8, 5.9 |
| NIST CSF 2.0 | ID.AM-05 asset prioritization by classification; ID.AM-07 data inventories; PR.DS-01, PR.DS-02 data at rest and in transit | 5.1 to 5.6 |
| UAE NESA and UAE law | Asset management and information classification control families; UAE personal data protection law and DIFC data protection law | 5.1 to 5.9 |

# 7. Enforcement and Sanctions

**7.1** Compliance with this Policy is mandatory. Violations shall be handled under the HR disciplinary procedure and the tiered sanctions in the Acceptable Use Policy, up to and including termination, in line with applicable employment law.

**7.2** Serious violations include: exposing or sending Restricted data to unauthorized people or accounts; storing PHI or card data outside approved systems; removing or lowering labels to avoid controls; and concealing mishandling.

**7.3** Data owners and managers who fail to classify data or to correct known mishandling are accountable and may face disciplinary action. Third parties face the remedies in their contracts.

# 8. Exceptions

**8.1** Exceptions shall be requested through the Policy Exception Management Process and shall be formally requested in writing, with a business justification, a risk assessment and compensating controls.

**8.2** Exceptions shall be approved by the CISO for Low and Medium risk and by the Executive Leadership Team for High or Critical risk, shall be time-limited to no more than 12 months, and shall be recorded in the exception register.

**8.3** No exception shall be granted to a requirement imposed by HIPAA, PCI DSS, GDPR or another law or client contract unless Legal confirms in writing that it is permitted.

# 9. Related Documents

| Document | ID | Type |
|---|---|---|
| Information Security Policy | POL-ISP-001 | Policy |
| Acceptable Use Policy | POL-AUP-001 | Policy |
| Access Control Policy | POL-ACC-001 | Policy |
| Privacy and Data Protection Policy | POL-PRV-001 | Policy |
| Incident Response Policy and Plan | POL-IRP-001 | Policy |
| Encryption and Key Management Standard | STD-CRY-001 | Standard |
| Removable Media Standard | STD-RMS-001 | Standard |
| Information Asset Register | IAR-001 | Register |
| Records Retention Schedule | To be confirmed by Legal | Schedule |
| Policy Exception Management Process | PRC-GRC-001 | Procedure |
| Data Handling Quick Reference Guide | GDL-DCH-001 | Guideline |

_Document IDs are proposed identifiers under the policy framework. Confirm them against the document register._

# 10. Review

This policy shall be reviewed annually or when significant changes occur. The Policy Owner initiates the review.

**10.1** The CISO shall also review this Policy after a significant data incident, a change in law or client requirements, an acquisition, or a major change to systems that hold Restricted data.

**10.2** The approved version shall be published in the controlled document repository, communicated to all personnel, and acknowledged within 30 days. Superseded versions shall be archived for at least six years.
