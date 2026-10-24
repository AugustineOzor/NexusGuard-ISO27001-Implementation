# NexusGuard Technologies Ltd. | GRC KPI and Metrics Framework | FWK-GRC-001

| Field | Detail |
|---|---|
| **Document Title** | GRC KPI and Metrics Framework |
| **Document ID** | FWK-GRC-001 |
| **Version** | 1.0 |
| **Classification** | Internal |
| **Author** | Augustine Ozor, GRC Analyst |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Information Security Steering Committee (approval pending), then presented to the Board |
| **Approval Date** | Pending (DD/MM/YYYY to be entered on approval) |
| **Effective Date** | Upon approval |
| **Next Review Date** | 12 months from approval date |
| **Applicable Regulations** | ISO/IEC 27001:2022 (Clauses 6.2, 9.1), HIPAA, PCI DSS v4.0, GDPR / UK GDPR, NIST CSF 2.0 (GV.OV), UAE NESA |

# Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 0.1 | 13/10/2026 | Augustine Ozor, GRC Analyst | Initial draft, requested by James Richardson after the CEO asked the ISSC how the security program will be shown to work. Prepared for the next quarterly Board review in six weeks. |
| 1.0 | Pending | Information Security Steering Committee | Approval and publication. |

# 1. Purpose

At the ISSC, the CEO, Sarah Al-Mansouri, asked: "How will we know if our security program is actually working?" NexusGuard Technologies Ltd. ("NexusGuard") has had no security metrics: no KPIs, no key risk indicators (KRIs) and no dashboards. This framework answers the question by defining what "working" means, how it is measured, who is accountable, and how it is reported.

It defines 26 metrics across the four GRC domains (Governance, Risk, Compliance and Operational). For each metric it sets a name, formula, data source, frequency, target, red/amber/green (RAG) thresholds and owner. It also sets the baseline at October 2026 and the targets for the next 12 months. The companion Excel workbook (NexusGuard_GRC_KPI_Dashboard.xlsx) holds the live dashboard, and the Metrics Narrative Report presents the baseline to the ISSC and the Board.

# 2. Scope and Audience

The framework covers information security governance, risk, compliance and operations at NexusGuard in Dubai, London and New York, and at PayStream Analytics. It supports ISO/IEC 27001:2022 Clause 9.1 (monitoring and measurement), the objectives in Table 1 of the Information Security Policy, and the HIPAA, PCI DSS and GDPR obligations that clients will ask NexusGuard to evidence.

| Audience | What they need | How they receive it |
|---|---|---|
| Board of Directors | A short view of the metrics that show whether the program is working, and what is off track | Quarterly Board Security Report: 8 headline metrics |
| ISSC | All metrics, trends and the actions needed to fix Red items | Monthly ISSC Report: full dashboard |
| Risk and Compliance Committees | The risk and compliance metrics they own | Quarterly committee packs |
| Metric owners | Clear definitions, thresholds and deadlines | This framework and the dashboard |
| Auditors and clients | Evidence that NexusGuard measures and acts on its controls | Dashboard, reports and records on request |

# 3. Design Principles

- **Answer a decision.** Every metric helps someone decide something. Metrics that nobody would act on are left out.
- **Outcomes as well as activity.** The set mixes outcome measures (breaches, availability, exposure) with activity measures (reviews done, training completed), and leading indicators with lagging ones.
- **Few and meaningful.** The framework has 26 metrics, not 200, so that each one can be understood, owned and challenged.
- **One owner each.** Every metric has a named accountable owner and a data source of record.
- **Evidence, not opinion.** Values come from systems and records, are repeatable, and can be re-checked by an auditor.
- **Baselined and targeted.** Each metric has a starting value, a target, and a glide path to it, so progress is visible.
- **Honest about data quality.** Estimated baselines are labeled as estimates and validated in the first cycle.

# 4. Framework Overview

The framework has four domains. Each answers one question about the security program.

**Table 1: The Four GRC Domains**

| Domain | Question it answers | Metrics | Mainly reviewed by |
|---|---|---|---|
| Governance | Are we directing and controlling security properly? | 6 | ISSC |
| Risk | Do we know our exposure and are we treating it? | 7 | Risk Committee |
| Compliance | Can we prove we meet our obligations? | 6 | Compliance Committee |
| Operational | Are controls working day to day? | 7 | ISSC |

**4.1** A **KPI** (key performance indicator) measures how well a process or control performs against a target. A **KRI** (key risk indicator) measures exposure and warns of rising risk. Each metric is labeled KPI or KRI in Section 6.

**4.2** Each metric links to one of the ten security objectives (O1 to O10) in Table 1 of the Information Security Policy, so that results show whether those objectives are being met (Table 2).

**Table 2: Metrics by Information Security Policy Objective**

| Objective | Summary | Metrics |
|---|---|---|
| O1 | Protect confidentiality of regulated data | G-06, R-01, R-07 |
| O2 | Maintain availability of client-facing services | O-07 |
| O4 | Achieve and sustain compliance | C-01, C-02, C-04, C-05, C-06 |
| O5 | Reduce exposure to vulnerabilities | R-03, O-01 |
| O6 | Control access rigorously | R-05, O-02, O-05, O-06 |
| O7 | Build a security-aware workforce | G-05, C-03 |
| O8 | Respond effectively to incidents | O-03, O-04 |
| O9 | Manage third-party risk | R-06 |
| O10 | Keep the ISMS current | G-01, G-02, G-03, G-04, R-02, R-04 |

_O3 (integrity of systems and data) is measured through change management and the integrity of the asset register, and is not yet a separate metric. The ISSC should consider adding a change success metric at the first annual review._

# 5. Measurement Standards

## 5.1 RAG Status

**5.1.1** Every metric has a Green threshold and an Amber threshold. Where higher is better, a value at or above the Green threshold is Green, at or above the Amber threshold is Amber, and below it is Red. Where lower is better the tests are reversed.

**5.1.2** Green means the objective is being met. Amber means the metric is close and recovering, and needs watching. Red means the metric is outside tolerance and needs a corrective action with an owner and date.

**5.1.3** A metric with no value is shown as No data and is treated as an issue to resolve. It shall not be left blank or shown as Green.

## 5.2 Trend

**5.2.1** Trend compares the latest value with the previous one and takes account of direction. A falling count of open Critical risks is Improving. The first reading is shown as Baseline.

## 5.3 Baselines

**5.3.1** Each metric records the basis of its baseline: **K** known from reviews, audits or documents (11 metrics); **E** estimated from CTO spreadsheets or professional judgment (14 metrics); or no baseline yet (1 metric).

**5.3.2** Estimated baselines shall be validated against source data in the first measurement cycle. The baseline may be restated once after validation, with the change recorded, and shall then be frozen.

## 5.4 Data Quality

**5.4.1** Each metric draws on a named system of record. The owner shall supply the value and attest that it is complete. The GRC Analyst shall reconcile it to the source report before it is published.

**5.4.2** Changes to a definition, formula or threshold shall be approved by the ISSC, recorded in the version history, and applied from the next period, with prior periods restated where practical.

**5.4.3** Manual overrides are not allowed unless the owner records the reason, and the GRC Analyst notes it in the report. Source extracts shall be retained for six years.

## 5.5 Frequency and Calendar

**5.5.1** Monthly metrics shall be supplied by the 5th business day of the month. Quarterly metrics shall be measured in the month after quarter-end. The Monthly ISSC Report shall be issued 3 business days before the ISSC meeting, and the Quarterly Board Security Report before each Board meeting.

## 5.6 Escalation

**Table 3: Escalation Rules**

| Trigger | Action | Escalate to |
|---|---|---|
| A metric is Red for two consecutive periods | Owner presents a corrective action plan with dates | ISSC |
| A KRI marked in Section 6 as Critical-exposure (R-01, R-05, R-07, O-05) is Red | Owner explains cause and fix within 2 business days | CEO and ISSC Chair |
| Data is not supplied by the deadline | Metric shows No data; owner told on day 1 | Owner's executive after 5 business days |
| Value falls below target after being Green | Owner explains the cause at the next ISSC | ISSC |
| A metric is Red for four consecutive periods | Reassess target, resourcing or definition | Risk Committee and Board |

# 6. Metric Definitions

The tables below define all 26 metrics. Percentages use the formula shown. Targets are the 12-month targets from the October 2026 baseline. Thresholds are the same ones the dashboard applies.

## 6.1 Governance Metrics

| Metric | Formula and data source | Frequency | 12-month target | RAG thresholds |
|---|---|---|---|---|
| **G-01** Policies reviewed on schedule<br>KPI, higher is better<br>Owner: Head of Compliance (Michael Chen) | (Policies reviewed by due date / Policies due for review in the period) x 100<br>Source: Document register (policy repository) | Quarterly | 100% | Green 95% or more; Amber 85% or more; Red below 85% |
| **G-02** Required Tier-1 policy set approved and in date<br>KPI, higher is better<br>Owner: CISO | (Approved, in-date Tier-1 policies / 8 required) x 100<br>Source: Document register | Quarterly | 100% | Green 100% or more; Amber 75% or more; Red below 75% |
| **G-03** Committee attendance (voting members)<br>KPI, higher is better<br>Owner: Committee Secretary (GRC Analyst), for the Chairs | (Voting member attendances / Expected attendances across the three committees) x 100<br>Source: Committee minutes and attendance register | Quarterly | 90% | Green 85% or more; Amber 75% or more; Red below 75% |
| **G-04** Exception requests decided within 10 business days<br>KPI, higher is better<br>Owner: CISO | (Exception requests decided within 10 business days / Requests received in the period) x 100<br>Source: Exception register and ITSM | Monthly | 95% | Green 95% or more; Amber 85% or more; Red below 85% |
| **G-05** Staff with a signed Acceptable Use Policy acknowledgment<br>KPI, higher is better<br>Owner: HR Director (Aisha Patel) | (Staff and contractors with a signed current AUP / Total staff and contractors) x 100<br>Source: HR system and LMS | Monthly | 100% | Green 98% or more; Amber 90% or more; Red below 90% |
| **G-06** Information assets recorded with owner and classification<br>KPI, higher is better<br>Owner: CISO, with the Head of IT | (Assets in the IAR with owner and classification / Estimated total asset population) x 100<br>Source: Information Asset Register, discovery scans and CMDB | Quarterly | 95% | Green 95% or more; Amber 80% or more; Red below 80% |

## 6.2 Risk Metrics

| Metric | Formula and data source | Frequency | 12-month target | RAG thresholds |
|---|---|---|---|---|
| **R-01** Critical risks open<br>KRI, lower is better<br>Owner: CISO (Risk Committee Chair accountable) | Count of open risks rated Critical in the risk register at period end<br>Source: Risk register | Monthly | 0 | Green 0 or less; Amber 2 or less; Red above 2 |
| **R-02** High and Critical risks with an approved treatment plan<br>KPI, higher is better<br>Owner: CISO | (High and Critical risks with an approved plan / All open High and Critical risks) x 100<br>Source: Risk register | Monthly | 100% | Green 100% or more; Amber 85% or more; Red below 85% |
| **R-03** Mean time to treat High risks<br>KPI, lower is better<br>Owner: CISO | Average of (treatment completed or accepted date minus date rated High) for High risks closed in the period<br>Source: Risk register and ITSM | Quarterly | 30 days | Green 30 days or less; Amber 60 days or less; Red above 60 days |
| **R-04** High and Critical risks reviewed in the last 90 days<br>KPI, higher is better<br>Owner: CISO | (High and Critical risks reviewed within 90 days / All open High and Critical risks) x 100<br>Source: Risk register | Quarterly | 100% | Green 95% or more; Amber 80% or more; Red below 80% |
| **R-05** Privileged accounts without current business justification<br>KRI, lower is better<br>Owner: Head of IT | Count of privileged accounts with no current justification at period end, from the privileged access register and quarterly review<br>Source: IAM and PAM reports; access review records | Monthly | 0 | Green 0 or less; Amber 5 or less; Red above 5 |
| **R-06** Critical suppliers with a current security assessment<br>KPI, higher is better<br>Owner: CISO, with the Procurement Lead | (Critical suppliers assessed in the last 12 months / Critical suppliers) x 100<br>Source: Third-party register | Quarterly | 100% | Green 95% or more; Amber 80% or more; Red below 80% |
| **R-07** Confirmed breaches of PHI, card or special category data<br>KRI, lower is better<br>Owner: CISO | Count of confirmed breaches of regulated data in the period, from the incident register<br>Source: Incident register (ITSM) and DPO breach log | Monthly | 0 | Green 0 or less; Amber 0 or less; Red above 0 |

## 6.3 Compliance Metrics

| Metric | Formula and data source | Frequency | 12-month target | RAG thresholds |
|---|---|---|---|---|
| **C-01** ISO 27001 Annex A controls implemented and evidenced<br>KPI, higher is better<br>Owner: Head of Compliance (Michael Chen) | (Applicable Annex A controls implemented with evidence / Applicable controls in the SoA) x 100<br>Source: Statement of Applicability and control testing | Quarterly | 95% | Green 90% or more; Amber 75% or more; Red below 75% |
| **C-02** Audit and assessment finding closure rate<br>KPI, higher is better<br>Owner: Head of Compliance (Michael Chen) | (Findings closed by due date / Findings due in the period) x 100<br>Source: Findings register | Monthly | 90% | Green 90% or more; Amber 75% or more; Red below 75% |
| **C-03** Security awareness training completion<br>KPI, higher is better<br>Owner: HR Director (Aisha Patel) | (Staff completing assigned annual training / Staff assigned) x 100<br>Source: Learning management system | Monthly | 98% | Green 98% or more; Amber 90% or more; Red below 90% |
| **C-04** HIPAA Security Rule specifications implemented<br>KPI, higher is better<br>Owner: CISO | (Specifications implemented and evidenced / Applicable specifications) x 100<br>Source: HIPAA risk analysis and control assessment | Quarterly | 100% | Green 95% or more; Amber 85% or more; Red below 85% |
| **C-05** PCI DSS v4.0 requirements in place<br>KPI, higher is better<br>Owner: CISO | (Applicable requirements in place / Applicable requirements) x 100<br>Source: PCI gap assessment and SAQ or ROC evidence | Quarterly | 100% | Green 98% or more; Amber 90% or more; Red below 90% |
| **C-06** Compliance obligations with a named owner and evidence<br>KPI, higher is better<br>Owner: Head of Compliance (Michael Chen) | (Obligations with owner and current evidence / Obligations in the register) x 100<br>Source: Compliance obligations register | Quarterly | 100% | Green 95% or more; Amber 80% or more; Red below 80% |

## 6.4 Operational Metrics

| Metric | Formula and data source | Frequency | 12-month target | RAG thresholds |
|---|---|---|---|---|
| **O-01** Mean time to patch Critical vulnerabilities<br>KPI, lower is better<br>Owner: Head of IT | Average of (remediation date minus detection date) for Critical vulnerabilities closed in the period<br>Source: Vulnerability scanner and ITSM | Monthly | 7 days | Green 7 days or less; Amber 14 days or less; Red above 14 days |
| **O-02** MFA coverage for privileged and remote access<br>KPI, higher is better<br>Owner: CISO | (Privileged and remote-access accounts protected by MFA / All such accounts) x 100<br>Source: Entra ID, PAM and VPN or ZTNA reports | Monthly | 100% | Green 99% or more; Amber 90% or more; Red below 90% |
| **O-03** Severity 1 and 2 incidents triaged within target<br>KPI, higher is better<br>Owner: Security Operations Center Manager | (Severity 1 triaged in 1 hour and Severity 2 in 2 hours / Severity 1 and 2 incidents) x 100<br>Source: ITSM and SIEM incident records | Monthly | 100% | Green 95% or more; Amber 80% or more; Red below 80% |
| **O-04** Mean time to contain Severity 1 incidents<br>KPI, lower is better<br>Owner: Security Operations Center Manager | Average of (containment time minus declaration time) for Severity 1 incidents closed in the period<br>Source: ITSM incident records | Monthly | 4 hours | Green 4 hours or less; Amber 8 hours or less; Red above 8 hours |
| **O-05** Active accounts of former staff<br>KRI, lower is better<br>Owner: Head of IT (IAM) | Count of enabled accounts with no current HR or contractor record at month end, across all identity stores<br>Source: IAM reconciliation (AD, Entra ID, AWS IAM, SaaS, PayStream directories) | Monthly | 0 | Green 0 or less; Amber 2 or less; Red above 2 |
| **O-06** Scheduled access reviews completed on time<br>KPI, higher is better<br>Owner: CISO | (Reviews completed within 15 business days / Reviews due) x 100<br>Source: IAM access review reports | Quarterly | 100% | Green 95% or more; Amber 80% or more; Red below 80% |
| **O-07** Client-facing service availability (rolling 12 months)<br>KPI, higher is better<br>Owner: Head of IT | ((Total service minutes - Unplanned downtime minutes) / Total service minutes) x 100<br>Source: Monitoring platform (Datadog) and incident records | Monthly | 99.9% | Green 99.9% or more; Amber 99.5% or more; Red below 99.5% |

# 7. Baseline and 12-Month Targets

The table shows each metric's baseline at October 2026 and its planned targets at 3, 6 and 12 months. Of 26 metrics, 20 are Red, 4 Amber and 1 Green at baseline, and 1 has no data yet. Baseline basis: K known; E estimate to validate.

**Table 4: Baseline and Targets**

| ID | Metric | Baseline | Status | 3 months | 6 months | 12 months |
|---|---|---|---|---|---|---|
| G-01 | Policies reviewed on schedule | 0% (K) | Red | 80% | 95% | 100% |
| G-02 | Required Tier-1 policy set approved and in date | 0% (K) | Red | 50% | 75% | 100% |
| G-03 | Committee attendance (voting members) | No data | No data | 85% | 88% | 90% |
| G-04 | Exception requests decided within 10 business days | 100% (K) | Green | 95% | 95% | 95% |
| G-05 | Staff with a signed Acceptable Use Policy acknowledgment | 0% (K) | Red | 90% | 98% | 100% |
| G-06 | Information assets recorded with owner and classification | 58% (E) | Red | 75% | 90% | 95% |
| R-01 | Critical risks open | 3 (E) | Red | 1 | 0 | 0 |
| R-02 | High and Critical risks with an approved treatment plan | 0% (K) | Red | 80% | 100% | 100% |
| R-03 | Mean time to treat High risks | 90 days (E) | Red | 75 days | 60 days | 30 days |
| R-04 | High and Critical risks reviewed in the last 90 days | 0% (K) | Red | 80% | 95% | 100% |
| R-05 | Privileged accounts without current business justification | 42 (K) | Red | 5 | 0 | 0 |
| R-06 | Critical suppliers with a current security assessment | 0% (E) | Red | 40% | 75% | 100% |
| R-07 | Confirmed breaches of PHI, card or special category data | 1 (E) | Red | 0 | 0 | 0 |
| C-01 | ISO 27001 Annex A controls implemented and evidenced | 78% (E) | Amber | 82% | 88% | 95% |
| C-02 | Audit and assessment finding closure rate | 25% (K) | Red | 60% | 80% | 90% |
| C-03 | Security awareness training completion | 92% (E) | Amber | 95% | 97% | 98% |
| C-04 | HIPAA Security Rule specifications implemented | 60% (E) | Red | 90% | 97% | 100% |
| C-05 | PCI DSS v4.0 requirements in place | 65% (E) | Red | 75% | 90% | 100% |
| C-06 | Compliance obligations with a named owner and evidence | 0% (K) | Red | 70% | 90% | 100% |
| O-01 | Mean time to patch Critical vulnerabilities | 12 days (E) | Amber | 10 days | 8 days | 7 days |
| O-02 | MFA coverage for privileged and remote access | 85% (E) | Red | 95% | 99% | 100% |
| O-03 | Severity 1 and 2 incidents triaged within target | 50% (E) | Red | 70% | 85% | 100% |
| O-04 | Mean time to contain Severity 1 incidents | 16 hours (E) | Red | 12 hours | 8 hours | 4 hours |
| O-05 | Active accounts of former staff | 8 (K) | Red | 0 | 0 | 0 |
| O-06 | Scheduled access reviews completed on time | 0% (K) | Red | 80% | 95% | 100% |
| O-07 | Client-facing service availability (rolling 12 months) | 99.6% (E) | Amber | 99.7% | 99.8% | 99.9% |

# 8. Data Sources and Collection

**Table 5: Systems of Record**

| Source | Owner | Feeds |
|---|---|---|
| Document register (policy repository) | Head of Compliance | G-01, G-02 |
| HR system and learning management system | HR Director | G-05, C-03 |
| Committee minutes and attendance register | Committee Secretary | G-03 |
| Exception register and ITSM | CISO | G-04, R-03 |
| Information Asset Register, discovery scans | CISO and Head of IT | G-06 |
| Risk register | CISO | R-01, R-02, R-03, R-04 |
| IAM and PAM reports, Entra ID, VPN and ZTNA, reconciliation | Head of IT (IAM) | R-05, O-02, O-05, O-06 |
| Third-party register | CISO and Procurement Lead | R-06 |
| Incident register and SIEM | Security Operations Center Manager | R-07, O-03, O-04 |
| Statement of Applicability, HIPAA and PCI assessments | Head of Compliance and CISO | C-01, C-04, C-05 |
| Findings register and obligations register | Head of Compliance | C-02, C-06 |
| Vulnerability scanner | Head of IT | O-01 |
| Monitoring platform | Head of IT | O-07 |

**8.1** Where a source system cannot yet produce a metric automatically, the owner shall supply it by a documented manual extract, and IT shall plan to automate it. Automation priority goes to the metrics that are Red and the Board set.

# 9. Reporting and Governance

**9.1** The ISSC shall review all 26 metrics monthly through the Monthly ISSC Report. The Risk Committee shall review the Risk metrics (R-01 to R-07) quarterly, and the Compliance Committee the Compliance metrics (C-01 to C-06) at each meeting.

**9.2** The Board shall receive a headline set of 8 metrics in the Quarterly Board Security Report: Critical risks open; Confirmed breaches of PHI, card or special category data; Privileged accounts without current business justification; Active accounts of former staff; MFA coverage for privileged and remote access; ISO 27001 Annex A controls implemented and evidenced; HIPAA Security Rule specifications implemented; Required Tier-1 policy set approved and in date.

**9.3** The CISO shall present the report, and the Chair of the relevant committee shall answer for the Risk and Compliance metrics. The report shall say what is Red, why, and what is being done.

**9.4** The KPI rows in the Monthly ISSC Report Template (TPL-ISSC-001) and the Quarterly Board Security Report Template (TPL-BRD-001) shall be aligned to the metric IDs in this framework before first use.

# 10. Roles and Responsibilities

| Role | Responsibilities |
|---|---|
| ISSC | Approves the framework, thresholds and targets; reviews all metrics monthly; acts on Red items. |
| Risk Committee and Compliance Committee | Review the Risk and Compliance metrics; challenge targets and treatment. |
| CISO | Owns the framework; accountable for the dashboard and reports; presents to the Board. |
| Metric owners | Supply values on time, attest to accuracy, explain Red items and deliver corrective actions. |
| GRC Analyst | Maintains the dashboard and definitions, reconciles data to sources, and issues the reports. |
| IT and Security Operations | Provide system extracts and automate data feeds. |
| Internal Audit | Tests the accuracy of reported metrics at least annually. |

# 11. Implementation Plan (six weeks to the Board review)

| Week | Activity | Owner | Output |
|---|---|---|---|
| 1 | Approve the framework, owners and thresholds at the ISSC | CISO; ISSC | Approved framework |
| 2 | Confirm data sources and extract methods with each owner | GRC Analyst; owners | Source map and data owners confirmed |
| 3 | Validate the estimated (E) baselines against source data | Owners; GRC Analyst | Validated baselines |
| 4 | Load validated data into the dashboard; fix gaps | GRC Analyst | Live dashboard |
| 5 | Dry run the Monthly ISSC Report; align the report templates | CISO; GRC Analyst | First ISSC report |
| 6 | Prepare and review the Quarterly Board Security Report | CISO; CEO | Board pack |

# 12. Review and Maintenance

**12.1** The ISSC shall review this framework after the first two quarters, to retire metrics that are not used and recalibrate thresholds that prove too easy or too hard, and then every 12 months.

**12.2** Metrics may be added or retired with ISSC approval. Each change shall be recorded in the version history and in the dashboard definitions sheet.

# 13. Related Documents

| Document | ID |
|---|---|
| Information Security Policy (objectives in Table 1) | POL-ISP-001 |
| Access Control Policy | POL-ACC-001 |
| Data Classification and Handling Policy | POL-DCH-001 |
| ISSC, Risk Committee and Compliance Committee Charters | CHR-ISSC-001, CHR-RSK-001, CHR-CMP-001 |
| Monthly ISSC Report Template | TPL-ISSC-001 |
| Quarterly Board Security Report Template | TPL-BRD-001 |
| KPI Dashboard workbook | NexusGuard_GRC_KPI_Dashboard.xlsx |
| Metrics Narrative Report | RPT-MET-001 |
