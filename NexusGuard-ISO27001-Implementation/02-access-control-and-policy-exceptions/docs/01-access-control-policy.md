# NexusGuard Technologies Ltd. | Access Control Policy | POL-ACC-001

| Field | Detail |
|---|---|
| **Document Title** | Access Control Policy |
| **Document ID** | POL-ACC-001 |
| **Version** | 1.0 |
| **Classification** | Internal |
| **Author** | Augustine Ozor, GRC Analyst |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Executive Leadership Team (approval pending) |
| **Approval Date** | Pending (DD/MM/YYYY to be entered on approval) |
| **Effective Date** | Upon approval |
| **Next Review Date** | 12 months from approval date |
| **Applicable Regulations** | ISO/IEC 27001:2022, HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0, UAE NESA |

# Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 0.1 | 12/10/2026 | Augustine Ozor, GRC Analyst | Initial draft, mandated by James Richardson for approval within two weeks (by 26/10/2026), ahead of HIPAA client onboarding. Follows an internal review that found excess privileged access, active accounts of former PayStream staff, and no joiner/mover/leaver process. |
| 1.0 | Pending | Executive Leadership Team | Approval and publication. |

# 1. Purpose

This Access Control Policy (the "Policy") sets the mandatory requirements for granting, managing, reviewing and removing access to NexusGuard Technologies Ltd. ("NexusGuard") information, systems and facilities. Its purpose is to make sure that only the right people have the right access, for the right time, and that every access decision can be shown to an auditor, a regulator or a client.

A recent internal review found three serious gaps: 42 employees hold privileged access they no longer need; 8 former PayStream Analytics employees still have active accounts three months after the acquisition; and NexusGuard has no formal joiner, mover and leaver (JML) process. With HIPAA client onboarding approaching, these gaps expose protected health information (PHI) and breach the access requirements of HIPAA, PCI DSS and ISO/IEC 27001.

This Policy shall:

- establish the principles of least privilege, need-to-know and separation of duties;
- require a formal process for user registration and de-registration (joiner, mover, leaver);
- set requirements for privileged access, authentication and passwords (aligned to NIST SP 800-63B) and remote access;
- control third-party and contractor access;
- mandate quarterly access reviews and the logging and monitoring of access events; and
- require the existing gaps to be closed within defined deadlines (Section 5.9).

# 2. Scope

| Dimension | Coverage |
|---|---|
| Who | All employees, contractors, consultants, temporary staff and interns, and third parties (suppliers, managed service providers, partners) with access to NexusGuard or client information or systems. This includes **PayStream Analytics** personnel and systems. |
| Accounts | All account types: standard user, privileged, service, third-party, shared (where permitted by exception) and emergency (break-glass) accounts. |
| Systems | All on-premises and cloud systems, including Microsoft Active Directory and Entra ID, Microsoft 365, AWS, SaaS applications, databases, network and security devices, VPN and Zscaler services, and applications that hold PHI, cardholder data or other Restricted information. |
| Locations | Dubai headquarters, London and New York offices, data centers, and remote and home locations. |

Where a law, regulation or client contract requires a stricter control than this Policy, the stricter requirement shall apply.

# 3. Definitions

| Term | Definition |
|---|---|
| Least privilege | Giving a person, process or system only the access needed to perform an approved task, for only as long as needed. |
| Need-to-know | Access to information only where it is required for a person's specific duties. |
| Separation of duties (SoD) | Dividing a sensitive task between people so that no one person can complete it, or approve their own work, alone. |
| Joiner, Mover, Leaver (JML) | The lifecycle events of a new starter, a change of role or location, and a departure. |
| Privileged account | An account with elevated rights over systems, security tools, cloud tenants, identity services or data (for example administrator, root, global admin, domain admin and database admin). |
| Service account | A non-human account used by an application or process to access systems. |
| Break-glass account | An emergency privileged account held under dual control for use only when normal access fails. |
| PAM | Privileged access management: the tooling and process that vaults privileged credentials, grants elevated access just in time and records sessions. |
| Just-in-time (JIT) access | Temporary elevation of rights, with approval and automatic expiry, instead of permanent privilege. |
| MFA | Multi-factor authentication using two or more independent factors. |
| ZTNA / Zscaler Private Access | Zero-trust network access that connects a verified user and compliant device to a specific application, rather than to the whole network. |
| Jump server | A hardened, monitored server through which administrators reach other systems. |
| Sponsor | The NexusGuard employee accountable for a third party's or contractor's access. |
| Orphan account | An account with no current, valid owner or HR or contractor record. |
| Dormant account | An account with no sign-in for 90 days. |
| Access recertification | A documented review in which an accountable person confirms that each access right is still needed. |
| shall / should / may | **shall** denotes a mandatory requirement; **should** a recommendation; **may** an optional action. |

# 4. Roles and Responsibilities

| Role | Responsibilities |
|---|---|
| Executive Leadership Team | Shall approve this Policy, resource its implementation and receive quarterly access control reporting. |
| CISO (Policy Owner) | Shall own this Policy, approve privileged access and exceptions within delegated authority, oversee access reviews, and report KPIs and gaps to the Executive Leadership Team. |
| IT Department (Identity and Access Management team) | Shall operate the JML process and the access register, provision and remove access, run reconciliations and review reports, and maintain PAM, MFA, VPN, Zscaler and jump servers. |
| HR Department | Shall act as the authoritative source for workforce records and notify IT of joiners, movers and leavers within the deadlines in Table 2, including before an involuntary departure is communicated. |
| Line Managers | Shall request and approve access appropriate to team roles, tell HR and IT of changes immediately, and certify team access in reviews. |
| System and Data Owners | Shall define roles and approve access to their systems and data, certify access in reviews, and accept access risk. |
| Security Operations | Shall monitor access events, respond to alerts, review privileged activity and investigate suspected misuse. |
| Third-party sponsors | Shall justify, scope, approve and certify third-party access, and ask IT to remove it when no longer needed. |
| PayStream integration lead | Shall make sure PayStream identity stores follow this Policy and are inventoried, reconciled and aligned within the deadlines in Section 5.9. |
| All users | Shall protect their credentials and MFA devices, use only the access they are granted, and report suspected misuse or unneeded access. |
| Internal Audit | Shall independently test access control and review evidence at least annually. |

# 5. Policy Statements

## 5.1 Access Control Principles

**5.1.1** **Least privilege.** Users, service accounts and systems shall be given only the minimum access needed for their approved role or task, and only for the time needed. Access shall be denied unless it is explicitly granted.

**5.1.2** **Need-to-know.** Access to Confidential and Restricted information, including PHI and cardholder data, shall be granted only to people who need it for specific duties. Seniority is not a basis for access.

**5.1.3** **Separation of duties.** No one person shall be able to request, approve and implement the same access change, or to administer a system and also administer its audit logs. Incompatible duties shall be recorded in an SoD matrix, reviewed annually. Where separation is not feasible, compensating monitoring shall be approved by the CISO.

**5.1.4** **Role-based access.** Access shall be assigned through role templates approved by system owners. Access outside a template shall be separately justified and approved. Role templates shall be reviewed at least annually.

**5.1.5** **Individual accountability.** Every user shall have a unique identity, and every action shall be traceable to one person. Shared or generic accounts are prohibited, except documented service accounts under Section 5.3.

**5.1.6** **Documented authorization.** Every access grant or change shall be requested and approved in the IT service management (ITSM) system, by the line manager and the system or data owner. Verbal, email-only or unrecorded grants are not valid.

**5.1.7** **Central identity.** HR records shall be the authoritative source for employees and the contractor register for contractors. Applications shall use single sign-on through Entra ID wherever supported. Local application accounts shall be documented and included in access reviews.

**5.1.8** IAM shall maintain an access register listing every identity store, account, privileged role and entitlement, including those of PayStream Analytics.

**Table 1: Account Types and Minimum Controls**

| Account type | Approval | Authentication | Review | Maximum validity |
|---|---|---|---|---|
| Standard user | Manager and system owner | MFA through SSO | Semi-annual | While employed |
| Privileged | System owner and CISO | Phishing-resistant MFA; PAM | Quarterly | JIT, 8 hours per elevation |
| Service | System owner and CISO delegate | Vaulted secret; no interactive login | Quarterly | Until owner or purpose changes |
| Third party / contractor | Sponsor, system owner and CISO delegate | MFA; ZTNA or gateway | Quarterly | 90 days, renewable |
| Break-glass | CISO | Sealed credentials; alert on use | Quarterly test | Per use |
| Shared | Prohibited | Not applicable | Not applicable | Not applicable |

## 5.2 User Registration and De-registration (Joiner, Mover, Leaver)

**5.2.1** NexusGuard shall operate a formal JML process, owned by IAM and documented in the User Access Provisioning Procedure (PRC-IAM-001). HR shall trigger it, so that no account is created, changed or retained without a current HR or contractor record.

### Joiners (registration)

**5.2.2** Access shall be granted only after identity verification, completion of pre-employment screening, and signed acknowledgment of the Acceptable Use Policy. Access to PHI or cardholder data requires completion of the relevant role-based training first.

**5.2.3** Accounts shall be created disabled, no earlier than five business days before the start date, and enabled on the start date. Access shall be assigned from the role template. Initial credentials shall be unique, delivered securely and changed on first use, and MFA enrolled at first sign-in.

**5.2.4** Provisioning shall be completed within three business days of an approved request.

### Movers (change of role)

**5.2.5** A change of role, department or location shall trigger an access review. New access shall be approved under Section 5.1.6, and access no longer needed shall be removed within five business days of the effective date, and privileged access within one business day. Retaining old access "just in case" is prohibited.

**5.2.6** Temporary moves, secondments and cover shall have an end date, after which access expires automatically and shall not exceed 90 days without re-approval.

### Leavers (de-registration)

**5.2.7** HR shall notify IAM of a departure as soon as the leaving date is known, and for an involuntary or high-risk departure before the person is informed.

**5.2.8** For standard departures, all access shall be disabled by the end of the last working day, and in any case within 24 hours of the termination effective date. For involuntary or high-risk departures, all access shall be disabled immediately, at or before the time the person is informed.

**5.2.9** At departure, IAM shall remove access to PAM, VPN and ZTNA, cloud, SaaS and third-party portals, de-register MFA devices, and rotate within 24 hours any shared secret known to the leaver. Managers shall recover devices, badges and tokens. Mailbox and data shall be handed to the manager for 30 days, and not forwarded to personal accounts.

**5.2.10** Disabled leaver accounts shall be deleted after 90 days, in line with retention rules, and user IDs shall never be reused.

**5.2.11** Contractor and third-party accounts shall be created with a mandatory end date and shall expire automatically at that date.

### Detective controls

**5.2.12** IAM shall reconcile all identity stores (Active Directory, Entra ID, AWS IAM, SaaS applications, VPN and Zscaler, PAM, and PayStream directories) against HR and contractor records at least monthly. Any account without a current record or owner shall be disabled within two business days and investigated.

**5.2.13** Accounts with no sign-in for 90 days shall be disabled automatically, and deleted after a further 30 days unless the owner re-justifies them.

**5.2.14** When NexusGuard acquires or merges with another organization, IAM shall inventory the acquired identity stores within 30 days and shall disable the accounts of personnel who are not retained on the transition date.

**Table 2: Joiner, Mover and Leaver Service Levels**

| Event | Trigger and owner | Deadline |
|---|---|---|
| Joiner | HR ticket after confirmed hire and screening; manager approves | Account created disabled up to 5 business days before start; provisioned within 3 business days of approved request |
| Mover | HR ticket on role change; manager and owner approve | Old access removed within 5 business days (privileged: 1 business day) |
| Leaver, standard | HR notifies IAM when the date is known | Disabled by end of last working day, within 24 hours of termination date |
| Leaver, involuntary or high risk | HR notifies IAM before the person is informed | Disabled immediately |
| Contractor / third party | Sponsor request with end date | Expires at end date; maximum 90 days before renewal |
| Reconciliation | IAM against HR, contractor and vendor records | Monthly; orphan accounts disabled within 2 business days |
| Dormant account | Automatic | Disabled after 90 days without sign-in |

## 5.3 Privileged Access Management

**5.3.1** Privileged access shall be granted only to named individuals, with a documented business justification approved by the system owner and the CISO or delegate, at the lowest effective privilege level.

**5.3.2** Privileged users shall have a separate privileged account, and shall not use it for email, web browsing or routine work.

**5.3.3** Standing privilege shall be minimized. Elevated rights shall be granted just in time through the PAM solution, with approval, a ticket reference, a maximum duration of 8 hours and automatic expiry. Any standing privileged role shall be listed in the privileged access register with CISO approval.

**5.3.4** Privileged credentials, including service, database, application and cloud root and global administrator credentials, shall be held in the PAM vault, checked out with MFA, and rotated after each check-out or at least every 90 days.

**5.3.5** Administrative access to servers, network devices, databases and production cloud environments shall be made only through PAM and jump servers (Section 5.5).

**5.3.6** Privileged sessions on Critical systems and systems holding Restricted data shall be recorded, and recordings retained for 12 months.

**5.3.7** Break-glass accounts shall be limited to two per platform, with sealed credentials under dual control. Each use shall raise an immediate alert, be reviewed within one business day, and be followed by a password change. Break-glass accounts shall be tested quarterly.

**5.3.8** Service accounts shall have a named owner, a documented purpose and least privilege, shall not permit interactive sign-in, and shall be reviewed quarterly.

**5.3.9** Local administrator rights shall be removed from standard users. Exceptions shall be approved, time-limited and logged.

**5.3.10** IAM shall maintain a privileged access register, reconcile it monthly against system data, and recertify it quarterly with system owners and the CISO. Privileged users shall complete role-based security training each year.

## 5.4 Authentication and Passwords

**5.4.1** Authentication shall follow NIST SP 800-63B, as set out in Table 3. Where PCI DSS, HIPAA or a client contract is stricter, the stricter requirement shall apply.

**5.4.2** Passwords and passphrases shall be at least 12 characters for standard accounts and at least 16 characters for privileged, service and break-glass accounts. Systems shall accept at least 64 characters, including spaces, and shall not impose composition rules such as mandatory symbols. Pasting and password managers shall be allowed.

**5.4.3** New passwords shall be checked against a blocklist of breached, common, dictionary and context-specific passwords (such as the user name or "NexusGuard").

**5.4.4** Passwords shall not be forced to change on a fixed schedule. They shall be changed immediately on evidence or suspicion of compromise, or where a regulation or contract requires it (for example PCI DSS 8.3.9 where passwords are the only factor).

**5.4.5** Password hints and knowledge-based security questions are prohibited. Passwords shall be stored only as salted hashes using approved algorithms and sent only over encrypted channels. Default and vendor passwords shall be changed before deployment, and credentials shall not be hard-coded in code or scripts.

**5.4.6** Accounts shall lock after no more than 10 failed attempts for at least 30 minutes, or until released by an administrator who has verified the user's identity.

**5.4.7** **MFA mandate.** MFA shall be enforced for: all remote access; all cloud and SaaS access through SSO, including Microsoft 365 and email; all privileged access; all access to systems holding PHI or cardholder data; PAM, VPN and Zscaler; and all third-party access. No account shall be exempt from MFA except under an approved exception.

**5.4.8** Approved authenticators are FIDO2 security keys, platform authenticators and authenticator apps with number matching. SMS and voice codes may be used only as a temporary fallback for standard users and are prohibited for privileged, break-glass and Restricted-system access. Email codes shall not be the only second factor.

**5.4.9** Users shall register at least two MFA methods. MFA resets shall require identity verification by the service desk and manager approval. Users shall report unexpected MFA prompts, and repeated prompts shall raise an alert.

**5.4.10** Conditional access shall check device compliance, location and sign-in risk. Sessions on privileged and Restricted systems shall require re-authentication after 15 minutes of inactivity, other systems after 30 minutes, and no session shall last longer than 12 hours.

**Table 3: Authentication Requirements**

| Requirement | Standard accounts | Privileged, service and break-glass |
|---|---|---|
| Minimum length | 12 characters | 16 characters |
| Composition rules | None; blocklist screening applies | None; blocklist screening applies |
| Scheduled rotation | None; change on compromise | Vault rotation after use or every 90 days |
| MFA | Required (remote, cloud, SSO, PHI, CDE) | Always; phishing-resistant for domain, cloud and PAM admins |
| Failed attempt lockout | 10 attempts, 30 minutes | 10 attempts, 30 minutes |
| Idle re-authentication | 30 minutes (15 for Restricted systems) | 15 minutes |
| SMS or voice as second factor | Temporary fallback only | Prohibited |

## 5.5 Remote Access Controls

**5.5.1** Remote access to internal systems shall use only approved methods: Zscaler Private Access (ZTNA) by default, the corporate VPN where ZTNA is not supported, and jump servers for administration. Management interfaces such as RDP, SSH and database ports shall not be exposed directly to the internet.

**5.5.2** Remote access shall require MFA and a compliant, managed device: enrolled, encrypted, running endpoint protection, patched and not jailbroken. Non-compliant devices shall be blocked. Personal devices shall follow the Acceptable Use Policy and shall never connect directly to the internal network.

**5.5.3** Internet traffic from managed devices shall be routed through Zscaler Internet Access, on or off the network, with threat protection and data loss prevention. Users shall not disable or bypass the Zscaler client.

**5.5.4** Remote access shall be granted per application, not to the whole network. Split tunneling shall be disabled for access to Restricted environments. VPN and ZTNA sessions shall end after 12 hours or after the idle limit in Section 5.4.10.

**5.5.5** Jump servers shall be dedicated, hardened and patched, placed in a management network segment, reachable only through ZTNA or VPN with MFA, and shall have no internet or email access and no data storage. All administrative sessions shall start from a jump server, be recorded, and have logs sent to the SIEM. Separate jump servers shall be used for PHI and cardholder environments, and for PayStream until integration is complete. Jump server access lists shall be reviewed quarterly.

**5.5.6** Remote access shall be allowed only from approved countries. Access from other countries requires prior approval, and impossible-travel sign-ins shall raise an alert.

**5.5.7** Remote control and remote desktop tools (such as TeamViewer or AnyDesk) are prohibited unless approved by Security. Remote access configuration shall be reviewed at least every six months.

## 5.6 Third-Party and Contractor Access

**5.6.1** Third-party access shall be granted only after a contract with security and confidentiality terms is in place, a HIPAA Business Associate Agreement before any PHI access, and a data processing agreement where personal data is involved. Each third party shall have a NexusGuard sponsor.

**5.6.2** Sponsors shall justify the access, define its scope and end date, approve each request, certify the access every quarter, and tell IAM when it is no longer needed. Sponsors are accountable for third-party access.

**5.6.3** Each third-party individual shall have a unique, named, clearly marked external account. Shared vendor accounts are prohibited.

**5.6.4** Third-party access shall be least privilege and limited to named systems. Privileged third-party access shall be just in time through PAM, with recorded sessions. Access to Restricted data requires data owner approval and CISO sign-off.

**5.6.5** Third-party accounts shall expire after 90 days unless the sponsor renews them, shall be disabled automatically at expiry, and shall be removed immediately when the contract ends.

**5.6.6** Third parties shall connect through ZTNA or an approved vendor gateway with MFA and, for administration, through jump servers. Vendor support sessions shall be started and supervised by NexusGuard staff.

**5.6.7** Third parties shall notify NexusGuard within one business day when their personnel with NexusGuard access leave or change roles, shall confirm their personnel list each quarter, and shall screen their personnel to the standard in their contract.

**5.6.8** IAM shall keep a third-party access register (who, system, sponsor, expiry) and the Security Operations team shall monitor third-party activity.

## 5.7 Access Reviews

**5.7.1** **Quarterly reviews are mandatory** for: all privileged accounts; all access to systems holding PHI, cardholder data or other Restricted information; all service and third-party accounts; Critical systems; and VPN, ZTNA and cloud administrative roles. All other access shall be reviewed at least every six months (Table 4).

**5.7.2** IAM shall generate entitlement reports directly from the systems, not compile them by hand, within the first five business days of each quarter, and reviews shall be completed within 15 business days.

**5.7.3** Line managers shall review their team's access, system and data owners shall review application and role membership, the CISO or delegate shall review privileged access, and sponsors shall review third-party access. No one shall review their own access.

**5.7.4** Reviewers shall mark each entitlement keep, modify or revoke, and shall give a justification for retaining privileged access. Blanket approval is not acceptable, and IAM shall sample completed reviews for quality.

**5.7.5** Reviews not completed in time shall be escalated to the reviewer's director after 10 business days and to the CISO after 15. Privileged and Restricted access not reviewed within 20 business days shall be suspended.

**5.7.6** Revocations shall be carried out within five business days, and privileged access within one business day, and IAM shall verify completion.

**5.7.7** Review records, including entitlements reviewed, decisions and evidence of removal, shall be kept for at least six years. The CISO shall report completion, revocation rates and overdue items to the Executive Leadership Team each quarter.

**5.7.8** Extra reviews shall be carried out after a security incident, a reorganization or an acquisition. System owners shall review role templates and the SoD matrix annually.

**Table 4: Access Review Schedule**

| Population | Frequency | Reviewer |
|---|---|---|
| Privileged and break-glass accounts | Quarterly | System owner and CISO or delegate |
| Systems holding PHI, cardholder data or Restricted information | Quarterly | Data owner and line managers |
| Service accounts | Quarterly | System owner |
| Third-party and contractor accounts | Quarterly | Sponsor |
| VPN, ZTNA, jump server and cloud admin access | Quarterly | IAM and CISO delegate |
| All other user access | Semi-annual | Line managers and system owners |

## 5.8 Logging and Monitoring of Access Events

**5.8.1** The following shall be logged: successful and failed sign-ins; account creation, change, disablement and deletion; group and role membership changes; privileged elevation and PAM check-outs; privileged session activity; MFA enrollment, reset and bypass events; remote access sessions; access to systems holding PHI and cardholder data; lockouts and password resets; and changes to access control settings.

**5.8.2** Logs shall be sent to the central SIEM, time-synchronized and protected from alteration. Administrators shall not be able to change or delete logs of their own activity.

**5.8.3** Access logs shall be retained for 12 months, with the most recent three months immediately available. Access requests, approvals and review records shall be retained for six years.

**5.8.4** Security Operations shall maintain alerts for at least: creation of privileged accounts; additions to privileged groups; break-glass use; sign-ins to disabled or dormant accounts; repeated failures and lockouts; impossible travel and non-approved countries; off-hours privileged use; MFA changes and repeated MFA denials; and new accounts with no HR record.

**5.8.5** Privileged activity shall be reviewed weekly. Failed sign-ins, lockouts and dormant accounts shall be reviewed monthly. Access to systems holding PHI shall be reviewed at least monthly as required by the HIPAA information system activity review.

**5.8.6** Access to logs shall be limited to Security Operations and auditors. Suspected misuse shall be handled under the incident management requirements of the Information Security Policy, and a suspected compromised account shall be disabled immediately.

**5.8.7** Monitoring of staff activity shall follow the notice and safeguards in the Acceptable Use Policy.

## 5.9 Transitional Requirements

**5.9.1** All active accounts of former PayStream Analytics personnel who are not current employees or approved contractors, including the eight identified in the internal review, shall be disabled immediately, and their activity since departure shall be reviewed as a potential security incident.

**5.9.2** All existing privileged access, including the 42 users identified in the internal review, shall be recertified within 30 days of the Effective Date. Access not re-justified shall be removed.

**5.9.3** The JML process in Section 5.2 shall be in operation, with HR notifications integrated with ITSM, within 30 days of the Effective Date.

**5.9.4** A baseline access review of all systems holding PHI, and a full reconciliation of identity stores against HR records, shall be completed and evidenced before HIPAA client onboarding goes live.

**5.9.5** PayStream identity stores shall be inventoried, reconciled and either integrated into NexusGuard identity services or brought into line with this Policy within 90 days of the Effective Date.

**5.9.6** The CISO shall report progress against Section 5.9 weekly to the executive sponsor until all items are closed, and the Executive Leadership Team shall be informed of any item that will miss its deadline.

# 6. Compliance

This Policy supports the requirements in Table 5. References are paraphrased pointers; the source text of each requirement prevails.

**Table 5: Compliance Basis**

| Regime | Key provisions supported | Policy sections |
|---|---|---|
| ISO/IEC 27001:2022 | A.5.3 segregation of duties; A.5.15 access control; A.5.16 identity management; A.5.17 authentication information; A.5.18 access rights; A.5.19 to A.5.22 supplier relationships; A.6.5 responsibilities after termination or change; A.6.7 remote working; A.8.2 privileged access rights; A.8.3 information access restriction; A.8.5 secure authentication; A.8.15 and A.8.16 logging and monitoring | 5.1 to 5.8 |
| HIPAA | 164.308(a)(3) workforce security, including authorization and termination procedures; 164.308(a)(4) information access management; 164.308(a)(1)(ii)(D) activity review; 164.312(a) access control, unique user ID and automatic logoff; 164.312(b) audit controls; 164.312(d) person or entity authentication; 164.308(b) business associates | 5.1 to 5.8 |
| PCI DSS v4.0 | Requirement 7 (7.2.1 access model, 7.2.4 account review, 7.2.5 system accounts); Requirement 8 (8.2.1 unique IDs, 8.2.4 account changes, 8.2.5 terminated users, 8.2.6 inactive accounts, 8.3 authentication, 8.4 MFA); Requirement 10 logging | 5.2 to 5.8 |
| GDPR / UK GDPR | Art. 5(1)(f) integrity and confidentiality; Art. 25 data protection by design; Art. 32(1)(b) and 32(4) security and staff acting only on instruction | 5.1, 5.2, 5.7 |
| NIST CSF 2.0 and SP 800-63B | PR.AA-01 to PR.AA-05 identities, credentials, authentication and access permissions including least privilege and SoD; DE.CM-03 monitoring; SP 800-63B authenticator and password guidance | 5.1 to 5.8 |
| UAE NESA | Access control and human resources security control families | 5.1 to 5.8 |

# 7. Enforcement and Sanctions

**7.1** Compliance with this Policy is mandatory. Violations shall be handled under the HR disciplinary procedure and the tiered sanctions in the Acceptable Use Policy, up to and including termination of employment or engagement, and shall comply with applicable employment law.

**7.2** The following are serious violations: sharing credentials or MFA devices; using another person's account; granting or approving access without authorization; bypassing PAM, jump servers or MFA; and concealing unneeded or unauthorized access.

**7.3** Line managers, sponsors and HR staff who fail to request or process access removal within the deadlines in Table 2, and IAM staff who fail to action it, are accountable and may face disciplinary action.

**7.4** Third parties who breach this Policy shall have access suspended and remedies applied under their contracts.

# 8. Exceptions

**8.1** Exceptions to this Policy shall be requested through the Policy Exception Management Process and shall be formally requested in writing, with a business justification, a risk assessment and compensating controls.

**8.2** Exceptions shall be approved by the CISO for Low and Medium risk and by the Executive Leadership Team for High or Critical risk, shall be time-limited to no more than six months, and shall be recorded and reviewed before expiry.

**8.3** No exception shall be granted to the MFA mandate for privileged or remote access, to the leaver deadlines in Section 5.2, or to a legal or contractual requirement, unless Legal confirms in writing that it is permitted.

# 9. Related Documents

| Document | ID | Type |
|---|---|---|
| Information Security Policy | POL-ISP-001 | Policy |
| Acceptable Use Policy | POL-AUP-001 | Policy |
| Data Classification and Handling Policy | POL-DCH-001 | Policy |
| Incident Response Policy and Plan | POL-IRP-001 | Policy |
| Third-Party Security Policy | POL-TPS-001 | Policy |
| Password and Authentication Standard | STD-IAM-001 | Standard |
| Privileged Access Management Standard | STD-PAM-001 | Standard |
| User Access Provisioning Procedure (JML) | PRC-IAM-001 | Procedure |
| Policy Exception Management Process | PRC-GRC-001 | Procedure |
| Secure Remote Working Guide | GDL-REM-001 | Guideline |

_Document IDs are proposed identifiers under the policy framework. PRC-IAM-001 replaces the placeholder PRC-HRS-001 listed in the Information Security Policy. Confirm all IDs against the document register._

# 10. Review

This policy shall be reviewed annually or when significant changes occur. The Policy Owner initiates the review.

**10.1** The CISO shall also review this Policy after a serious access-related incident, a significant audit finding, a change in law or client requirements, or an acquisition.

**10.2** The approved version shall be published in the controlled document repository and communicated to all personnel and third parties in scope. Superseded versions shall be archived for at least six years.
