# NexusGuard Technologies Ltd. | Policy Gap Analysis Report | RPT-ISP-001

| Field | Detail |
|---|---|
| **Document Title** | Policy Gap Analysis Report: Information Security Policy v1.0 vs v3.0 |
| **Document ID** | RPT-ISP-001 |
| **Version** | 1.0 |
| **Classification** | Internal |
| **Author** | Augustine Ozor, GRC Analyst |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Pending |
| **Approval Date** | Pending |
| **Effective Date** | Upon approval of POL-ISP-001 v3.0 |
| **Next Review Date** | 12 months from approval date |
| **Applicable Regulations** | ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0, UAE NESA |

# Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 0.1 | 11/10/2026 | Augustine Ozor | Initial draft: gap analysis of IS Policy v1.0 against v3.0. |
| 1.0 | Pending | CISO | Approved and published with POL-ISP-001 v3.0. |

# 1. Purpose

This report compares the Information Security Policy v1.0 (January 2021) with the new v3.0 (POL-ISP-001). It records each gap in v1.0, the original wording, the requirement that closes the gap in v3.0 and the rationale, so that management can see why the policy was rewritten rather than amended.

# 2. Scope and Method

All ten sections of v1.0 and its annotated gaps were reviewed, then tested against ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0 and UAE NESA, and against NexusGuard's current footprint (Dubai, London and New York, cloud infrastructure, healthcare clients and PayStream Analytics). Severity is rated as follows.

**Critical:** non-conformity with a mandatory legal, regulatory or contractual requirement, or a gap that directly exposes regulated data. **High:** significant control weakness that would likely fail an ISO 27001, HIPAA or PCI DSS audit. **Medium:** maturity or structure improvement without direct regulatory exposure.

# 3. Summary of Findings

Sixteen gaps were identified: the 14 annotated in v1.0 (G-01 to G-14) and 2 further gaps found during review (G-15 and G-16). Of these, 6 are Critical, 9 High and 1 Medium. v3.0 closes all of them.

| Severity | Count | Gaps |
|---|---|---|
| Critical | 6 | G-02 scope: locations; G-03 scope: people and entities; G-05 roles (no CISO); G-08 passwords and MFA; G-10 data protection; G-12 incident reporting |
| High | 9 | G-01, G-04, G-06, G-07, G-09, G-11, G-13, G-14, G-15 |
| Medium | 1 | G-16 policy framework hierarchy |

# 4. Detailed Gap Analysis

| Gap | Old text (v1.0) | New requirement (v3.0) | Rationale |
|---|---|---|---|
| **G-01**<br>Introduction and regulatory basis<br>**Severity: High**<br>_[GAP: No reference to ISO 27001, HIPAA, PCI DSS or GDPR.]_ | "NexusGuard Technologies is committed to protecting its information assets. This policy establishes the framework for information security within the company." | Sections 1 and 6 state the purpose and the regulatory basis (ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0, UAE NESA), with a crosswalk from each policy domain to controls (Tables 6 and 7). | ISO 27001 requires legal and contractual requirements to be identified (Cl. 4.2, A.5.31). HIPAA 164.316 and PCI DSS 12.1 require documented policies. Healthcare and payment clients expect evidence. |
| **G-02**<br>Scope: locations<br>**Severity: Critical**<br>_[GAP: Covers only the Dubai HQ; London and New York omitted.]_ | "...all employees of NexusGuard Technologies and their use of company information systems at our Dubai headquarters." | Section 2 covers Dubai, London and New York, data centers, home working and travel, and all future offices. | GDPR / UK GDPR and US state laws apply to the London and New York operations. Unprotected locations leave regulated data outside ISMS control. |
| **G-03**<br>Scope: people and entities<br>**Severity: Critical**<br>_[GAP: No contractors, third parties or PayStream Analytics (acquired 2025).]_ | "This policy applies to all employees..." | Section 2 covers employees, contractors, temporary staff, interns and third parties, and names PayStream Analytics. Clause 5.11.6 sets a 90-day gap assessment and 12-month alignment plan. | Contractors and suppliers hold the same access as staff. HIPAA 164.308(b) and GDPR Art. 28 require third-party obligations. An acquired entity with separate controls is a weak link. |
| **G-04**<br>Scope: systems and cloud<br>**Severity: High**<br>_[GAP: Cloud infrastructure not covered.]_ | "...their use of company information systems..." | Section 2 covers on-premises, data center, cloud (IaaS, PaaS, SaaS including Microsoft 365), endpoints, BYOD and AI tools. Section 5.10 sets cloud security requirements. | ISO 27001 A.5.23 and PCI DSS 12.8 require control of cloud services. Cloud misconfiguration is a leading cause of data exposure. |
| **G-05**<br>Responsibilities: roles<br>**Severity: Critical**<br>_[GAP: No CISO role (hired 2023); no security, compliance or management responsibilities.]_ | "The IT Manager is responsible for information security." | Section 4 assigns responsibilities to the Board, CISO, Governance Committee, Security Operations, DPO, Legal and Compliance, IT, HR, line managers, owners, employees, contractors, third parties and PayStream. | ISO 27001 A.5.2 and Cl. 5.3 and HIPAA 164.308(a)(2) require assigned security responsibility. GDPR Art. 37 requires a DPO where applicable. |
| **G-06**<br>Language: enforceability<br>**Severity: High**<br>_[GAP: Uses "should" instead of "shall"; not enforceable.]_ | "All employees should follow this policy." | All mandatory requirements use "shall". Section 3 defines shall, should and may, and Section 7 binds personnel through contracts. | Advisory wording cannot support disciplinary action or demonstrate control to auditors and regulators. |
| **G-07**<br>Objectives<br>**Severity: High**<br>_[GAP: Not measurable; no business alignment, KPIs or explicit confidentiality, integrity and availability.]_ | "Our objectives are to keep our data safe and ensure our systems are available for business use." | Clause 5.1 and Table 1 set ten objectives with measures and targets covering confidentiality, integrity and availability, each tied to business strategy and reported quarterly. | ISO 27001 Cl. 6.2 requires measurable security objectives. Without KPIs management cannot evaluate performance (Cl. 9.1). |
| **G-08**<br>Password and authentication<br>**Severity: Critical**<br>_[GAP: 6 characters is too short; no MFA; no ban on sharing; no privileged account rules; forced rotation contradicts NIST 800-63B.]_ | "All employees should use strong passwords of at least 6 characters. Passwords should be changed every 90 days." | Clauses 5.5.2 to 5.5.10: unique IDs; 12 characters (16 for privileged and service accounts); breached-password screening; no scheduled rotation; sharing prohibited; MFA for remote, cloud, privileged, PHI and CDE access; PAM; lockout; access reviews. | PCI DSS 8.3.6 requires at least 12 characters and 8.4.2 requires MFA for CDE access. HIPAA 164.312(d) requires authentication. NIST SP 800-63B advises against periodic rotation. |
| **G-09**<br>Email and internet use<br>**Severity: High**<br>_[GAP: No phishing guidance, no forwarding limits, no M365 or social media rules.]_ | "Employees may use company email and internet for business purposes. Personal use should be limited." | Section 5.8: M365 hardening with SPF, DKIM and DMARC; no external auto-forwarding; encrypted channels for sensitive data; phishing reporting within 1 hour and quarterly simulations; social media and generative AI rules. | Phishing is a primary attack path to credentials. PCI DSS 12.6.3.1 requires phishing awareness. Data leakage through email and AI tools must be prevented. |
| **G-10**<br>Data protection<br>**Severity: Critical**<br>_[GAP: No classification scheme, definition of "sensitive", PHI, PCI or PII coverage, GDPR lawful basis, handling procedures or encryption.]_ | "Employees should take care when handling company data. Sensitive information should not be shared with unauthorized persons." | Sections 5.4 and 5.6: four-level classification (Table 3), lawful basis and minimization, PHI minimum necessary, PAN protection, AES-256 at rest, TLS 1.2+ in transit, key management, DLP, retention, cross-border transfers and data subject requests. | GDPR Art. 5, 6, 9 and 32, HIPAA 164.312, and PCI DSS 3 and 4 require defined protection of regulated data. Classification is the basis for proportionate controls (ISO A.5.12). |
| **G-11**<br>Physical security<br>**Severity: High**<br>_[GAP: Dubai only; no data center, clean desk, remote work or device security.]_ | "The office should be secured with access cards. Visitors must sign in at reception." | Section 5.7: tiered zones at all sites and data centers, visitor escort and logs, CCTV, clear desk and screen, remote working rules, device encryption and management, lost-device reporting within 1 hour, media controls. | HIPAA 164.310 and PCI DSS 9 require physical safeguards. Post-COVID hybrid work moves data onto laptops and home networks (ISO A.6.7, A.8.1). |
| **G-12**<br>Incident reporting<br>**Severity: Critical**<br>_[GAP: No classification, escalation, regulatory notification, IR plan reference or evidence preservation.]_ | "If you notice a security problem, please inform the IT department." | Section 5.12: report within 1 hour; four severity levels (Table 4); tested IR plan; notification deadlines (Table 5: GDPR 72 hours, HIPAA 60 days maximum, PCI immediate, UAE and US state laws); evidence handling; post-incident review. | GDPR Art. 33 sets a 72-hour clock and HIPAA 164.410 a 60-day limit. Late notification brings fines and client contract breaches. PCI DSS 12.10 and ISO A.5.24-5.28 require formal response. |
| **G-13**<br>Compliance, enforcement and exceptions<br>**Severity: High**<br>_[GAP: No defined sanctions, no link to employment contract or HR procedure, no exception process.]_ | "Failure to follow this policy may result in disciplinary action." | Sections 7 and 8: graduated sanctions under the HR disciplinary procedure, contractor and third-party remedies, 24-hour escalation of serious violations, and a time-limited, risk-assessed exception process. | HIPAA 164.308(a)(1)(ii)(C) requires a sanction policy. ISO A.6.4 requires a disciplinary process. Uncontrolled exceptions erode the control environment. |
| **G-14**<br>Approval and document control<br>**Severity: High**<br>_[GAP: Approved by IT Manager only; no CISO, Board or management review; not reviewed since creation; no version history.]_ | "Approved by: Ahmed Hassan, IT Manager. Date: 15 January 2021." | Version history, ownership and Section 10: annual review, approval by Executive Leadership Team and Board, major.minor versioning, controlled repository, 30-day acknowledgment, six-year archive. | ISO 27001 Cl. 5.2 requires top-management approval and Cl. 7.5 documented information control. PCI DSS 12.1.2 requires annual review. |
| **G-15**<br>Missing security domains (analyst finding)<br>**Severity: High**<br>_[GAP: Not annotated in v1.0: no awareness and training, third-party, continuity, vulnerability, logging, backup or asset management requirements.]_ | (No corresponding text in v1.0.) | Sections 5.3 and 5.4 (risk, assets), 5.9 (vulnerabilities, logging, backups, change, development), 5.11 (third parties), 5.13 (continuity) and 5.14 (personnel and training). | The domains are required by ISO 27001 Annex A, HIPAA 164.308(a)(5) and (a)(7), and PCI DSS 6, 10, 11 and 12.8. Their absence would cause audit failure. |
| **G-16**<br>Policy framework hierarchy (analyst finding)<br>**Severity: Medium**<br>_[GAP: Not annotated in v1.0: no structure linking policy to standards, procedures and guidelines.]_ | (No corresponding text in v1.0.) | Section 5.2 and Table 2: four-tier hierarchy with approvers, review cycles, precedence rules and document ID convention. | A structured hierarchy lets a short umbrella policy stay stable while technical detail is maintained in standards and procedures (ISO A.5.1). |

# 5. Regulatory Coverage: v1.0 vs v3.0

| Regime | v1.0 coverage | v3.0 coverage |
|---|---|---|
| ISO/IEC 27001:2022 | None cited. No objectives, roles or document control. | Aligned to Clauses 4 to 10 and Annex A themes 5 to 8, with a crosswalk (Table 7). |
| HIPAA | None. No PHI, breach notification, BAAs or sanctions. | PHI handling, BAAs, 60-day breach limit, sanction policy, six-year retention. |
| PCI DSS v4.0 | None. 6-character passwords and no MFA. | 12/16-character passwords, MFA for CDE, PAN protection, logging, scanning, incident response. |
| GDPR / UK GDPR | None. No lawful basis or 72-hour notification. | Lawful basis, DPIA, DPO, transfers, data subject requests, 72-hour notification. |
| NIST CSF 2.0 | None. | ISMS structured by the six functions and mapped in Table 7. |
| UAE NESA | None. | Dubai HQ in scope; UAE notification and control families referenced. |

# 6. Recommendations and Next Steps

| Action | Owner | Suggested timing |
|---|---|---|
| Approve POL-ISP-001 v3.0 through the Executive Leadership Team and Board, replacing v1.0. | CISO | Next scheduled meeting |
| Publish v3.0, brief managers and obtain staff acknowledgment. | CISO and HR | Within 30 days of approval |
| Issue priority supporting documents: Access Control Policy, Password Standard, Data Classification Policy, Incident Response Plan, Third-Party Security Policy. | CISO | Within 90 days |
| Complete PayStream Analytics gap assessment, then align controls. | PayStream security lead | 90 days, then 12 months |
| Roll out awareness and role-based training and begin quarterly phishing simulations. | HR and Security | Within 60 days |
| Baseline the Table 1 KPIs and report to the Executive Leadership Team. | CISO | First quarterly report after approval |

_Timings are recommendations for management decision, not commitments already made._

# 7. Related Documents and Review

Related: POL-ISP-001 Information Security Policy v3.0; IS Policy v1.0 (superseded); Policy Exception Management Process (PRC-GRC-001). This report shall be reviewed when POL-ISP-001 is next reviewed; the Policy Owner initiates the review.
