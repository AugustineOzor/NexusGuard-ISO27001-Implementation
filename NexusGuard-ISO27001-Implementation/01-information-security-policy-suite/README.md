<p align="center">
  <img width="2800" height="680" alt="banner1" src="https://github.com/user-attachments/assets/95fe252d-0db7-4faa-a93b-f0fb7f70931f" />

</p>

# Information Security Policy Suite

Fictional ISO 27001 policy suite for a tech company: Information Security Policy v3.0 with a 16-gap analysis, Acceptable Use Policy and Data Classification and Handling Policy, each with a one-page employee quick reference guide.

## What this project is

The policy layer of an ISO/IEC 27001:2022 implementation. NexusGuard's only policy was a 2021 document with no regulatory basis, no classification scheme and no enforceable language. This suite replaces it with an umbrella policy, two topic policies that fix the specific gaps (acceptable use and data handling), and short guides that staff will actually read.

## Contents

| # | Document | What it covers |
|---|---|---|
| 1 | [Information Security Policy v3.0](docs/01-information-security-policy-v3.md) | Objectives, roles, policy hierarchy, 15 security domains, breach notification clocks, regulatory crosswalk, enforcement, exceptions and document control |
| 2 | [Policy Gap Analysis Report](docs/02-policy-gap-analysis-report.md) | 16 gaps in the 2021 policy (6 Critical, 9 High, 1 Medium) with old text, new requirement and rationale |
| 3 | [Acceptable Use Policy](docs/03-acceptable-use-policy.md) | Company devices, BYOD, internet, email, cloud and AI tools, prohibited activities, remote work, monitoring and four sanction tiers, with a signed acknowledgment form |
| 4 | [AUP Quick Reference Card](docs/04-aup-quick-reference-card.md) | One-page do and don't card for workstations |
| 5 | [Data Classification and Handling Policy](docs/05-data-classification-and-handling-policy.md) | Four-tier scheme, handling rules for PHI, card data, personal data and source code, labeling, cross-border transfers and retention |
| 6 | [Data Handling Quick Reference Guide](docs/06-data-handling-quick-reference-guide.md) | Two-page guide: which tier is it, and how to handle it |

`files/` holds the Word versions of each document.

## How it supports ISO/IEC 27001:2022

| Requirement | Where it is addressed |
|---|---|
| Clause 5.2 Information security policy | Document 1 |
| A.5.1 Policies for information security | Documents 1 to 5 |
| A.5.10 Acceptable use of information and assets | Documents 3 and 4 |
| A.5.12 and A.5.13 Classification and labelling | Documents 5 and 6 |
| A.5.14 Information transfer; A.5.34 Privacy and PII | Documents 1 and 5 |
| A.6.4 Disciplinary process | Documents 1 and 3 |

## What this project demonstrates

- Replacing a weak policy with measurable, enforceable requirements ("shall", targets, sanctions)
- Mapping each domain to ISO 27001, HIPAA, PCI DSS, GDPR, NIST CSF and UAE NESA
- Designing a four-tier classification scheme and handling rules for four data types
- Turning policy into short, employee-friendly guidance

## Scenario note

The exercises in this series used slightly different NexusGuard details in places (for example offices and headcount), so each document reflects the facts of its own scenario.

## Disclaimer

NexusGuard, its people, systems, incidents and figures are fictional and were created for skills practice and portfolio use. This is not legal advice or a compliance determination. Control and regulation references are paraphrased pointers, so verify them against the source text before relying on them.

## Author


