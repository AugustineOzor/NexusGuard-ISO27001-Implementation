# NexusGuard Information Asset Register: Summary for the ISSC

_Briefing for the Information Security Steering Committee | October 2026 | Augustine Ozor, GRC Analyst_

Companion files: `NexusGuard_IAR_Summary_ISSC.pptx` and `.pdf` (8 slides), [full register in Markdown](IAR_NexusGuard_Completed.md).

---

## Slide 1: Information Asset Register: approach and key findings

- Briefing for the Information Security Steering Committee
- Register grew from **15** assets (template) to **45** assets today

**Speaker notes:** The register moved from 15 example assets to 45 assets, including eight provisional PayStream Analytics assets. The next slides explain why we needed it, how it was built, and what it shows.

---

## Slide 2: Why a register, and why now

| Driver | Why it matters |
|---|---|
| **Audit observation** | We are ISO 27001 certified, yet the previous auditor noted we have never kept a formal asset register. |
| **PayStream assets** | The 2025 acquisition brings 40+ new assets that need owners, classification and risk ratings. |
| **HIPAA and PCI DSS** | Both require precise inventories of systems and the regulated data they hold. |

**Speaker notes:** Three drivers. First, the audit observation. Second, PayStream. Third, HIPAA and PCI DSS expect a precise inventory, which we cannot demonstrate without a register.

---

## Slide 3: How we built the register

1. **Collect:** CTO spreadsheets and system documentation, reviewed against the 15 template assets.
2. **Classify:** Four-level data classification and four-level business criticality from the Classification Guide.
3. **Assign:** Named owner, custodian and business unit for every asset.
4. **Assess and review:** Risk level, regulatory relevance, dependencies and a review date.

**14 required fields per asset:** ID, name, description, category, owner, custodian, business unit, classification, criticality, location, regulatory relevance, dependencies, risk level, review date.

**Speaker notes:** The approach follows the NexusGuard template: collect, classify, assign accountability, then assess risk and set a review date. Every asset has all 14 fields completed.

---

## Slide 4: The register at a glance

| Measure | Value |
|---|---|
| Assets registered | 45 |
| From PayStream Analytics | 8 |
| Restricted data assets | 13 |
| Rated Critical | 28 |

**Assets by category**

| Category | Assets |
|---|---|
| Software | 12 |
| Infrastructure | 8 |
| Hardware | 7 |
| Data Asset | 7 |
| IT Service | 6 |
| Facility | 5 |

**Speaker notes:** Forty-five assets across all six categories. Eight come from PayStream. Thirteen hold Restricted data, and 28 are rated Critical for the business.

---

## Slide 5: Most critical assets carry high risk

- **27 of 45** assets (60%) are rated High risk and need formal treatment.
- **23 of 28** Critical assets are also rated High risk.

**Risk level by category (assets)**

| Category | High | Medium | Low |
|---|---|---|---|
| Software | 9 | 3 | 0 |
| Infrastructure | 6 | 2 | 0 |
| Hardware | 4 | 2 | 1 |
| Data Asset | 4 | 3 | 0 |
| IT Service | 2 | 4 | 0 |
| Facility | 2 | 3 | 0 |

_Risk levels are initial judgments pending formal risk assessment._

**Speaker notes:** Sixty percent of the register is rated High risk, and 23 of the 28 Critical assets are High. These ratings are initial judgments from the register build and need confirmation through formal risk assessment.

---

## Slide 6: Four findings for the ISSC

1. **9 and 9:** AWS Production Account and Microsoft Entra ID each support nine other assets, so they are single points of concentration.
2. **14 of 45:** assets (31%) sit in the HQ data center or server room, with one recorded DR site as the fallback.
3. **23 critical:** assets are rated High risk, which calls for formal risk treatment under the guide.
4. **5 owners:** hold 26 of 45 assets (58%), so accountability rests with a few managers.

**Speaker notes:** Concentration is the theme. Two services underpin nine assets each. Almost a third of assets are physically in the HQ data center. Most critical assets are High risk and need formal treatment. Five owners hold 58 percent of the assets.

---

## Slide 7: PayStream: first tranche recorded

**8 of 40+** assets recorded; 32 or more still to discover.

- 7 of 8 rated High risk; 5 hold Restricted data.
- Legacy Active Directory and AWS account are not yet aligned to NexusGuard baselines.
- Entries are provisional; review date set to 15 Dec 2026.

| ID | Asset | Classification | Risk |
|---|---|---|---|
| AST-038 | Payment Analytics Platform | Restricted | High |
| AST-039 | Cardholder Data Environment | Restricted | High |
| AST-040 | Transaction Data Warehouse | Restricted | High |
| AST-041 | Payment HSM | Restricted | High |
| AST-042 | Customer API Gateway | Confidential | High |
| AST-043 | AWS Account | Restricted | High |
| AST-044 | Legacy Active Directory | Confidential | High |
| AST-045 | Corporate Email Tenant | Confidential | Medium |

**Speaker notes:** Eight PayStream assets are recorded so far, about a fifth of the expected 40 or more. They are built from acquisition documentation and must be validated through discovery. Seven of the eight are High risk, mainly because identity and cloud controls are not yet aligned.

---

## Slide 8: Decisions requested from the ISSC

1. **Approve the register** as the authoritative asset inventory, owned by the CISO and reviewed at least quarterly.
2. **Require owner attestation** from every asset owner to confirm entries within 30 days.
3. **Fund PayStream discovery** to find the remaining 32+ assets within 90 days.
4. **Start risk treatment** for the 23 Critical, High-risk assets, beginning with AWS, Entra ID and the cardholder environment.
5. **Embed the register** in procurement and change management so new assets are recorded at onboarding.

**Speaker notes:** Five decisions. The timings are recommendations for the committee to confirm. The register is only useful if owners attest to it and it is kept current through procurement and change management.
