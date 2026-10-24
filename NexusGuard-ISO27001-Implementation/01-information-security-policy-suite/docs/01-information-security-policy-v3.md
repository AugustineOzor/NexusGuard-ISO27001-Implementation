# NexusGuard Technologies Ltd. | Information Security Policy | POL-ISP-001

| Field | Detail |
|---|---|
| **Document Title** | Information Security Policy |
| **Document ID** | POL-ISP-001 |
| **Version** | 3.0 |
| **Classification** | Internal |
| **Author** | Augustine Ozor, GRC Analyst |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Executive Leadership Team and Board of Directors (approval pending) |
| **Approval Date** | Pending (DD/MM/YYYY to be entered on approval) |
| **Effective Date** | Upon approval |
| **Next Review Date** | 12 months from approval date |
| **Applicable Regulations** | ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0, UAE NESA |

# Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 15/01/2021 | Ahmed Hassan, IT Manager | Original Information Security Policy, approved by the IT Manager only. Superseded by v3.0. |
| 3.0 (draft) | 11/10/2026 | Augustine Ozor, GRC Analyst | Complete rewrite commissioned by Michael Chen. Replaces v1.0 in full. Addresses all gaps recorded in the Policy Gap Analysis Report (RPT-ISP-001). |
| 3.0 | Pending | Executive Leadership Team / Board | Approval and publication. |

# 1. Purpose

This Information Security Policy (the "Policy") is the overarching policy of the NexusGuard Technologies Ltd. ("NexusGuard") Information Security Management System (ISMS). It sets out management's direction and the mandatory requirements for protecting the confidentiality, integrity and availability of NexusGuard's information assets, of the information that clients entrust to NexusGuard (including protected health information and payment card data), and of the systems that process it.

Version 1.0 of this Policy (January 2021) was written for a company of about 200 employees operating from one office, with no cloud infrastructure and no healthcare clients. NexusGuard now operates from Dubai, London and New York, runs workloads in the cloud, serves healthcare and payment-sensitive clients, and has acquired PayStream Analytics (2025). This version replaces v1.0 in full.

This Policy shall:

- establish the framework through which NexusGuard meets the requirements of ISO/IEC 27001:2022 (Clause 5.2), HIPAA, PCI DSS v4.0, GDPR / UK GDPR, the NIST Cybersecurity Framework 2.0 and UAE NESA;
- set measurable information security objectives that support NexusGuard's business strategy;
- assign clear and enforceable accountability for information security at every level of the organization;
- define the policy framework (policies, standards, procedures and guidelines) that supports it; and
- mandate baseline requirements across all security domains: governance, risk, access, data, physical, operations, cloud, third parties, incident response, continuity and awareness.

# 2. Scope

This Policy applies to the following, without exception other than through the process in Section 8.

| Dimension | Coverage |
|---|---|
| Organizational entities | NexusGuard Technologies Ltd., including its Dubai headquarters and its London and New York offices; **PayStream Analytics** (acquired 2025) and its personnel, systems and data; and any future subsidiary, affiliate or acquired business from the date it joins the group. |
| People | All employees (permanent, fixed-term and part-time), contractors, consultants, temporary staff, interns, directors with access to information, and **third parties** (suppliers, managed service providers, cloud providers, partners and their personnel) that access NexusGuard or client information or systems. |
| Information | All information in any form (electronic, paper or verbal), including protected health information (PHI), personal data, cardholder data, client data, source code, financial, HR and strategic information. |
| Systems and technology | All on-premises systems, data centers and co-location, **cloud infrastructure and services** (IaaS, PaaS and SaaS, including Microsoft 365), networks, endpoints, mobile devices, personally owned devices used for work, development, test and production environments, and AI tools. |
| Facilities and locations | All offices, data centers, home and remote working locations, and business travel. |

Where a law, regulation or client contract requires a stricter control than this Policy, the stricter requirement shall apply. PayStream Analytics shall apply the stricter of its existing policies and this Policy until its controls are fully aligned, as set out in clause 5.11.6.

# 3. Definitions

| Term | Definition |
|---|---|
| Availability | The property of being accessible and usable on demand by an authorized party. |
| Confidentiality | The property that information is not made available or disclosed to unauthorized individuals, entities or processes. |
| Integrity | The property of accuracy and completeness of information and processing. |
| Information asset | Any information, and any system, device, service or facility that creates, stores, processes or transmits it, that has value to NexusGuard or its clients. |
| ISMS | The Information Security Management System: the policies, processes, people and controls used to manage information security risk. |
| PHI | Protected health information as defined under HIPAA: individually identifiable health information held or transmitted by a covered entity or business associate. |
| Personal data | Any information relating to an identified or identifiable natural person (GDPR Art. 4). Special category data (for example health data) requires additional protection. |
| Cardholder data (CHD) | The primary account number (PAN) and, where stored with it, cardholder name, expiry date and service code. Sensitive authentication data must never be stored after authorization. |
| CDE | Cardholder data environment: the people, processes and technology that store, process or transmit cardholder data or sensitive authentication data. |
| MFA | Multi-factor authentication: authentication using two or more independent factors (something known, held or inherent). |
| Privileged account | An account with elevated rights over systems, applications, security tooling, cloud tenants or data (for example administrator, root, global admin and service accounts). |
| Third party | Any external organization or individual that provides services to, or has access to the information or systems of, NexusGuard or its clients. |
| Information security incident | One or more unwanted or unexpected information security events that have a significant probability of compromising operations or threatening information security. |
| Personal data breach | A breach of security leading to the accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or access to, personal data. |
| Risk | The effect of uncertainty on objectives, expressed as a combination of the likelihood of an event and its impact. |
| shall / should / may | **shall** denotes a mandatory requirement; **should** a recommendation that may be departed from only with documented justification; **may** an optional action. |

# 4. Roles and Responsibilities

Information security is the responsibility of everyone at NexusGuard. The following roles carry specific accountabilities.

| Role | Responsibilities |
|---|---|
| Board of Directors / Executive Leadership Team | Shall approve this Policy and the ISMS objectives; provide adequate resources; accept risks above the defined appetite; and review ISMS performance at least annually. |
| Chief Information Security Officer (CISO) (Policy Owner) | Shall own this Policy and the ISMS; lead the security team; maintain the risk methodology, incident response plan and supporting standards; report security KPIs and significant risks to the Executive Leadership Team quarterly; and approve security exceptions within delegated authority. |
| Information Security Governance Committee | Shall oversee implementation of the ISMS, review risks, incidents and audit findings, and approve supporting policies and standards before release. |
| Security Operations Team | Shall monitor, detect, triage and respond to security events 24x7 for critical systems and operate the vulnerability management and logging programs. |
| Data Protection Officer (DPO) / Privacy Lead | Shall advise on GDPR, UK GDPR, UAE and other privacy obligations; oversee DPIAs and data subject requests; and decide, with Legal and the CISO, on personal data breach notifications. |
| Legal and Compliance (GRC) | Shall identify applicable legal, regulatory and contractual requirements; maintain the compliance register; support regulator and client engagement; and track audit findings to closure. |
| IT Department | Shall implement and operate technical controls in line with security standards; manage systems, identity, endpoints, cloud platforms and backups; and remediate vulnerabilities within the required timeframes. |
| HR Department | Shall carry out pre-employment screening; include security terms in employment contracts; notify IT of joiners, movers and leavers in time to meet access deadlines; deliver training records; and administer disciplinary action under Section 7. |
| Line Managers | Shall ensure their teams know and follow this Policy; approve access appropriate to roles; review team access periodically; and report incidents and non-compliance. |
| System and Data Owners | Shall classify information; approve and review access; accept risk for their assets; and ensure controls are applied to their systems. |
| All employees | Shall comply with this Policy and related documents; complete mandatory training; protect credentials and devices; and report suspected incidents immediately. |
| Contractors and temporary staff | Shall comply with this Policy and applicable contract terms; use only approved systems; and return or securely destroy NexusGuard information and assets at the end of their engagement. |
| Third parties and suppliers | Shall meet the security, privacy and breach-notification obligations in their contracts; give NexusGuard assurance evidence on request; and flow requirements down to their subcontractors. |
| PayStream Analytics security lead | Shall act as the accountable point of contact for aligning PayStream controls with this Policy and report progress to the CISO. |
| Internal Audit / independent reviewer | Shall independently assess ISMS conformity and effectiveness at least annually. |

# 5. Policy Statements

## 5.1 Information Security Governance and Objectives

**5.1.1** The Executive Leadership Team shall demonstrate leadership of information security by approving this Policy, assigning roles and authority, providing resources, and reviewing ISMS performance at least annually (management review).

**5.1.2** NexusGuard shall establish, implement, maintain and continually improve an ISMS aligned with ISO/IEC 27001:2022 and structured using the six functions of the NIST Cybersecurity Framework 2.0 (Govern, Identify, Protect, Detect, Respond, Recover).

**5.1.3** Security decisions shall be risk-based and aligned with NexusGuard's business strategy: protecting client trust in healthcare and payment services, supporting international growth, and securely integrating acquired businesses.

**5.1.4** The objectives in Table 1 shall be measured, reviewed at least annually, and reported by the CISO to the Executive Leadership Team each quarter. Targets may be raised but shall not be lowered without Executive Leadership Team approval.

**Table 1: Information Security Objectives**

| # | Objective | Measure and target | Business alignment |
|---|---|---|---|
| O1 | Protect confidentiality of regulated data | Zero confirmed breaches of PHI, cardholder data or special category personal data caused by a control failure, per year. | Client trust in healthcare and payment services |
| O2 | Maintain availability of client-facing services | 99.9% annual availability; RTO and RPO met in 100% of continuity tests. | Contractual SLAs and retention of enterprise clients |
| O3 | Maintain integrity of systems and data | 100% of production changes approved, tested and logged; no unauthorized change detected without a corresponding incident record. | Reliable, auditable service delivery |
| O4 | Achieve and sustain compliance | ISO/IEC 27001:2022 certification maintained with no major nonconformity; PCI DSS validation and HIPAA risk analysis completed annually; 100% of notifications made within legal deadlines. | Market access and regulatory standing |
| O5 | Reduce exposure to vulnerabilities | Critical vulnerabilities remediated within 7 days and high within 30 days, with at least 95% SLA attainment. | Reduced likelihood of compromise |
| O6 | Control access rigorously | 100% of privileged and remote access protected by MFA; 100% of leavers' access revoked within 24 hours; 100% of scheduled access reviews completed on time. | Least privilege across a growing workforce |
| O7 | Build a security-aware workforce | At least 98% of staff complete annual training; phishing simulation click rate at or below 5% and report rate at or above 70%. | People as a defensive control |
| O8 | Respond effectively to incidents | Severity 1 incidents triaged within 1 hour and contained within 4 hours on average; post-incident review held for 100% of Severity 1 and 2 incidents. | Limit impact and regulatory exposure |
| O9 | Manage third-party risk | 100% of critical suppliers assessed before onboarding and at least annually thereafter. | Secure supply chain and acquisitions |
| O10 | Keep the ISMS current | 100% of ISMS policies reviewed on schedule; risk register reviewed quarterly. | Governance that keeps pace with change |

## 5.2 Policy Framework Hierarchy

**5.2.1** NexusGuard shall maintain a four-tier documentation hierarchy (Table 2) under this Policy. Each tier derives its authority from the tier above.

**5.2.2** Where documents conflict, the higher tier shall prevail, and where requirements differ in strictness the stricter shall apply. Applicable law and client contract terms prevail over all tiers.

**5.2.3** Every document in the framework shall carry a unique ID (POL-, STD-, PRC- or GDL- prefix), a named owner, a version, a classification and a review date, and shall be held in the controlled document repository.

**Table 2: Policy Framework Hierarchy**

| Tier | Document type | Nature | Approver / review | Examples |
|---|---|---|---|---|
| 1 | Policies | Mandatory. State what must be done and why, in high-level terms. | Executive Leadership Team or Board; annual | This Policy; Acceptable Use; Access Control; Data Classification and Handling; Incident Response; Privacy |
| 2 | Standards | Mandatory. Specify minimum technical and organizational requirements that implement policies. | CISO via Governance Committee; annual | Password and Authentication Standard; Encryption and Key Management; Secure Configuration (CIS baselines); Logging and Monitoring |
| 3 | Procedures | Mandatory. Step-by-step instructions to carry out a process. | Process owner, reviewed by CISO; at least annual | Joiner-Mover-Leaver; Incident Response Procedure; Vulnerability and Patch Management; Access Review |
| 4 | Guidelines | Advisory. Good-practice advice and templates; not enforceable on their own. | Document owner; as needed | Secure Remote Working Guide; Phishing Awareness Guide; Cloud Security Reference Architecture |

## 5.3 Risk Management

**5.3.1** NexusGuard shall maintain an approved information security risk assessment methodology and apply it to all in-scope systems at least annually and upon significant change, including new systems, new client types, new jurisdictions and acquisitions.

**5.3.2** Risks shall be recorded in a central risk register with an owner, treatment decision and residual rating. The register shall be reviewed at least quarterly.

**5.3.3** Risk acceptance shall be documented and approved at a level matching the risk: Low by the risk owner, Medium by the CISO, and High or Critical by the Executive Leadership Team.

**5.3.4** A data protection impact assessment shall be completed before any high-risk processing of personal data begins (GDPR Art. 35).

## 5.4 Asset Management and Data Classification

**5.4.1** An inventory of all information assets, including hardware, software, data stores, cloud accounts and subscriptions, and SaaS applications, shall be maintained with a named owner for each asset and reviewed at least quarterly.

**5.4.2** All information shall be classified by its owner using the scheme in Table 3, labelled accordingly, and handled according to its classification.

**5.4.3** Restricted information shall be stored and processed only in systems approved for that purpose. Information of mixed classification shall be handled at the highest level present.

**Table 3: Data Classification Scheme**

| Level | Definition | Examples | Minimum handling |
|---|---|---|---|
| Public | Approved for unrestricted release; no harm if disclosed. | Marketing material, published documentation | No special controls; approved owner publishes. |
| Internal | For use within NexusGuard; limited harm if disclosed. | Internal policies, org charts, general procedures | Share only with staff and approved contractors. |
| Confidential | Business-sensitive; serious harm if disclosed. | Client contracts, financials, source code, HR records | Encrypt at rest and in transit; need-to-know access. |
| Restricted | Regulated or highest sensitivity; severe harm and legal consequences if disclosed. | PHI, cardholder data, special category personal data, credentials, cryptographic keys | Encryption, MFA, logging, DLP, segregated environments, named access only. |

**5.4.4** Storage media and devices shall be sanitized to NIST SP 800-88 standards before reuse or disposal, with a certificate of destruction retained for Confidential and Restricted media.

**5.4.5** NexusGuard assets shall be used for business purposes, with limited incidental personal use that does not affect security or work. Users shall not install unlicensed or unapproved software, circumvent security controls, access illegal content, or place Confidential or Restricted information in unapproved cloud storage or AI tools.

## 5.5 Access Control and Identity Management

**5.5.1** Access shall be granted on the principles of least privilege and need-to-know, using role-based access approved by the system or data owner.

**5.5.2** Every user shall have a unique identity. Shared or generic accounts shall be prohibited, except documented service accounts that have an owner, vaulted credentials and no interactive login.

**5.5.3** Passwords and passphrases shall be at least 12 characters for standard accounts and at least 16 characters for privileged and service accounts. Passwords shall be screened against lists of breached and commonly used passwords. Six-character passwords are prohibited.

**5.5.4** Passwords shall not be forced to change on a fixed schedule. They shall be changed immediately on suspected compromise, and periodic change shall be applied only where a regulation or contract requires it (for example PCI DSS Requirement 8.3.9 where passwords are the only factor).

**5.5.5** Users shall not share passwords, authentication codes or tokens with anyone, including IT staff and managers, and shall not write them down or store them unencrypted. Approved password managers shall be used.

**5.5.6** MFA shall be enforced for: all remote access; all cloud services, including Microsoft 365 and email; all privileged access; and all access to systems that store or process PHI or cardholder data. Phishing-resistant MFA (FIDO2 or hardware keys) shall be used for administrators and for Restricted systems where technically feasible.

**5.5.7** Privileged access shall use accounts separate from day-to-day accounts, be granted just in time through a privileged access management solution where available, be session-logged, and be reviewed at least quarterly. Local administrator rights shall be removed from standard users.

**5.5.8** Access shall be provisioned only after HR confirmation and manager approval; adjusted within 5 business days of a role change; and revoked within 24 hours of termination, and immediately for involuntary or high-risk departures. Contractor access shall expire on the contract end date and shall not exceed 90 days without renewal.

**5.5.9** User access rights shall be reviewed at least every six months, and quarterly for privileged accounts and for systems holding PHI or cardholder data. Accounts inactive for 90 days shall be disabled.

**5.5.10** Accounts shall lock after no more than 10 failed attempts for at least 30 minutes or until released by an administrator. Duties for critical functions (request, approve, implement) shall be segregated.

## 5.6 Data Protection, Cryptography and Privacy

**5.6.1** Personal data shall be processed only with a documented lawful basis (GDPR Art. 6, and Art. 9 for health data), for specified purposes, minimized to what is necessary, and retained no longer than the retention schedule allows. Data protection by design and by default shall be applied to new systems and changes.

**5.6.2** PHI shall be accessed, used and disclosed only for purposes permitted by HIPAA and the applicable Business Associate Agreement, applying the minimum necessary standard.

**5.6.3** Cardholder data shall be stored only where there is a documented business need. PAN shall be rendered unreadable wherever stored (strong cryptography, truncation or tokenization), sensitive authentication data shall never be stored after authorization, and the CDE shall be segmented from other networks.

**5.6.4** Confidential and Restricted data shall be encrypted at rest with AES-256 or equivalent, including laptops, mobile devices, backups and removable media.

**5.6.5** Data in transit outside NexusGuard-controlled networks, and Restricted data in transit anywhere, shall be encrypted with TLS 1.2 or higher (TLS 1.3 preferred). Insecure protocols (including SSL, TLS 1.0/1.1, FTP and Telnet) shall not be used.

**5.6.6** Cryptographic keys shall be managed under an approved standard covering generation, storage in a hardware security module or managed key service, rotation, revocation and separation of duties. Keys, secrets and credentials shall never be embedded in source code.

**5.6.7** Data loss prevention controls shall monitor and block unauthorized transfer of Restricted data through email, endpoints and cloud services.

**5.6.8** Data shall be securely deleted at the end of its retention period. Documentation required by HIPAA shall be retained for six years.

**5.6.9** Personal data shall be transferred across borders only under a lawful transfer mechanism approved by the DPO and Legal (for example adequacy decision, standard contractual clauses or UK addendum, or UAE and DIFC requirements), and client data residency commitments shall be honored.

**5.6.10** Data subject requests shall be logged and answered within the legal timeframe (one month under GDPR) under the DPO's direction.

## 5.7 Physical and Environmental Security

**5.7.1** All NexusGuard facilities, including the Dubai headquarters, the London and New York offices and data centers, shall use tiered physical zones (public, general office and restricted) with badge-controlled entry. Access logs shall be retained for at least 12 months and CCTV footage for restricted areas for at least 90 days.

**5.7.2** Visitors shall sign in, show identification, wear a visitor badge, be escorted at all times, and be recorded in a visitor log retained for at least 12 months.

**5.7.3** Data centers and co-location facilities used by NexusGuard shall provide fire suppression, resilient power and cooling, environmental monitoring and controlled access, with assurance evidence (ISO/IEC 27001 or SOC 2) obtained annually for third-party facilities.

**5.7.4** Users shall lock screens when leaving a device, screens shall auto-lock after no more than 10 minutes of inactivity, and Confidential and Restricted paper documents shall be locked away when not in use and destroyed by cross-cut shredding or secure bins.

**5.7.5** Remote working shall be done only on NexusGuard-managed or approved devices, over VPN or zero-trust access with MFA, from a location where screens and conversations cannot be observed. Restricted information shall not be printed outside NexusGuard facilities.

**5.7.6** Laptops and mobile devices shall be enrolled in device management, use full-disk encryption, run endpoint detection and response, and support remote wipe. Lost or stolen devices shall be reported immediately and within 1 hour of discovery. Personally owned devices may be used only if approved and enrolled in a managed container.

**5.7.7** Removable media shall be blocked by default. Exceptions require approval and encryption.

## 5.8 Email, Internet, Social Media and AI Use

**5.8.1** Email and collaboration services in Microsoft 365 shall be configured with anti-phishing and safe-attachment protection, SPF, DKIM and enforced DMARC, conditional access and baseline hardening aligned to the CIS Microsoft 365 Benchmark.

**5.8.2** Company email and internet access shall be used for business purposes, with limited personal use that does not interfere with work or security. Automatic forwarding to external addresses shall be disabled, and Restricted information shall not be sent to personal accounts. Confidential and Restricted information shall be emailed only through approved encrypted channels.

**5.8.3** Users shall report suspected phishing through the designated reporting button or channel immediately, and within 1 hour of discovery. Simulated phishing exercises shall run at least quarterly.

**5.8.4** Web filtering shall block malicious and prohibited categories. Users shall not download software from unapproved sources.

**5.8.5** Personnel shall not disclose Confidential or Restricted information, client names or incident details on social media, and shall not speak for NexusGuard on social media unless authorized. Official channels shall be managed by Marketing and Communications.

**5.8.6** Generative AI and similar tools shall be used only if approved. Confidential, Restricted and personal data shall not be entered into unapproved tools, and AI output shall be reviewed by a person before use in client or regulated work.

## 5.9 Operations, Network and Development Security

**5.9.1** Endpoint detection and response shall be deployed on all endpoints and servers, and protection shall update automatically.

**5.9.2** Authenticated vulnerability scans shall run at least monthly (and at least quarterly for external ASV scans where PCI DSS applies). Critical vulnerabilities shall be remediated within 7 days, high within 30 days and medium within 90 days. Penetration tests shall be performed at least annually and after significant change.

**5.9.3** Systems shall be built to hardened baselines (CIS Benchmarks or equivalent). Deviations shall be approved and recorded.

**5.9.4** Logs from critical systems, identity services, cloud control planes and security tools shall be sent to a central SIEM, time-synchronized and protected from tampering. Logs shall be retained for at least 12 months with the most recent 3 months immediately available, and reviewed through 24x7 monitoring.

**5.9.5** Backups of critical systems shall be taken at least daily, encrypted and stored separately from production. Restoration shall be tested at least quarterly for critical systems and annually for others.

**5.9.6** Networks shall be segmented, with the CDE and PHI environments isolated. Firewalls shall be default-deny, wireless networks shall use WPA2/WPA3 Enterprise, guest networks shall be isolated, and firewall rules shall be reviewed at least every six months.

**5.9.7** All changes to production shall be assessed for security impact, approved, tested and recorded. Emergency changes shall be reviewed within 5 business days.

**5.9.8** Software shall be developed under a secure development lifecycle including code review, static and dynamic testing and dependency scanning. Development, test and production shall be separated, and live PHI or PAN shall not be used in non-production environments unless masked.

## 5.10 Cloud Security

**5.10.1** Cloud services shall not be procured or used without CISO approval and a security assessment. Unapproved cloud use (shadow IT) is prohibited.

**5.10.2** The shared responsibility model shall be documented for each cloud provider. Cloud accounts and subscriptions shall be placed under a central organizational structure with baseline configuration aligned to the relevant CIS Foundations Benchmark and monitored continuously for misconfiguration.

**5.10.3** Public exposure of storage, databases and management interfaces shall be prohibited unless an approved exception exists. Root and global administrator accounts shall be protected by MFA and used only for break-glass purposes.

**5.10.4** Restricted data in the cloud shall be encrypted with customer-managed keys, and audit logging shall be enabled for all control plane and data access activity.

**5.10.5** Cloud providers shall supply current assurance evidence (SOC 2 Type II, ISO/IEC 27001, PCI AOC and a HIPAA Business Associate Agreement where relevant) at least annually, and data residency shall conform to Section 5.6.9.

## 5.11 Third-Party and Supplier Security

**5.11.1** Third parties shall be risk-tiered and assessed for security before engagement. Critical suppliers shall be reassessed at least annually and others at least every two years or on material change.

**5.11.2** Contracts shall include security and confidentiality obligations, breach notification within the timeframe set by NexusGuard (no later than 72 hours, and sooner where a client contract requires), audit rights, flow-down to subcontractors, and return or secure destruction of data on exit.

**5.11.3** A HIPAA Business Associate Agreement shall be signed before any PHI is disclosed, a GDPR Art. 28 data processing agreement before any personal data is shared, and a PCI DSS responsibility matrix and Attestation of Compliance obtained from any service provider that can affect the CDE.

**5.11.4** Third-party access shall be least-privilege, time-bound, MFA-protected and logged, and shall not be granted before contract and confidentiality terms are signed.

**5.11.5** When an engagement ends, third-party access shall be revoked immediately and the supplier shall confirm return or destruction of NexusGuard and client data.

**5.11.6** PayStream Analytics shall complete a gap assessment against this Policy within 90 days of the Effective Date and align its controls within 12 months. Until alignment is complete, the stricter of PayStream's existing policies and this Policy shall apply, and PayStream shall maintain its own regulatory and certification obligations.

## 5.12 Incident Management and Breach Notification

**5.12.1** All personnel shall report suspected or actual security incidents and events immediately, and within 1 hour of discovery at the latest, through the designated incident reporting channel. Personnel shall not investigate on their own or discuss incidents externally.

**5.12.2** The Security Operations Team shall classify every incident using Table 4 within 30 minutes of triage and escalate according to its severity.

**Table 4: Incident Severity Classification**

| Severity | Definition | Response target | Escalation |
|---|---|---|---|
| 1 Critical | Confirmed or suspected compromise of Restricted data (PHI, cardholder or special category data) or a major outage of client-facing services. | Triage within 1 hour; continuous response until contained. | CISO, DPO, Legal and Executive Leadership Team within 1 hour. |
| 2 High | Compromise of Confidential data, a privileged account breach, active malware, or a significant service degradation. | Triage within 2 hours. | CISO and affected owners within 4 hours. |
| 3 Medium | Contained security event with limited impact, or a policy violation with potential for harm. | Triage within 1 business day. | Security Operations Lead. |
| 4 Low | Minor event or information request with no evidence of harm. | Triage within 3 business days. | Logged and tracked. |

**5.12.3** The CISO shall maintain a documented Incident Response Plan covering roles, communications, legal notification, containment, eradication, recovery and evidence handling. The plan shall be tested at least annually through a tabletop or simulated exercise and updated after every Severity 1 or 2 incident.

**5.12.4** Regulatory and client notification decisions shall be made by Legal, the DPO and the CISO within 24 hours of an incident being confirmed, and notifications shall meet the deadlines in Table 5.

**Table 5: Breach Notification Requirements**

| Regime | Trigger | Deadline | Recipient |
|---|---|---|---|
| GDPR / UK GDPR | Personal data breach likely to result in a risk to individuals (Art. 33, 34). | Controller: 72 hours after becoming aware. Processor: without undue delay to the controller. Individuals without undue delay if high risk. | Supervisory authority (for example ICO), client controller, data subjects |
| HIPAA Breach Notification Rule | Breach of unsecured PHI (45 CFR 164.400-414). | NexusGuard as business associate: without unreasonable delay and no later than 60 days from discovery, or sooner if the BAA states. | Affected covered entity (which notifies individuals, HHS and media) |
| PCI DSS v4.0 | Suspected or confirmed compromise of account data (Req. 12.10). | Immediately, as defined by acquirer and card brand rules. | Acquirer, payment brands, forensic investigator if required |
| UAE and DIFC law | Personal data breach affecting UAE or DIFC data subjects. | As prescribed by the applicable law and authority. | Relevant UAE authority |
| US state laws (for example New York SHIELD Act) | Breach of private information of state residents. | As prescribed by the applicable state law. | State regulators and affected individuals |

**5.12.5** Evidence shall be preserved with a chain of custody, including forensic images and relevant logs. Affected systems shall not be wiped or powered off without CISO approval, and legal hold shall be applied when required.

**5.12.6** A post-incident review shall be held within 10 business days of closure of every Severity 1 or 2 incident. Corrective actions shall be tracked to completion.

**5.12.7** Incident records shall be retained for at least six years. No person shall suffer retaliation for reporting an incident in good faith.

## 5.13 Business Continuity and Disaster Recovery

**5.13.1** A business impact analysis shall be performed at least annually and shall define recovery time objectives (RTO) and recovery point objectives (RPO) for each critical service.

**5.13.2** Business continuity and disaster recovery plans shall exist for all critical services, be tested at least annually, and have results reported to the Governance Committee with remedial actions tracked.

**5.13.3** Crisis communication arrangements shall identify who informs clients, regulators and staff during a disruption.

## 5.14 Personnel Security, Awareness and Training

**5.14.1** Employees and contractors shall be screened before engagement, in proportion to the sensitivity of their access and as permitted by law, covering identity, employment history and qualifications and, where lawful, criminal record checks.

**5.14.2** Employment and contractor agreements shall include confidentiality and security obligations that continue after termination. Personnel shall acknowledge this Policy at onboarding and annually.

**5.14.3** All personnel shall complete security awareness training before being given access to Confidential or Restricted information and within 30 days of joining, and shall complete a refresher at least annually.

**5.14.4** Role-based training shall be provided for staff who handle PHI (HIPAA), work in the CDE (PCI DSS), process personal data (GDPR), hold privileged access, or develop software, and Executive Leadership Team and Board members shall receive an annual security briefing.

**5.14.5** Staff who fail simulated phishing exercises repeatedly shall receive targeted coaching. Non-completion of mandatory training 30 days after the due date shall be escalated to the line manager and may result in access suspension.

**5.14.6** Training records shall be retained for at least six years. On termination, personnel shall return all assets, have access revoked and be reminded of continuing confidentiality obligations.

## 5.15 Monitoring, Audit and Continual Improvement

**5.15.1** The ISMS shall be audited internally at least annually by a function independent of the area audited, and externally through certification and client audits.

**5.15.2** PCI DSS validation, a HIPAA security risk analysis and a review of GDPR records of processing shall be completed at least annually.

**5.15.3** Audit findings and nonconformities shall be recorded with an owner and due date. Critical findings shall be closed within 30 days.

**5.15.4** Security KPIs (Table 1) shall be reported to the Executive Leadership Team quarterly, and lessons from incidents, audits and changes in risk shall drive continual improvement of this Policy.

# 6. Compliance

This Policy supports NexusGuard's legal, regulatory and contractual obligations. Table 6 shows the regimes in scope, and Table 7 maps each policy domain to the controls it supports. References are paraphrased pointers; the source text of each standard or regulation prevails.

**Table 6: Regulatory and Standards Basis**

| Regime | Relevance to NexusGuard | Key provisions supported |
|---|---|---|
| ISO/IEC 27001:2022 | ISMS standard; certification target. | Clauses 4 to 10 (including 5.2 policy, 6.2 objectives, 9.3 management review); Annex A themes 5 to 8. |
| HIPAA Security and Breach Notification Rules | NexusGuard handles PHI as a business associate for healthcare clients. | 45 CFR 164.308 (administrative), 164.310 (physical), 164.312 (technical), 164.314, 164.316 (documentation), 164.400-414 (breach notification). |
| PCI DSS v4.0 | Applies to payment account data in scope, including PayStream Analytics. | Requirements 1 to 12, notably 8 (authentication), 10 (logging), 12.1 (information security policy), 12.6 (awareness), 12.8 (service providers) and 12.10 (incident response). |
| GDPR / UK GDPR | EU and UK personal data; London office and EU clients. | Art. 5 principles, 6 and 9 (lawful basis), 24, 25, 28, 30, 32, 33, 34, 35 and 44 to 49. |
| NIST CSF 2.0 | Framework used to structure and measure the ISMS. | Govern, Identify, Protect, Detect, Respond and Recover functions. |
| UAE NESA and UAE law | Dubai headquarters and UAE clients. | UAE Information Assurance management and technical control families, and UAE data protection law. |

**Table 7: Policy Domain to Control Crosswalk**

| Policy section | ISO/IEC 27001:2022 | HIPAA | PCI DSS v4.0 | GDPR | NIST CSF 2.0 |
|---|---|---|---|---|---|
| 5.1 Governance and objectives | Cl. 5.2, 6.2, 9.3; A.5.1, A.5.2 | 164.308(a)(1)-(2) | 12.1, 12.4 | Art. 5(2), 24 | GV.OC, GV.RR, GV.PO |
| 5.2 Policy framework | Cl. 7.5; A.5.1 | 164.316 | 12.1 | Art. 24 | GV.PO |
| 5.3 Risk management | Cl. 6.1, 8.2, 8.3 | 164.308(a)(1)(ii)(A)-(B) | 12.3 | Art. 32, 35 | GV.RM, ID.RA |
| 5.4 Asset and data classification | A.5.9, 5.10, 5.12, 5.13, 7.10, 7.14 | 164.310(d) | 9.4, 12.5.1 | Art. 30 | ID.AM, PR.DS |
| 5.5 Access control | A.5.15-5.18, 8.2, 8.5 | 164.308(a)(3)-(4); 164.312(a), (d) | 7, 8 | Art. 32 | PR.AA |
| 5.6 Data protection and privacy | A.5.34, 8.24 | 164.312(a)(2)(iv), (c), (e) | 3, 4 | Art. 5, 6, 9, 25, 32, 44-49 | PR.DS |
| 5.7 Physical security | A.7.1-7.14, 6.7, 8.1 | 164.310 | 9 | Art. 32 | PR.AA, PR.PS |
| 5.8 Email, internet, social, AI | A.5.10, 5.14, 8.7, 8.23 | 164.308(a)(5)(ii)(B) | 5, 12.6 | Art. 32 | PR.AT, PR.DS |
| 5.9 Operations and network | A.8.7-8.9, 8.13, 8.15, 8.16, 8.20-8.22, 8.25, 8.32 | 164.312(b) | 1, 2, 5, 6, 10, 11 | Art. 32 | PR.PS, PR.IR, DE.CM |
| 5.10 Cloud security | A.5.23, 8.9 | 164.308(b) | 2, 12.8 | Art. 28, 32 | GV.SC, PR.IR |
| 5.11 Third parties | A.5.19-5.22 | 164.308(b); 164.314(a) | 12.8 | Art. 28 | GV.SC |
| 5.12 Incident management | A.5.24-5.28, 6.8 | 164.308(a)(6); 164.400-414 | 12.10 | Art. 33, 34 | DE.AE, RS |
| 5.13 Continuity and DR | A.5.29, 5.30, 8.13, 8.14 | 164.308(a)(7) | 12.10.1 | Art. 32(1)(c) | RC.RP, PR.IR |
| 5.14 Personnel and training | A.6.1-6.5, 6.3 | 164.308(a)(3), (a)(5) | 12.6, 12.7 | Art. 32(4), 39 | PR.AT, GV.RR |
| 5.15 Monitoring and improvement | Cl. 9, 10; A.5.35, 5.36 | 164.308(a)(8) | 11, 12.4 | Art. 24, 32(1)(d) | ID.IM, GV.OV |

# 7. Enforcement and Sanctions

**7.1** Compliance with this Policy and its supporting documents is mandatory. Personnel shall not knowingly violate it, and managers shall not instruct or permit violations.

**7.2** Violations shall be handled under the HR disciplinary procedure and the sanction policy required by HIPAA 164.308(a)(1)(ii)(C). Sanctions shall be proportionate and consistently applied and may include retraining, a formal warning, suspension of access, suspension without pay, and termination of employment.

**7.3** Contractors and temporary staff who violate this Policy shall be subject to termination of their contract. Third parties shall be subject to the remedies in their contracts, including suspension of access and termination.

**7.4** Serious or deliberate violations, including unauthorized disclosure of Restricted data, circumvention of security controls, or concealment of an incident, shall be escalated to the CISO and the HR Director within 24 hours, and may be referred to law enforcement or regulators where laws have been broken.

**7.5** Employment contracts and contractor agreements shall reference this Policy so that its obligations are enforceable.

# 8. Exceptions

**8.1** Exceptions to this Policy shall be requested through the Policy Exception Management Process and shall be formally requested in writing, with a business justification, a risk assessment and proposed compensating controls.

**8.2** Exceptions shall be approved by the CISO for Low and Medium risk and by the Executive Leadership Team for High or Critical risk. They shall be time-limited to no more than 12 months (six months for High risk), recorded in the exception register, and reviewed before expiry.

**8.3** No exception shall be granted for a requirement imposed by law, regulation or a client contract, unless Legal confirms in writing that it is permitted.

**8.4** Unapproved or expired exceptions shall be treated as violations under Section 7.

# 9. Related Documents

| Document | ID | Tier |
|---|---|---|
| Policy Exception Management Process | PRC-GRC-001 | 3 Procedure |
| Acceptable Use Policy | POL-AUP-001 | 1 Policy |
| Access Control Policy | POL-ACC-001 | 1 Policy |
| Data Classification and Handling Policy | POL-DCH-001 | 1 Policy |
| Privacy and Data Protection Policy | POL-PRV-001 | 1 Policy |
| Incident Response Policy and Plan | POL-IRP-001 | 1 Policy |
| Third-Party Security Policy | POL-TPS-001 | 1 Policy |
| Business Continuity and Disaster Recovery Policy | POL-BCP-001 | 1 Policy |
| Password and Authentication Standard | STD-IAM-001 | 2 Standard |
| Encryption and Key Management Standard | STD-CRY-001 | 2 Standard |
| Joiner-Mover-Leaver Procedure | PRC-HRS-001 | 3 Procedure |
| Vulnerability and Patch Management Procedure | PRC-VUL-001 | 3 Procedure |
| Secure Remote Working Guide | GDL-REM-001 | 4 Guideline |

_Document IDs are proposed identifiers under the framework in Section 5.2. Confirm them against the document register as each document is issued._

# 10. Review

This policy shall be reviewed annually or when significant changes occur. The Policy Owner initiates the review.

## 10.1 Review Cycle

**10.1.1** The CISO shall initiate a full review of this Policy at least every 12 months, and sooner after any of the following: an acquisition or new office, a new or changed regulation, a Severity 1 incident, a major audit finding, a significant change to the technology estate, or a change in business strategy.

**10.1.2** Each review shall be recorded in the Version History, even where no change is made.

## 10.2 Document Control

**10.2.1** Changes shall follow the approval path: author, CISO, consultation with Legal, HR and IT, Governance Committee review, and approval by the Executive Leadership Team and Board of Directors. Minor edits that do not change requirements may be approved by the CISO and reported at the next committee meeting.

**10.2.2** Versions shall use major.minor numbering. A major version change indicates a change in requirements and a minor version an editorial change.

**10.2.3** The approved version shall be published in the controlled document repository, communicated to all personnel and third parties in scope, and acknowledged by personnel within 30 days of publication. Superseded versions shall be archived and retained for at least six years.
