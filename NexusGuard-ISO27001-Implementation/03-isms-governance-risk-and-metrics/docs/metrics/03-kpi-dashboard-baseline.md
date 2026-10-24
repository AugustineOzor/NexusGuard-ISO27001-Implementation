# NexusGuard GRC KPI Dashboard (baseline, October 2026)

This is the Markdown view of the Excel dashboard (`NexusGuard_GRC_KPI_Dashboard.xlsx`). RAG status is calculated from the baseline value and the thresholds shown. Baseline basis: K known; E estimate to validate in the first cycle. Trend shows **Baseline** until a second month of data is entered.

## Summary

| Domain | Green | Amber | Red | No data | Total |
|---|---|---|---|---|---|
| Governance | 1 | 0 | 4 | 1 | 6 |
| Risk | 0 | 0 | 7 | 0 | 7 |
| Compliance | 0 | 2 | 4 | 0 | 6 |
| Operational | 0 | 2 | 5 | 0 | 7 |
| **Total** | **1** | **4** | **20** | **1** | **26** |

## Governance metrics

| ID | Metric | Type | Baseline | Status | Trend | 12-month target | Thresholds | Owner | Frequency |
|---|---|---|---|---|---|---|---|---|---|
| G-01 | Policies reviewed on schedule | KPI | 0% (K) | Red | Baseline | 100% | Green 95% or more; Amber 85% or more; Red below 85% | Head of Compliance (Michael Chen) | Quarterly |
| G-02 | Required Tier-1 policy set approved and in date | KPI | 0% (K) | Red | Baseline | 100% | Green 100% or more; Amber 75% or more; Red below 75% | CISO | Quarterly |
| G-03 | Committee attendance (voting members) | KPI | No data | No data | No data | 90% | Green 85% or more; Amber 75% or more; Red below 75% | Committee Secretary (GRC Analyst), for the Chairs | Quarterly |
| G-04 | Exception requests decided within 10 business days | KPI | 100% (K) | Green | Baseline | 95% | Green 95% or more; Amber 85% or more; Red below 85% | CISO | Monthly |
| G-05 | Staff with a signed Acceptable Use Policy acknowledgment | KPI | 0% (K) | Red | Baseline | 100% | Green 98% or more; Amber 90% or more; Red below 90% | HR Director (Aisha Patel) | Monthly |
| G-06 | Information assets recorded with owner and classification | KPI | 58% (E) | Red | Baseline | 95% | Green 95% or more; Amber 80% or more; Red below 80% | CISO, with the Head of IT | Quarterly |

## Risk metrics

| ID | Metric | Type | Baseline | Status | Trend | 12-month target | Thresholds | Owner | Frequency |
|---|---|---|---|---|---|---|---|---|---|
| R-01 | Critical risks open | KRI | 3 (E) | Red | Baseline | 0 | Green 0 or less; Amber 2 or less; Red above 2 | CISO (Risk Committee Chair accountable) | Monthly |
| R-02 | High and Critical risks with an approved treatment plan | KPI | 0% (K) | Red | Baseline | 100% | Green 100% or more; Amber 85% or more; Red below 85% | CISO | Monthly |
| R-03 | Mean time to treat High risks | KPI | 90 days (E) | Red | Baseline | 30 days | Green 30 days or less; Amber 60 days or less; Red above 60 days | CISO | Quarterly |
| R-04 | High and Critical risks reviewed in the last 90 days | KPI | 0% (K) | Red | Baseline | 100% | Green 95% or more; Amber 80% or more; Red below 80% | CISO | Quarterly |
| R-05 | Privileged accounts without current business justification | KRI | 42 (K) | Red | Baseline | 0 | Green 0 or less; Amber 5 or less; Red above 5 | Head of IT | Monthly |
| R-06 | Critical suppliers with a current security assessment | KPI | 0% (E) | Red | Baseline | 100% | Green 95% or more; Amber 80% or more; Red below 80% | CISO, with the Procurement Lead | Quarterly |
| R-07 | Confirmed breaches of PHI, card or special category data | KRI | 1 (E) | Red | Baseline | 0 | Green 0 or less; Amber 0 or less; Red above 0 | CISO | Monthly |

## Compliance metrics

| ID | Metric | Type | Baseline | Status | Trend | 12-month target | Thresholds | Owner | Frequency |
|---|---|---|---|---|---|---|---|---|---|
| C-01 | ISO 27001 Annex A controls implemented and evidenced | KPI | 78% (E) | Amber | Baseline | 95% | Green 90% or more; Amber 75% or more; Red below 75% | Head of Compliance (Michael Chen) | Quarterly |
| C-02 | Audit and assessment finding closure rate | KPI | 25% (K) | Red | Baseline | 90% | Green 90% or more; Amber 75% or more; Red below 75% | Head of Compliance (Michael Chen) | Monthly |
| C-03 | Security awareness training completion | KPI | 92% (E) | Amber | Baseline | 98% | Green 98% or more; Amber 90% or more; Red below 90% | HR Director (Aisha Patel) | Monthly |
| C-04 | HIPAA Security Rule specifications implemented | KPI | 60% (E) | Red | Baseline | 100% | Green 95% or more; Amber 85% or more; Red below 85% | CISO | Quarterly |
| C-05 | PCI DSS v4.0 requirements in place | KPI | 65% (E) | Red | Baseline | 100% | Green 98% or more; Amber 90% or more; Red below 90% | CISO | Quarterly |
| C-06 | Compliance obligations with a named owner and evidence | KPI | 0% (K) | Red | Baseline | 100% | Green 95% or more; Amber 80% or more; Red below 80% | Head of Compliance (Michael Chen) | Quarterly |

## Operational metrics

| ID | Metric | Type | Baseline | Status | Trend | 12-month target | Thresholds | Owner | Frequency |
|---|---|---|---|---|---|---|---|---|---|
| O-01 | Mean time to patch Critical vulnerabilities | KPI | 12 days (E) | Amber | Baseline | 7 days | Green 7 days or less; Amber 14 days or less; Red above 14 days | Head of IT | Monthly |
| O-02 | MFA coverage for privileged and remote access | KPI | 85% (E) | Red | Baseline | 100% | Green 99% or more; Amber 90% or more; Red below 90% | CISO | Monthly |
| O-03 | Severity 1 and 2 incidents triaged within target | KPI | 50% (E) | Red | Baseline | 100% | Green 95% or more; Amber 80% or more; Red below 80% | Security Operations Center Manager | Monthly |
| O-04 | Mean time to contain Severity 1 incidents | KPI | 16 hours (E) | Red | Baseline | 4 hours | Green 4 hours or less; Amber 8 hours or less; Red above 8 hours | Security Operations Center Manager | Monthly |
| O-05 | Active accounts of former staff | KRI | 8 (K) | Red | Baseline | 0 | Green 0 or less; Amber 2 or less; Red above 2 | Head of IT (IAM) | Monthly |
| O-06 | Scheduled access reviews completed on time | KPI | 0% (K) | Red | Baseline | 100% | Green 95% or more; Amber 80% or more; Red below 80% | CISO | Quarterly |
| O-07 | Client-facing service availability (rolling 12 months) | KPI | 99.6% (E) | Amber | Baseline | 99.9% | Green 99.9% or more; Amber 99.5% or more; Red below 99.5% | Head of IT | Monthly |

## 12-month glide path

| ID | Metric | Baseline | 3 months (Jan-27) | 6 months (Apr-27) | 12 months (Oct-27) |
|---|---|---|---|---|---|
| G-01 | Policies reviewed on schedule | 0% (K) | 80% | 95% | 100% |
| G-02 | Required Tier-1 policy set approved and in date | 0% (K) | 50% | 75% | 100% |
| G-03 | Committee attendance (voting members) | No data | 85% | 88% | 90% |
| G-04 | Exception requests decided within 10 business days | 100% (K) | 95% | 95% | 95% |
| G-05 | Staff with a signed Acceptable Use Policy acknowledgment | 0% (K) | 90% | 98% | 100% |
| G-06 | Information assets recorded with owner and classification | 58% (E) | 75% | 90% | 95% |
| R-01 | Critical risks open | 3 (E) | 1 | 0 | 0 |
| R-02 | High and Critical risks with an approved treatment plan | 0% (K) | 80% | 100% | 100% |
| R-03 | Mean time to treat High risks | 90 days (E) | 75 days | 60 days | 30 days |
| R-04 | High and Critical risks reviewed in the last 90 days | 0% (K) | 80% | 95% | 100% |
| R-05 | Privileged accounts without current business justification | 42 (K) | 5 | 0 | 0 |
| R-06 | Critical suppliers with a current security assessment | 0% (E) | 40% | 75% | 100% |
| R-07 | Confirmed breaches of PHI, card or special category data | 1 (E) | 0 | 0 | 0 |
| C-01 | ISO 27001 Annex A controls implemented and evidenced | 78% (E) | 82% | 88% | 95% |
| C-02 | Audit and assessment finding closure rate | 25% (K) | 60% | 80% | 90% |
| C-03 | Security awareness training completion | 92% (E) | 95% | 97% | 98% |
| C-04 | HIPAA Security Rule specifications implemented | 60% (E) | 90% | 97% | 100% |
| C-05 | PCI DSS v4.0 requirements in place | 65% (E) | 75% | 90% | 100% |
| C-06 | Compliance obligations with a named owner and evidence | 0% (K) | 70% | 90% | 100% |
| O-01 | Mean time to patch Critical vulnerabilities | 12 days (E) | 10 days | 8 days | 7 days |
| O-02 | MFA coverage for privileged and remote access | 85% (E) | 95% | 99% | 100% |
| O-03 | Severity 1 and 2 incidents triaged within target | 50% (E) | 70% | 85% | 100% |
| O-04 | Mean time to contain Severity 1 incidents | 16 hours (E) | 12 hours | 8 hours | 4 hours |
| O-05 | Active accounts of former staff | 8 (K) | 0 | 0 | 0 |
| O-06 | Scheduled access reviews completed on time | 0% (K) | 80% | 95% | 100% |
| O-07 | Client-facing service availability (rolling 12 months) | 99.6% (E) | 99.7% | 99.8% | 99.9% |

_All figures are illustrative scenario data for portfolio use._
