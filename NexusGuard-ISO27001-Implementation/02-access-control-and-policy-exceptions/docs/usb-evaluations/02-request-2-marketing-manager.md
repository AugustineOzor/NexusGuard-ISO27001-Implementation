# NexusGuard Technologies Ltd. | USB Device Request Evaluation Form | USB-2026-002

| Field | Detail |
|---|---|
| **Request ID** | USB-2026-002 |
| **Date of evaluation** | 13/10/2026 |
| **Requester** | Marketing Manager, Marketing |
| **Evaluated by** | Augustine Ozor, GRC Analyst |
| **Device requested** | Personal USB drive (owned by the employee, unmanaged) |
| **Data involved** | Client presentation containing client logos and contract details |
| **Classification (ISP Table 3)** | Confidential (client contract details) |
| **Source and destination** | From the employee's home to a company office workstation |
| **Business justification (as stated)** | The employee wants to bring the presentation to the office from home on a personal USB drive. |
| **DECISION** | DENY |
| **Approval validity** | Not applicable. A new request may be submitted if the facts change. |

# 1. Request Summary

A marketing manager asks to use a personal USB drive to bring a client presentation, which includes contract details, from home to an office workstation. The request reveals two issues: the file is on, or has passed through, a personal device outside NexusGuard control, and the proposed route puts unmanaged media into a corporate workstation. Approved alternatives already exist, so there is no case for an exception.

# 2. Applicable Policy Clauses

| Policy and clause | What it requires | How it applies to this request |
|---|---|---|
| ISP 5.7.7 | Removable media is blocked by default. Exceptions need approval and encryption. | A personal drive cannot be registered, managed or verified as encrypted, so it cannot qualify for an exception. |
| ISP 5.4.2 and Table 3 | Client contracts are Confidential and need encryption and need-to-know handling. | The contract details must stay in approved, managed systems. |
| ISP 5.6.4 | Confidential data on removable media is encrypted with AES-256. | A personal drive offers no assurance of encryption. |
| ISP 5.4.5 | Assets are for business use. Confidential or Restricted information shall not be placed in unapproved cloud storage or AI tools. | Copies of the contract on a home computer or personal cloud sit outside approved storage. |
| AUP 5.7.1 (Table 1) | Copying data to USB or personal devices, and introducing unapproved media, are prohibited. | The proposed transfer falls directly within the prohibited data exfiltration activity. |
| AUP 5.3.3 and 5.8.1 | Work data stays in managed containers or company devices, and remote work uses company-owned or enrolled devices. | Work on a home device outside the managed container is not permitted. |
| AUP 5.6.1 and 5.6.4 | Only approved services are used for work data. Personal cloud storage is prohibited. | Approved file sharing (Microsoft 365) meets the need. |
| ACP 5.1.1 and 5.5.1 | Least privilege, and remote access only through ZTNA or VPN from compliant managed devices. | Staff can reach the file securely from a managed laptop. No removable media is needed. |
| ISP 5.12.1 and AUP 5.11.1 | Suspected incidents are reported within 1 hour of discovery. | If the file already sits on a personal device, that shall be reported. |

_ISP = Information Security Policy POL-ISP-001 v3.0; ACP = Access Control Policy POL-ACC-001 v1.0; AUP = Acceptable Use Policy POL-AUP-001 v1.0. The Data Classification and Handling Policy (POL-DCH-001) has not yet been issued, so data classification is taken from ISP clause 5.4 and Table 3, the scheme that policy will adopt._

# 3. Risk Assessment

| Threat | Vulnerability | Potential impact |
|---|---|---|
| Malware entering the corporate workstation from an unmanaged personal drive; leakage or loss of client contract details held on personal media or a home computer. | The drive is unmanaged and unencrypted. NexusGuard has no endpoint control, DLP or malware scanning on the home device. The file may already be outside approved systems. | Breach of client confidentiality and contract terms; malware on a corporate workstation; regulatory and reputational damage. |

| Measure | Likelihood | Impact | Score |
|---|---|---|---|
| Inherent risk (as requested) | 4 Likely | 3 Moderate | 12 High |
| Residual risk (approved alternative used) | 1 Rare | 2 Minor | 2 Low |

_Scoring uses a 5 x 5 scale (likelihood 1 Rare to 5 Almost certain; impact 1 Negligible to 5 Severe). Score = likelihood x impact: Low 1-4, Medium 5-9, High 10-16, Critical 17-25. Under ISP 5.3.3 a residual Medium risk is accepted by the CISO._

# 4. Decision and Justification

**Decision: DENY.**

The request is denied because the risk is High, no business need justifies it, and approved alternatives exist. ISP 5.7.7 allows an exception only for encrypted, approved media, and a personal drive cannot meet that test. The same work can be done securely through Microsoft 365 file sharing on a managed laptop over Zscaler or VPN.

The employee did the right thing by asking first. The denial is not a finding against them. The one open concern is that the file may already be stored on a personal device, which Security shall check (see actions below).

# 5. Approved Alternatives and Required Actions

| # | Action | Policy basis | Owner |
|---|---|---|---|
| 1 | Share the presentation through the approved Microsoft 365 service (SharePoint or OneDrive), using the company account with MFA, from a company laptop connected through Zscaler or VPN. | AUP 5.6.1; ACP 5.5.1 | Requester; IT |
| 2 | If offline transfer is truly unavoidable, submit a new request for a company-issued, hardware-encrypted USB device with manager approval, as in USB-2026-001. | ISP 5.7.7, 5.6.4 | Requester |
| 3 | If a personal device is needed for remote work in future, request BYOD enrollment so work data stays in the managed container. | AUP 5.3.1, 5.3.3 | Requester; IT |
| 4 | Security shall ask the requester whether the file is already on a personal drive, home computer or personal cloud. If so, record it as a Severity 3 event, have the copy securely deleted and confirmed, and scan the personal drive before any reuse. | ISP 5.12.1, Table 4; AUP 5.11.1 | Security Operations |
| 5 | Any breach found is handled under AUP Table 3. Prompt self-disclosure counts as mitigation (AUP 7.3). Give the requester a short refresher on approved file sharing. | AUP 7.3, Table 3 | HR; Line manager |

# 6. Sign-off

| Role | Name | Decision | Signature and date |
|---|---|---|---|
| Requester |  | Informed of decision |  |
| GRC Analyst (evaluator) | Augustine Ozor | Deny |  |
| CISO |  | Informed; appeal if raised |  |

_Approved conditional requests are policy exceptions under ISP clause 8 and ACP clause 8. They shall be recorded in the exception register with an expiry date. This form and its approvals shall be kept for at least six years._
