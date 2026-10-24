# NexusGuard Technologies Ltd. | USB Device Request Evaluation Form | USB-2026-003

| Field | Detail |
|---|---|
| **Request ID** | USB-2026-003 |
| **Date of evaluation** | 13/10/2026 |
| **Requester** | Database Administrator, IT (holds privileged access; signed PAM agreement) |
| **Evaluated by** | Augustine Ozor, GRC Analyst |
| **Device requested** | USB storage device (type and ownership not stated) |
| **Data involved** | Encrypted backup verification scripts that contain database connection strings |
| **Classification (ISP Table 3)** | Restricted until credentials are removed (ISP Table 3 lists credentials as Restricted). Confidential once the scripts hold no secrets. |
| **Source and destination** | Production data center (AST-031) to the disaster recovery site (AST-032) |
| **Business justification (as stated)** | The DBA needs to carry backup verification scripts between the production data center and the DR site. |
| **DECISION** | APPROVE WITH CONDITIONS (short-term bridge) |
| **Approval validity** | 30 days from CISO approval, for the named scripts only. Not renewable without a new request. |

# 1. Request Summary

A database administrator asks to move backup verification scripts between the production data center and the DR site on USB. The scripts contain database connection strings, which normally include account names and often passwords. The DBA is trusted and has signed a PAM agreement, but that agreement covers privileged access, not removable media. The weakness is that credentials sit inside scripts, which policy prohibits, and the production databases hold PHI.

# 2. Applicable Policy Clauses

| Policy and clause | What it requires | How it applies to this request |
|---|---|---|
| ISP 5.7.7 | Removable media is blocked by default. Exceptions need approval and encryption. | The request is an exception and needs an encrypted, registered device. |
| ISP Table 3 and 5.4.3 | Credentials are Restricted and may be held only in approved systems. | Scripts holding credentials are Restricted and carry the highest handling requirements. |
| ISP 5.6.6 and ACP 5.4.5 | Credentials and secrets are never embedded in source code, scripts or configuration. | The scripts breach this today, so credentials shall be removed before any transfer. |
| ACP 5.3.4 and 5.3.1 | Privileged credentials are held in the PAM vault and checked out with MFA. Privileged access is justified and approved. | The scripts shall fetch secrets from the vault at run time. The PAM agreement does not authorize USB use. |
| ACP 5.3.5 and 5.3.6 | Administration runs through PAM and jump servers, with sessions recorded. | Running the scripts shall use recorded PAM sessions. |
| ACP 5.1.3 and 5.1.6 | No self-approval. Approvals are recorded in ITSM. | Manager, database owner and CISO approvals are required. |
| ISP 5.6.4 and 5.6.7 | Confidential and Restricted data on removable media is encrypted; DLP monitors transfers. | The device is hardware-encrypted and the copy is monitored. |
| ISP 5.4.4 and 5.12.1 | Media is sanitized to NIST SP 800-88. Losses are reported within 1 hour. | The device is wiped after use and any loss reported at once. |
| ISP 8.1 to 8.3 | Exceptions are risk-assessed, time-limited and approved. | The CISO approves a 30-day exception. |
| AUP 5.7.1 (Table 1) | Copying data to USB is a prohibited activity unless approved. | The transfer is permitted only through this exception. |

_ISP = Information Security Policy POL-ISP-001 v3.0; ACP = Access Control Policy POL-ACC-001 v1.0; AUP = Acceptable Use Policy POL-AUP-001 v1.0. The Data Classification and Handling Policy (POL-DCH-001) has not yet been issued, so data classification is taken from ISP clause 5.4 and Table 3, the scheme that policy will adopt._

# 3. Risk Assessment

| Threat | Vulnerability | Potential impact |
|---|---|---|
| Loss, theft or interception of the USB device in transit between sites; misuse of embedded credentials to reach production databases. | Credentials hard-coded in scripts; physical transport of removable media; a PAM agreement that does not cover removable media. The Information Asset Register shows a WAN link to the DR site, so a network route may exist. | Unauthorized access to production databases holding PHI, causing a possible HIPAA breach; loss of trust of healthcare clients; compromise of recovery capability. |

| Measure | Likelihood | Impact | Score |
|---|---|---|---|
| Inherent risk (as requested) | 3 Possible | 5 Severe | 15 High |
| Residual risk (with conditions) | 2 Unlikely | 4 Major | 8 Medium |

_Scoring uses a 5 x 5 scale (likelihood 1 Rare to 5 Almost certain; impact 1 Negligible to 5 Severe). Score = likelihood x impact: Low 1-4, Medium 5-9, High 10-16, Critical 17-25. Under ISP 5.3.3 a residual Medium risk is accepted by the CISO._

# 4. Decision and Justification

**Decision: APPROVE WITH CONDITIONS (short-term bridge).**

Approval is justified as a short bridge because both endpoints are NexusGuard-controlled facilities, backup verification is a legitimate resilience task, and the DBA is a vetted privileged user. Handled as a Restricted item, the risk falls from High to Medium, which the CISO can accept under ISP 5.3.3.

Two conditions are non-negotiable. First, no credentials may be on the device. If they cannot be removed, the request is denied. Second, the DBA shall show that the approved network route is not available, and if it is, that route shall be used and this approval lapses. The approval lasts 30 days so that the root cause, secrets in scripts, is fixed rather than accommodated.

# 5. Conditions of Approval

| # | Condition | Policy basis | Owner |
|---|---|---|---|
| 1 | **No credentials on the media.** Rewrite connection strings to use PAM vault references or short-lived tokens. A second person (DBA lead or Security) confirms with a secrets scan before copying. | ISP 5.6.6; ACP 5.4.5, 5.3.4 | DBA; Security |
| 2 | **Necessity.** The DBA records in ITSM why transfer over the site-to-site link through a jump server is not possible, and Security confirms. If the network route is available, it shall be used and this approval lapses. | ISP 5.7.7; ACP 5.5.5 | DBA; Security |
| 3 | Use only a company-issued, hardware-encrypted (AES-256) USB device registered in the asset register. Sign and encrypt the scripts with keys held in the vault. | ISP 5.6.4, 5.6.6 | IT; DBA |
| 4 | Run the scripts only inside PAM-controlled, recorded sessions through a jump server, on both production and DR systems. | ACP 5.3.5, 5.3.6 | DBA; Security |
| 5 | Carry the device in a tamper-evident pouch, directly between sites, never unattended. Record the hand-off at both locations in a chain-of-custody log signed by two people. | ISP 5.7.1; ACP 5.1.3 | DBA; Facilities |
| 6 | Scan the device for malware and verify file hashes at both ends. Log the file copy through endpoint DLP for Security Operations review. | ISP 5.9.1, 5.6.7 | IT; Security Operations |
| 7 | Valid for 30 days for the named scripts only. Within that time IT and the DBA shall replace the USB route with a secure network or vault-based transfer. Record the exception in the exception register. | ISP 8.2 | GRC; CISO; IT |
| 8 | Record approvals in ITSM from the line manager, database owner and CISO. The DBA shall not approve their own request. | ACP 5.1.3, 5.1.6 | Manager; Owner; CISO |
| 9 | Wipe the device to NIST SP 800-88 after each use and log it. Report any loss within 1 hour; it shall be assessed as at least Severity 2. | ISP 5.4.4, 5.12.1 | IT; DBA |

_Related action: Security shall scan other scripts and configuration files for embedded credentials, because the same practice is likely elsewhere._

# 6. Sign-off

| Role | Name | Decision | Signature and date |
|---|---|---|---|
| Requester |  | Acknowledges conditions |  |
| Line manager |  | Approve / Decline |  |
| Database owner |  | Approve / Decline |  |
| GRC Analyst (evaluator) | Augustine Ozor | Approve with conditions |  |
| CISO |  | Approve exception |  |

_Approved conditional requests are policy exceptions under ISP clause 8 and ACP clause 8. They shall be recorded in the exception register with an expiry date. This form and its approvals shall be kept for at least six years._
