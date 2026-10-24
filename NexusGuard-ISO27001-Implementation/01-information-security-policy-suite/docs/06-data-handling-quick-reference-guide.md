# NexusGuard Technologies Ltd. | Data Handling Quick Reference Guide | GDL-DCH-001

## DATA HANDLING QUICK REFERENCE

_Classify it. Label it. Handle it by tier._

### Step 1: Which tier is it?

Go from the top. Stop at the first "yes".

| Tier | Ask yourself |
|---|---|
| **Restricted** | Contains **PHI**, **payment card data**, special category or government ID data, **credentials, keys or secrets**? |
| **Confidential** | Contains **employee PII**, **source code**, client contracts or pricing, security reports, financials, network diagrams? |
| **Internal** | For NexusGuard staff and approved partners only, and not any of the above? |
| **Public** | Approved by Marketing and Communications for release to anyone? |

### Step 2: Handle it

| | Public | Internal | Confidential | Restricted |
|---|---|---|---|---|
| **Label** | None needed | "Internal" (default if unlabeled) | **"NexusGuard Confidential"** in header or footer, M365 label, [CONFIDENTIAL] email tag | **"NexusGuard Restricted"** on every file, [RESTRICTED] email tag, red media label |
| **Store in** | Any approved system | Approved systems (Microsoft 365, approved SaaS) | Approved, encrypted systems; no USB without approval | **Only systems approved for Restricted data**; no local copies; no printing |
| **Send by** | Any channel | Company email and approved tools | Encrypted email or secure share with named access; **no public links** | **Encrypted channels between approved systems only**; never chat, SMS or plain email |
| **Destroy by** | Delete or recycle | Delete; secure shred bin | Secure delete; cross-cut shred; media wiped | **Cryptographic erase or NIST 800-88**; certificate; shred to P-5 |

### The four data types you meet most

**PHI (patient health records)** (Tier: Restricted)

- Minimum necessary only; a BAA must exist first
- Never on personal devices, USB or AI tools
- Never in email subjects, chat or tickets

**Payment card data** (Tier: Restricted)

- PAN unreadable wherever stored; mask on screen
- Never store security codes (CVV) or PINs
- Never send PAN by email or chat

**Employee PII** (Tier: Confidential)

- HR systems only; need-to-know access
- Special category, ID and bank details are Restricted
- Follow the retention schedule

**Source code** (Tier: Confidential)

- Approved repository only, with MFA and code review
- No secrets, keys or live PHI or card data in code
- Not in personal repos, email or unapproved AI tools

### Always and never

| ALWAYS | NEVER |
|---|---|
| Label Confidential and Restricted files | Send work data to personal email, cloud or devices |
| Check the recipient before you press send | Put PHI or card data in chat, tickets or AI tools |
| Lock your screen; keep paper locked away | Use USB drives without written approval |
| Classify one tier higher if unsure, then ask the data owner or DPO | Remove or lower a label to get around a control |

**Sending data abroad?** Ask the DPO or Legal first. PHI stays in the regions in the client contract. EU and UK personal data needs a lawful transfer mechanism.

**Keep only what you need.** Follow the Records Retention Schedule. Never keep copies on desktops, personal drives or old mailboxes. Destroy securely when the period ends.

**Lost, misdirected or exposed data? Report it within 1 hour** through the incident reporting channel. Honest, prompt reports are protected from retaliation.

---

_Full policy: Data Classification and Handling Policy POL-DCH-001 v1.0  |  Quick Reference GDL-DCH-001  |  Classification: Internal  |  Questions: ask the data owner, DPO or Security_
