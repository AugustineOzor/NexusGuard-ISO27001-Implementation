# NexusGuard RACI Matrix

R = Responsible, A = Accountable, C = Consulted, I = Informed. Every activity has exactly one A and at least one R.

| # | Activity | CISO | IT Security Manager | GRC Analyst | Risk Manager | Compliance Officer | IT Operations Manager | Internal Auditor | Data Protection Officer | Business Unit Lead | System Administrator |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Define information security strategy and objectives | A | C | R | C | C | C | I | C | C | I |
| 2 | Approve information security policies | A | C | R | C | C | C | I | C | C | I |
| 3 | Establish security governance framework | A | C | R | C | R | I | C | C | C | I |
| 4 | Allocate security budget and resources | A | R | C | C | I | C | I | I | C | I |
| 5 | Align security program with business objectives | A | C | R | C | C | C | I | C | R | I |
| 6 | Conduct enterprise risk assessment | A | C | R | R | C | C | I | C | I | I |
| 7 | Maintain risk register | C | C | R | A | C | C | I | C | C | I |
| 8 | Evaluate and prioritize risk treatment options | A | R | C | R | C | C | I | C | C | I |
| 9 | Develop risk mitigation plans | A | R | C | C | C | R | I | C | C | I |
| 10 | Report risk status to senior management | A | C | C | R | C | I | I | C | I | I |
| 11 | Monitor regulatory changes and updates | I | I | R | C | A | I | I | C | I | I |
| 12 | Conduct compliance gap analysis | C | C | R | C | A | C | I | C | C | I |
| 13 | Manage regulatory audit requests | C | R | R | I | A | C | I | C | I | I |
| 14 | Maintain compliance documentation | I | C | R | I | A | C | I | C | I | I |
| 15 | Track compliance metrics and KPIs | I | C | R | C | A | C | I | C | I | I |
| 16 | Draft and review security policies | A | R | R | C | C | C | I | C | C | I |
| 17 | Publish and distribute policy updates | C | I | R | I | A | I | I | I | I | I |
| 18 | Conduct security awareness training | A | R | C | I | C | I | I | C | C | I |
| 19 | Manage phishing simulation campaigns | C | A | R | I | I | C | I | C | I | R |
| 20 | Track training completion rates | A | C | R | I | C | I | I | I | C | I |
| 21 | Develop incident response procedures | A | R | C | C | C | R | I | C | I | C |
| 22 | Activate incident response team | A | R | R | C | C | R | I | C | I | R |
| 23 | Classify and escalate security incidents | C | A | I | I | C | R | I | C | I | R |
| 24 | Conduct root cause analysis post-incident | A | R | C | C | C | R | I | C | C | R |
| 25 | Produce incident reports for management | A | R | C | I | C | C | I | C | I | I |
| 26 | Manage vulnerability scanning program | I | A | I | I | I | C | I | I | I | R |
| 27 | Oversee penetration testing activities | A | R | C | C | C | C | I | C | C | C |
| 28 | Administer access control and IAM policies | A | R | C | C | C | R | I | C | C | R |
| 29 | Monitor security event logs and SIEM alerts | I | A | C | I | I | C | I | I | I | R |
| 30 | Manage security tool configurations | I | A | I | I | I | C | I | I | I | R |
| 31 | Plan annual internal audit schedule | C | I | R | C | C | I | A | I | I | I |
| 32 | Execute audit testing procedures | C | C | R | I | C | C | A | C | C | C |
| 33 | Document audit findings and recommendations | C | C | R | I | I | C | A | I | C | I |
| 34 | Track remediation of audit findings | A | R | R | I | C | R | C | I | R | I |
| 35 | Produce audit assurance reports | I | I | R | I | I | I | A | I | I | I |
| 36 | Conduct Data Protection Impact Assessments | I | I | R | C | C | I | I | A | C | I |
| 37 | Manage data classification program | R | C | R | C | C | C | I | A | R | I |
| 38 | Oversee data subject access requests | I | C | R | I | C | R | I | A | C | R |
| 39 | Ensure cross-border data transfer compliance | C | C | R | C | R | C | I | A | C | I |
| 40 | Assess third-party vendor security risks | A | R | C | C | C | C | I | C | C | I |
| 41 | Review vendor compliance certifications | C | C | R | I | A | I | I | C | I | I |
| 42 | Maintain vendor risk register | I | C | R | A | C | I | I | C | C | I |

## Role workload

| Role | A | R | C | I |
|---|---|---|---|---|
| CISO | 20 | 1 | 11 | 10 |
| IT Security Manager | 5 | 14 | 18 | 5 |
| GRC Analyst | 0 | 27 | 12 | 3 |
| Risk Manager | 2 | 3 | 20 | 17 |
| Compliance Officer | 7 | 2 | 26 | 7 |
| IT Operations Manager | 0 | 8 | 23 | 11 |
| Internal Auditor | 4 | 0 | 2 | 36 |
| Data Protection Officer | 4 | 0 | 28 | 10 |
| Business Unit Lead | 0 | 3 | 21 | 18 |
| System Administrator | 0 | 9 | 3 | 30 |

## Gaps and overlaps found

| # | Finding | Type | Why it matters | Suggested action |
|---|---|---|---|---|
| # | Finding | Type | Why it matters | Suggested action |
| 1 | Template has no column for Executive Leadership, the Board or a Risk Committee, so risk acceptance and policy approval cannot be assigned to the people with real authority. | Gap | The CISO shows as A for approvals that, in practice, are taken above the CISO. This is the likely source of the escalation delays the CISO describes. | Add an Executive Leadership / Risk Committee column, and move A for risk acceptance and policy approval to it. |
| 2 | The brief lists HR, Finance, Vendor Management, Product Teams, External Auditors and a Risk Committee. The template has no columns for them. | Gap | HR owns joiner/leaver and training records. Finance owns budget. Vendor Management owns contracts. Product Teams (NexusHealth Pro, NexusFinance Shield, PayStream) own most remediation. | Add these roles, or map them: Business Unit Lead stands in for Product Teams and Department Heads in this version. |
| 3 | The template has no activities for patch deployment, access termination, business continuity, DR testing or crisis communication, which the brief names. | Gap | These are exactly the areas where audit gaps and delays are likely, and none has an owner. | Add the missing activities in a second pass and assign them with the same rules. |
| 4 | Business Unit Lead is responsible for several items but accountable for none. | Gap | Business owners should own risk acceptance and remediation of risks in their products. Without an A, the CISO carries risks the business should own. | Give Business Unit Leads A for accepting risks within their delegated authority. |
| 5 | GRC Analyst has the highest number of R assignments. | Overlap / load | One analyst role cannot sustain this across risk, compliance, policy, audit support and privacy. It becomes a bottleneck. | Spread R to the Compliance Officer and Risk Manager, or add analyst capacity. |
| 6 | Several rows have two or more R assignments (for example incident activation and tooling). | Overlap | Shared R is fine when tasks are split, but it can blur who finishes the work. | Name a lead R in the procedure for each shared row. |
| 7 | GRC Analyst is R on audit rows, while Internal Auditor is A. The template checklist asks for this. | Independence risk | Audit conclusions must stay independent. GRC support is limited to scheduling, evidence preparation and compilation, not testing judgments. | State this limit in the audit procedure, and review it annually. |

## Justification of five critical decisions

### 1. #2 Approve information security policies

- **Decision:** CISO is Accountable. GRC Analyst is Responsible for the approval workflow and records. IT Security, Risk, Compliance, IT Operations, DPO and Business Unit Lead are Consulted. Internal Auditor and System Administrator are Informed.
- **Alternatives considered:** Compliance Officer as A (it owns document control). Business Unit Lead as A.
- **Rationale:** A policy needs one owner who answers for its content and for whether it works. The CISO owns the security program and its risk, so approval authority sits there. Compliance and the DPO are Consulted, not Accountable, so that legal advice informs the policy without deciding its security content. The Internal Auditor is only Informed to keep audit independence.
- **Risk if wrong, and safeguard:** Risk: policies that need Board-level sign-off are treated as the CISO's alone. Safeguard: add an Executive Leadership column (see Gap and Overlap Analysis, finding 1), so Tier-1 policies are approved there and the CISO stays accountable for the content.

### 2. #23 Classify and escalate security incidents

- **Decision:** IT Security Manager is Accountable. IT Operations Manager and System Administrator are Responsible. The CISO, Compliance Officer and DPO are Consulted.
- **Alternatives considered:** CISO as A (as for activating the response team, row 22). Compliance Officer as A.
- **Rationale:** Classification and escalation must happen in minutes. The IT Security Manager runs triage and has the facts, so decision rights belong there. Making the CISO Accountable for every classification creates the delay the CISO has seen. The CISO and DPO are Consulted so that serious incidents, and those involving regulated data such as PHI and card data, reach them early for notification decisions.
- **Risk if wrong, and safeguard:** Risk: an under-rated incident is not escalated. Safeguard: written severity criteria, a rule that any Severity 1 or 2 incident goes to the CISO immediately, and a post-incident check of classifications.

### 3. #31, #32, #33 and #35 Internal audit planning, testing, findings and reporting

- **Decision:** Internal Auditor is Accountable for these four audit activities. GRC Analyst is Responsible for scheduling, evidence preparation and compilation. The CISO and business roles are only Consulted or Informed. Follow-up on remediation (row 34) is treated separately, in decision 5.
- **Alternatives considered:** CISO or Compliance Officer as A. Internal Auditor as R with no A.
- **Rationale:** Internal audit must be independent of the functions it audits. If the CISO or Compliance Officer were Accountable, audit conclusions could be influenced by the people being audited. The template has no audit committee column, and each row needs a Responsible role, so the GRC Analyst handles support work while the Internal Auditor keeps ownership of conclusions.
- **Risk if wrong, and safeguard:** Risk: GRC support drifts into audit judgments. Safeguard: the audit procedure limits GRC to coordination and evidence handling, and findings are signed only by the Internal Auditor.

### 4. #36 to #39 Privacy activities (DPIA, data classification, DSAR, cross-border transfers)

- **Decision:** Data Protection Officer is Accountable. The GRC Analyst is Responsible for assessments and records. Business Unit Lead, IT Operations Manager and System Administrator are Responsible where data and systems are involved. The CISO is Responsible for classification and Consulted on the rest.
- **Alternatives considered:** CISO as A for classification and transfers. Compliance Officer as A for transfers.
- **Rationale:** The DPO has a legal duty to be independent and to advise on data protection. Accountability for DPIAs, subject requests and transfer decisions aligns with that role. NexusGuard operates in several countries (UAE, Saudi Arabia, Egypt) and handles PHI and cardholder data, so transfer and request decisions need one clear owner. Classification covers personal data first, and the CISO is Responsible for the security controls that follow.
- **Risk if wrong, and safeguard:** Risk: the DPO is asked to decide business uses, which compromises independence. Safeguard: the business owns the purpose of processing, and the DPO's accountability is for the privacy assessment and for the request and transfer process.

### 5. #34 Track remediation of audit findings

- **Decision:** CISO is Accountable. IT Security Manager, GRC Analyst, IT Operations Manager and Business Unit Lead are Responsible. The Internal Auditor is Consulted to verify closure.
- **Alternatives considered:** Internal Auditor as A. Compliance Officer as A.
- **Rationale:** Management, not audit, owns the fix. If the Internal Auditor were Accountable for remediation, it would be marking its own homework and lose independence. The CISO answers for security remediation, the GRC Analyst keeps the tracker, and the owners of the systems do the work. The Internal Auditor verifies closure.
- **Risk if wrong, and safeguard:** Risk: remediation owners in the business do not act. Safeguard: Business Unit Lead is Responsible with due dates, overdue items go to the Risk Committee, and the Internal Auditor re-tests closed findings.

_NexusGuard is a fictional company; this matrix is for portfolio use._
