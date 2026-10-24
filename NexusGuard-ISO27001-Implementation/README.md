<p align="center">
  <img width="2800" height="680" alt="banner" src="https://github.com/user-attachments/assets/e3f2a9d6-cc87-4424-a763-9d472116d636" />

</p>

# NexusGuard ISO 27001 Implementation

A fictional end-to-end ISO/IEC 27001:2022 implementation for **NexusGuard Technologies Ltd.**, a technology company handling PHI, payment card data and personal data. It starts from very little (an outdated 2021 policy, no asset register, no committee charters, no metrics, no documented procedures) and builds the documents an ISMS needs, grouped into five projects.

## The five projects

| # | Project | Description |
|---|---|---|
| 01 | [**Information Security Policy Suite**](01-information-security-policy-suite/README.md)<br>`nexusguard-information-security-policy-suite` | Fictional ISO 27001 policy suite for a tech company: Information Security Policy v3.0 with a 16-gap analysis, Acceptable Use Policy and Data Classification and Handling Policy, each with a one-page employee quick reference guide. |
| 02 | [**Access Control and Policy Exceptions**](02-access-control-and-policy-exceptions/README.md)<br>`nexusguard-access-control-and-policy-exceptions` | Fictional ISO 27001 access control package: Access Control Policy (joiner/mover/leaver, PAM, MFA, remote access, quarterly reviews), a risk-based Policy Exception Management Process with three worked examples, and three USB request decisions. |
| 03 | [**ISMS Governance, Risk and Metrics**](03-isms-governance-risk-and-metrics/README.md)<br>`nexusguard-isms-governance-risk-metrics` | Fictional ISO 27001 governance toolkit: ISSC, Risk and Compliance committee charters, board and ISSC report templates, a 26-metric GRC KPI framework with baseline narrative and Excel dashboard, and a 42-activity RACI matrix. |
| 04 | [**Asset Register and Security SOPs**](04-asset-register-and-security-sops/README.md)<br>`nexusguard-asset-register-and-security-sops` | Fictional ISO 27001 operations pack: a 45-asset Information Asset Register with ISSC findings deck, plus four SOPs with flowcharts for access provisioning, incident classification, vulnerability patching and third-party vendor onboarding. |
| 05 | [**Security Awareness Program FY2026**](05-security-awareness-program/README.md)<br>`nexusguard-security-awareness-program` | Fictional role-based security awareness program for 450 staff: program plan, 12-month calendar with KPI targets, and a 15-slide phishing training module, mapped to ISO 27001 A.6.3, HIPAA and PCI DSS 12.6. |

## How the projects fit together

| ISMS area | Project | Typical ISO/IEC 27001:2022 reference |
|---|---|---|
| Leadership, roles, objectives and measurement | 03 ISMS Governance, Risk and Metrics | Clauses 5.1, 5.3, 6.2, 9.1, 9.3; A.5.2, A.5.4 |
| Policies | 01 Information Security Policy Suite | Clause 5.2; A.5.1, A.5.10, A.5.12, A.5.13 |
| Access and exceptions | 02 Access Control and Policy Exceptions | A.5.15 to A.5.18, A.8.2, A.8.5, A.5.36 |
| Assets and operational procedures | 04 Asset Register and Security SOPs | A.5.9, A.5.19 to A.5.28, A.8.8 |
| People | 05 Security Awareness Program | Clause 7.3; A.6.3 |

**Suggested reading order:** 03 (who governs and how success is measured), 01 (the rules), 02 (access and exceptions), 04 (assets and procedures), 05 (people).

## Banners

### 01. Information Security Policy Suite

<a href="01-information-security-policy-suite/README.md"><img src="01-information-security-policy-suite/assets/banner.jpg" alt="Information Security Policy Suite" width="100%"></a>

### 02. Access Control and Policy Exceptions

<a href="02-access-control-and-policy-exceptions/README.md"><img src="02-access-control-and-policy-exceptions/assets/banner.jpg" alt="Access Control and Policy Exceptions" width="100%"></a>

### 03. ISMS Governance, Risk and Metrics

<a href="03-isms-governance-risk-and-metrics/README.md"><img src="03-isms-governance-risk-and-metrics/assets/banner.jpg" alt="ISMS Governance, Risk and Metrics" width="100%"></a>

### 04. Asset Register and Security SOPs

<a href="04-asset-register-and-security-sops/README.md"><img src="04-asset-register-and-security-sops/assets/banner.jpg" alt="Asset Register and Security SOPs" width="100%"></a>

### 05. Security Awareness Program FY2026

<a href="05-security-awareness-program/README.md"><img src="05-security-awareness-program/assets/banner.jpg" alt="Security Awareness Program FY2026" width="100%"></a>

## Folder layout

```
NexusGuard-ISO27001-Implementation/
├── README.md
├── 01-information-security-policy-suite/
├── 02-access-control-and-policy-exceptions/
├── 03-isms-governance-risk-and-metrics/
├── 04-asset-register-and-security-sops/
└── 05-security-awareness-program/
    ├── README.md
    ├── REPO_DESCRIPTION.txt
    ├── assets/banner.jpg
    ├── docs/        Markdown documents (and diagrams)
    └── files/       Word, Excel, PowerPoint and PDF versions
```

## Publishing

Publish the whole folder as one repository, or publish each project as its own repository. For one project, copy its contents (not the numbered folder itself) to a new repository. Each project's `REPO_DESCRIPTION.txt` has a repository name, About text and topics. Add a license file before publishing, otherwise the default is all rights reserved.

## Disclaimer

NexusGuard, its people, systems, incidents and figures are fictional and were created for skills practice and portfolio use. This is not legal advice or a compliance determination. Control and regulation references are paraphrased pointers, so verify them against the source text before relying on them. The exercises in this series used slightly different NexusGuard details in places (for example offices and headcount), so each document reflects the facts of its own scenario.

## Author
