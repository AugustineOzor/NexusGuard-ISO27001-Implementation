<p align="center">
<img width="2800" height="680" alt="banner4" src="https://github.com/user-attachments/assets/6c693cbd-6f6e-47cd-b6da-24cc749f9c50" />

</p>

# Asset Register and Security SOPs

Fictional ISO 27001 operations pack: a 45-asset Information Asset Register with ISSC findings deck, plus four SOPs with flowcharts for access provisioning, incident classification, vulnerability patching and third-party vendor onboarding.

## What this project is

The operational evidence an ISO 27001 auditor asks for. NexusGuard never kept a formal asset register, and had policies but no documented procedures. This pack builds the register that everything else depends on, and the step-by-step procedures that show staff know how to do the work.

## Contents

| Area | Document | What it covers |
|---|---|---|
| Asset register | [Information Asset Register](docs/asset-register/IAR_NexusGuard_Completed.md) | 45 assets in six categories (8 from an acquired company), with owner, custodian, classification, criticality, regulatory relevance, dependencies and risk |
| | [ISSC summary deck](docs/asset-register/NexusGuard_IAR_Summary_ISSC.md) | Approach, key findings (27 of 45 assets rated High risk; two services each support nine other assets) and five decisions for the committee |
| SOPs | [SOP-A User Access Provisioning](docs/sops/SOP-A_User_Access_Provisioning.md) | Joiner, mover and leaver lifecycle with flowchart and service levels |
| | [SOP-B Incident Classification and Escalation](docs/sops/SOP-B_Incident_Classification_and_Escalation.md) | 15 steps, severity scale, escalation times and notification clocks |
| | [SOP-C Vulnerability Scanning and Patch Management](docs/sops/SOP-C_Vulnerability_Scanning_and_Patch_Management.md) | 14 steps, scan schedule, priority and fix times, verification |
| | [SOP-D Third-Party Vendor Security Onboarding](docs/sops/SOP-D_Third_Party_Vendor_Security_Onboarding.md) | 13 steps, vendor tiers, contract terms and go-live gate |

SOP-B, C and D follow an 11-section standard: header, purpose, scope, definitions, roles, procedure, flow diagram, exceptions, related documents, ISO control mapping and document history.

`files/` holds the register workbook, the ISSC deck (PowerPoint and PDF), and the Word and PDF versions of each SOP.

## How it supports ISO/IEC 27001:2022

| Requirement | Where it is addressed |
|---|---|
| A.5.9 Inventory of information and other associated assets | Information Asset Register |
| A.5.12 Classification of information | Register classification and criticality |
| A.5.18 Access rights; A.8.2 Privileged access rights | SOP-A |
| A.5.24 to A.5.28 Incident management; A.6.8 Event reporting | SOP-B |
| A.8.8 Management of technical vulnerabilities; A.8.32 Change management | SOP-C |
| A.5.19 to A.5.23 Supplier relationships and cloud services | SOP-D |

## What this project demonstrates

- Building and populating an asset register, and turning it into findings for management
- Writing SOPs with triggers, decision points, flowcharts, exceptions and ISO control mapping
- Linking asset data to risk, so response and patching follow business criticality

## Scenario note

The exercises in this series used slightly different NexusGuard details in places (for example offices and headcount), so each document reflects the facts of its own scenario.

## Disclaimer

NexusGuard, its people, systems, incidents and figures are fictional and were created for skills practice and portfolio use. This is not legal advice or a compliance determination. Control and regulation references are paraphrased pointers, so verify them against the source text before relying on them.


