# NexusGuard Technologies Ltd. | Memo: USB Device Request Decisions | MEM-USB-2026-001

| Field | Detail |
|---|---|
| **To** | Chief Information Security Officer (CISO) |
| **From** | Augustine Ozor, GRC Analyst |
| **Date** | 13/10/2026 |
| **Subject** | Evaluation of three USB device requests (USB-2026-001 to USB-2026-003) |
| **Action needed** | Approve two time-limited exceptions; note one denial; decide on the recommendations below |

# 1. Decisions

| Request | Data and route | Decision | Risk (inherent to residual) | Key condition |
|---|---|---|---|---|
| 1. Developer | 2 GB source code (Confidential) to an air-gapped test environment | **Approve with conditions** | High 12 to Medium 6 | Company-issued encrypted USB; secrets scan; malware scan; one transfer in 5 business days |
| 2. Marketing Manager | Client contract presentation (Confidential) from home on a personal USB | **Deny** | High 12 to Low 2 | Use Microsoft 365 sharing on a managed laptop; check whether the file is already on a personal device |
| 3. Database Administrator | Scripts with connection strings (Restricted) between production and DR sites | **Approve with conditions** (30-day bridge) | High 15 to Medium 8 | No credentials on the media; show the network route is unavailable; recorded PAM sessions; two-person custody |

_Decisions apply ISP POL-ISP-001, ACP POL-ACC-001 and AUP POL-AUP-001. The Data Classification and Handling Policy (POL-DCH-001) is not yet issued, so ISP 5.4 and Table 3 supplied the classifications. Full reasoning, clauses and conditions are in the three evaluation forms._

# 2. Overall Risk Considerations

- **Need, not status, decides.** Request 1 shows that a "Restricted" clearance does not widen what can be copied or waive controls (ACP 5.1.2). Request 3 shows that a signed PAM agreement does not authorize removable media.
- **Credentials in scripts is the biggest finding.** Request 3 exposes a practice that breaches ISP 5.6.6 and ACP 5.4.5 and probably exists in other scripts. If a USB holding credentials were lost, the exposure would reach PHI.
- **Personal media is the weakest link.** Request 2 would bring unmanaged media into a corporate workstation, and may mean a client contract is already on a personal device. Approved file sharing meets the need.
- **Policy gap.** ISP 5.7.7 is the only removable media rule. There is no managed USB pool, scan station or technical device control, so every request depends on manual checks.
- **Exception hygiene.** Both approvals are time-limited exceptions that must go in the exception register and expire (ISP 8.2).

# 3. Recommendations

- Approve the exceptions for USB-2026-001 and USB-2026-003 on the stated conditions, and note the denial of USB-2026-002.
- Direct Security to scan scripts and configuration files for embedded credentials and move secrets to the PAM vault.
- Issue a Removable Media Standard, with a pool of registered encrypted devices, an IT scan and wipe station, and endpoint device control that blocks unregistered USB devices.
- Issue the Data Classification and Handling Policy so that future evaluations can cite its clauses directly.
- Remind staff of approved file sharing and the BYOD route through awareness communications.

I am available to brief the requesters and managers on the decisions.
