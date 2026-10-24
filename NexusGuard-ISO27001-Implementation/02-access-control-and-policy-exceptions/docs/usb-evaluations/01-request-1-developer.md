# NexusGuard Technologies Ltd. | USB Device Request Evaluation Form | USB-2026-001

| Field | Detail |
|---|---|
| **Request ID** | USB-2026-001 |
| **Date of evaluation** | 13/10/2026 |
| **Requester** | Software Developer, Product Engineering (holds "Restricted" clearance) |
| **Evaluated by** | Augustine Ozor, GRC Analyst |
| **Device requested** | USB storage device (type and ownership not stated) |
| **Data involved** | 2 GB of software source code |
| **Classification (ISP Table 3)** | Confidential (source code). Treated as Restricted if it contains credentials, keys or production data. |
| **Source and destination** | Developer workstation to an air-gapped testing environment with no network connectivity |
| **Business justification (as stated)** | The air-gapped test environment cannot receive files over a network, so the source code must be carried across on removable media. |
| **DECISION** | APPROVE WITH CONDITIONS |
| **Approval validity** | One transfer, within 5 business days of CISO approval. The approval then expires. |

# 1. Request Summary

A developer asks to copy 2 GB of source code to a USB device and load it into an air-gapped testing environment. The need is genuine: an isolated environment has no other way to receive the code. The main risks are malware crossing into the isolated environment, and loss or copying of source code. The developer's "Restricted" clearance describes the data they may access. It does not exempt them from removable media controls.

# 2. Applicable Policy Clauses

| Policy and clause | What it requires | How it applies to this request |
|---|---|---|
| ISP 5.7.7 | Removable media is blocked by default. Exceptions need approval and encryption. | The request is an exception. It can proceed only with approval and an encrypted device. |
| ISP 5.4.2 and Table 3 | Information is classified by its owner. Source code is Confidential. | The code is handled as Confidential, with encryption and need-to-know access. |
| ISP 5.6.4 | Confidential and Restricted data is encrypted at rest (AES-256), including on removable media. | The device must be hardware-encrypted. |
| ISP 5.6.6 | Keys, secrets and credentials are never embedded in source code. | The repository shall be scanned and any secrets removed before the copy. |
| ISP 5.9.8 | Live PHI or card data is not used in non-production unless masked. | The test environment shall not receive production data. |
| ISP 5.6.7 and 5.9.1 | Data loss prevention monitors transfers; endpoint protection runs on all endpoints. | The file copy shall be logged, and the media scanned for malware. |
| ISP 5.4.4 | Media is sanitized to NIST SP 800-88 before reuse. | The device shall be wiped after the transfer. |
| ISP 8.1 to 8.3 | Exceptions are risk-assessed, time-limited and approved (CISO for Low and Medium risk). | The CISO approves this time-limited exception. |
| ACP 5.1.1 and 5.1.2 | Least privilege and need-to-know. Seniority is not a basis for access. | The scope is limited to the named repository. Clearance alone does not justify wider copying. |
| ACP 5.1.3 and 5.1.6 | No one approves their own request. Approvals are recorded in ITSM by the manager and data owner. | The developer cannot self-approve. Approvals shall be recorded in ITSM. |
| AUP 5.7.1 (Table 1) | Copying data to USB and introducing unapproved software are prohibited activities. | The transfer is allowed only through this approved exception. |

_ISP = Information Security Policy POL-ISP-001 v3.0; ACP = Access Control Policy POL-ACC-001 v1.0; AUP = Acceptable Use Policy POL-AUP-001 v1.0. The Data Classification and Handling Policy (POL-DCH-001) has not yet been issued, so data classification is taken from ISP clause 5.4 and Table 3, the scheme that policy will adopt._

# 3. Risk Assessment

| Threat | Vulnerability | Potential impact |
|---|---|---|
| Malware carried into the isolated environment on removable media; theft, loss or unauthorized copying of source code. | Removable media bypasses network controls. The air-gapped environment has limited monitoring. An unencrypted or personal USB would expose code if lost. | Loss of intellectual property; compromised test environment and unreliable releases; damage to client trust. |

| Measure | Likelihood | Impact | Score |
|---|---|---|---|
| Inherent risk (before conditions) | 3 Possible | 4 Major | 12 High |
| Residual risk (with conditions) | 2 Unlikely | 3 Moderate | 6 Medium |

_Scoring uses a 5 x 5 scale (likelihood 1 Rare to 5 Almost certain; impact 1 Negligible to 5 Severe). Score = likelihood x impact: Low 1-4, Medium 5-9, High 10-16, Critical 17-25. Under ISP 5.3.3 a residual Medium risk is accepted by the CISO._

# 4. Decision and Justification

**Decision: APPROVE WITH CONDITIONS.**

Approval is justified because the business need is real, there is no network alternative, and the data is Confidential rather than Restricted. The conditions below bring the risk from High to Medium, which the CISO can accept under ISP 5.3.3.

Approval is limited in scope, time and method. It covers one named repository and one transfer, on a company-issued encrypted device. It does not create a standing right to use USB devices, and further transfers need a new request or a managed transfer process.

# 5. Conditions of Approval

| # | Condition | Policy basis | Owner |
|---|---|---|---|
| 1 | Use only a company-issued, hardware-encrypted (AES-256) USB device, registered in the asset register and signed out from IT. Personal or unregistered devices are prohibited. | ISP 5.7.7, 5.6.4 | IT; Developer |
| 2 | Limit the copy to the named repository and release. Scan it for secrets and remove credentials, keys, production data, PHI and card data before copying. The data owner confirms the contents in ITSM. | ISP 5.6.6, 5.9.8; ACP 5.1.2 | Data owner; Developer |
| 3 | Scan the device for malware at the IT scan station before it enters the air-gapped environment and again on return. Record a SHA-256 hash of the files and verify it at the destination. | ISP 5.9.1 | IT; Security |
| 4 | Approval is for one transfer within 5 business days. Recurring needs require a new request or a managed transfer process. Record the exception in the exception register. | ISP 8.2 | GRC; CISO |
| 5 | Record approvals in ITSM from the line manager and the data owner, and CISO approval of the exception. The developer shall not approve their own request. | ACP 5.1.3, 5.1.6; ISP 8.2 | Manager; Data owner; CISO |
| 6 | Log the file copy through endpoint DLP, and have Security Operations review it. Alert on any copy beyond the approved scope. | ISP 5.6.7; AUP 5.10 | Security Operations |
| 7 | Keep the device under the developer's control at all times, return it to IT within 1 business day, and report any loss within 1 hour. | AUP 5.2.4; ISP 5.12.1 | Developer |
| 8 | IT shall wipe the device to NIST SP 800-88 on return and log the wipe. Sign a chain-of-custody record at issue, transfer and return. | ISP 5.4.4 | IT |

# 6. Sign-off

| Role | Name | Decision | Signature and date |
|---|---|---|---|
| Requester |  | Acknowledges conditions |  |
| Line manager |  | Approve / Decline |  |
| Data owner (source code) |  | Approve / Decline |  |
| GRC Analyst (evaluator) | Augustine Ozor | Approve with conditions |  |
| CISO |  | Approve exception |  |

_Approved conditional requests are policy exceptions under ISP clause 8 and ACP clause 8. They shall be recorded in the exception register with an expiry date. This form and its approvals shall be kept for at least six years._
