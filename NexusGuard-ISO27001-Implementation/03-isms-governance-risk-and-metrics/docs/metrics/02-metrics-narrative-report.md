# NexusGuard Technologies Ltd. | Metrics Narrative Report | RPT-MET-001

| Field | Detail |
|---|---|
| **Report** | Metrics Narrative Report: baseline position and 12-month targets |
| **Document ID** | RPT-MET-001 (v1.0, draft) |
| **Prepared by** | Augustine Ozor, GRC Analyst, for the CISO |
| **Audience** | ISSC; Board of Directors at the next quarterly review |
| **Baseline date** | October 2026 (report date 13/10/2026) |

# 1. The Answer to the CEO's Question

The CEO asked how we will know whether the security program is working. Until now, NexusGuard measured nothing, so today we cannot show that it is. This report gives the first answer. Across the 26 metrics in the GRC KPI and Metrics Framework, **20 are Red, 4 Amber and 1 Green, and 1 cannot yet be measured**. That is what we should expect from a program that is only now getting approved policies, access controls, a risk register and an asset register. It is not yet working well enough, and the baseline shows where.

"Working" will mean this within 12 months: no open Critical risks and no active accounts of former staff; MFA on all privileged and remote access; Critical vulnerabilities fixed in 7 days; all eight Tier-1 policies approved and in date; ISO 27001 controls at 95% and the HIPAA and PCI DSS requirements fully in place; and incidents contained within 4 hours.

| Domain | Metrics | Green | Amber | Red | No data |
|---|---|---|---|---|---|
| Governance | 6 | 1 | 0 | 4 | 1 |
| Risk | 7 | 0 | 0 | 7 | 0 |
| Compliance | 6 | 0 | 2 | 4 | 0 |
| Operational | 7 | 0 | 2 | 5 | 0 |
| **Total** | **26** | **1** | **4** | **20** | **1** |

# 2. Governance: the Foundations Are Not Yet in Place

No policy under the new framework is in force yet: none of the eight required Tier-1 policies is approved, and the only existing policy, from January 2021, has never been reviewed. No one has signed the Acceptable Use Policy, and the committees are chartered but have not met. The asset register covers an estimated 58% of assets, with PayStream still largely to be discovered. One metric is Green: policy exceptions are decided quickly. Over 12 months we plan to approve all eight policies (four in the first three months), reach 100% acknowledgment of the Acceptable Use Policy, and cover 95% of assets.

| ID | Metric | Baseline | Status | 12-month target |
|---|---|---|---|---|
| G-01 | Policies reviewed on schedule | 0% (K) | Red | 100% |
| G-02 | Required Tier-1 policy set approved and in date | 0% (K) | Red | 100% |
| G-03 | Committee attendance (voting members) | No data | No data | 90% |
| G-04 | Exception requests decided within 10 business days | 100% (K) | Green | 95% |
| G-05 | Staff with a signed Acceptable Use Policy acknowledgment | 0% (K) | Red | 100% |
| G-06 | Information assets recorded with owner and classification | 58% (E) | Red | 95% |

# 3. Risk: Critical Exposure Is Concentrated in Access

Three Critical risks are open: excess privileged access, active accounts of former PayStream staff, and client data sent to a personal account. Forty-two privileged accounts have no current justification. There is no risk register, so no High or Critical risk yet has an approved treatment plan, and High risks take around 90 days to treat, based on how long the PayStream accounts stayed active. The aim is zero Critical risks and zero unjustified privileged accounts within six months, treatment plans on every High and Critical risk by month six, and a 30-day treatment time by month 12.

| ID | Metric | Baseline | Status | 12-month target |
|---|---|---|---|---|
| R-01 | Critical risks open | 3 (E) | Red | 0 |
| R-02 | High and Critical risks with an approved treatment plan | 0% (K) | Red | 100% |
| R-03 | Mean time to treat High risks | 90 days (E) | Red | 30 days |
| R-04 | High and Critical risks reviewed in the last 90 days | 0% (K) | Red | 100% |
| R-05 | Privileged accounts without current business justification | 42 (K) | Red | 0 |
| R-06 | Critical suppliers with a current security assessment | 0% (E) | Red | 100% |
| R-07 | Confirmed breaches of PHI, card or special category data | 1 (E) | Red | 0 |

# 4. Compliance: Certified, but the New Obligations Are Not Yet Met

ISO 27001 controls are estimated at about 78% implemented, which is Amber for a certified organization with gaps such as the missing asset register and classification scheme. HIPAA (60%) and PCI DSS (65%) are the most urgent, because the first HIPAA client is about to go live and the PayStream cardholder environment is not yet assessed. Only one of four known audit findings is closed, and there is no obligations register. Training completion is Amber at about 92%, but it is generic, not role-based. By month 12 the plan is ISO controls at 95%, HIPAA and PCI DSS at 100%, 90% of findings closed on time, and every obligation owned and evidenced.

| ID | Metric | Baseline | Status | 12-month target |
|---|---|---|---|---|
| C-01 | ISO 27001 Annex A controls implemented and evidenced | 78% (E) | Amber | 95% |
| C-02 | Audit and assessment finding closure rate | 25% (K) | Red | 90% |
| C-03 | Security awareness training completion | 92% (E) | Amber | 98% |
| C-04 | HIPAA Security Rule specifications implemented | 60% (E) | Red | 100% |
| C-05 | PCI DSS v4.0 requirements in place | 65% (E) | Red | 100% |
| C-06 | Compliance obligations with a named owner and evidence | 0% (K) | Red | 100% |

# 5. Operational: Controls Exist but Are Slow and Uneven

Eight former PayStream employees still have active accounts, no access reviews have been run, and only about half of serious incidents are triaged on time. Containing a Severity 1 incident takes about 16 hours against a 4-hour target, and MFA covers about 85% of privileged and remote access. Patching Critical vulnerabilities takes about 12 days, and availability is estimated at 99.6%. The plan is to remove all former-staff accounts at once, complete the first quarterly review within three months, reach 100% MFA and 7-day patching by month 12, and bring containment to 4 hours.

| ID | Metric | Baseline | Status | 12-month target |
|---|---|---|---|---|
| O-01 | Mean time to patch Critical vulnerabilities | 12 days (E) | Amber | 7 days |
| O-02 | MFA coverage for privileged and remote access | 85% (E) | Red | 100% |
| O-03 | Severity 1 and 2 incidents triaged within target | 50% (E) | Red | 100% |
| O-04 | Mean time to contain Severity 1 incidents | 16 hours (E) | Red | 4 hours |
| O-05 | Active accounts of former staff | 8 (K) | Red | 0 |
| O-06 | Scheduled access reviews completed on time | 0% (K) | Red | 100% |
| O-07 | Client-facing service availability (rolling 12 months) | 99.6% (E) | Amber | 99.9% |

# 6. How Much to Trust These Numbers

Of the 26 baselines, **11 are known** from the internal review, audits and documents, **14 are estimates** from CTO spreadsheets and judgment, and 1 has no baseline yet. Estimated baselines are marked (E) in the tables and will be validated against source data in the first cycle, so some values will move. The direction is unlikely to change: the Red items rest mainly on known facts such as the 42 privileged accounts and 8 former-staff accounts.

# 7. What We Ask of the ISSC and the Board

- **Approve** the framework, thresholds and the 12-month targets, and **note** the baseline.
- **Set a HIPAA go-live gate:** all required Security Rule specifications evidenced before the first client goes live, tracked as C-04.
- **Confirm owners** and require data by the 5th business day each month, and fund automated feeds for the Red metrics first.
- **Agree the Board set** of 8 metrics for the quarterly Board report (R-01, R-07, R-05, O-05, O-02, C-01, C-04, G-02).

_Figures are illustrative scenario data for portfolio use. Full definitions are in the GRC KPI and Metrics Framework (FWK-GRC-001) and the live dashboard in NexusGuard_GRC_KPI_Dashboard.xlsx._
