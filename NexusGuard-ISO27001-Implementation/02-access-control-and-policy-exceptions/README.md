<p align="center">
<img width="2800" height="680" alt="banner2" src="https://github.com/user-attachments/assets/4b17294c-e99c-47c6-aff5-41fd437d3336" />

</p>

# Access Control and Policy Exceptions

Fictional ISO 27001 access control package: Access Control Policy (joiner/mover/leaver, PAM, MFA, remote access, quarterly reviews), a risk-based Policy Exception Management Process with three worked examples, and three USB request decisions.

## What this project is

How a security team controls who gets access, and what happens when someone needs to depart from the rules. An internal review found 42 employees holding privileged access they no longer need, 8 former PayStream Analytics employees with active accounts, and no formal joiner/mover/leaver process. The package sets the access rules and a formal way to handle exceptions, and shows both applied to real requests.

## Contents

| # | Document | What it covers |
|---|---|---|
| 1 | [Access Control Policy](docs/01-access-control-policy.md) | Least privilege, need-to-know and separation of duties; joiner/mover/leaver with service levels; PAM; NIST 800-63B passwords and MFA mandate; remote access (VPN, ZTNA, jump servers); third-party access; mandatory quarterly reviews; logging; transitional deadlines |
| 2 | [Policy Exception Management Process](docs/02-policy-exception-management-process.md) | Six-step lifecycle with flowchart, request form, risk levels (Low to Critical), approval matrix, registry, review schedule and three worked examples (MFA on a legacy test environment, data routed through Europe, a scanning freeze) |
| 3 | USB request evaluations | Three decisions and a memo: [developer](docs/usb-evaluations/01-request-1-developer.md) (approve with conditions), [marketing manager](docs/usb-evaluations/02-request-2-marketing-manager.md) (deny), [database administrator](docs/usb-evaluations/03-request-3-database-administrator.md) (approve with conditions), and the [CISO memo](docs/usb-evaluations/04-ciso-memo.md) |

`files/` holds the Word versions, a PDF of the exception process, and a working Excel exception registry that calculates days to expiry and status. The provisioning procedure that implements this policy is SOP-A in project 04.

## How it supports ISO/IEC 27001:2022

| Requirement | Where it is addressed |
|---|---|
| A.5.15 Access control; A.5.16 Identity management | Access Control Policy, joiner/mover/leaver |
| A.5.17 Authentication information; A.8.5 Secure authentication | Passwords and MFA mandate |
| A.5.18 Access rights; A.8.2 Privileged access rights | Provisioning, quarterly reviews, PAM |
| A.5.3 Segregation of duties | Access principles and approval rules |
| A.7.10 Storage media | USB evaluations |
| A.5.36 Compliance with policies, rules and standards | Exception process and registry |
| Clause 5.3 Roles, responsibilities and authorities | Approval authority matrix |

## What this project demonstrates

- Writing access rules with deadlines that close real audit gaps
- Designing a risk-based exception process with approval levels, time limits and a registry
- Applying policy to real requests and documenting a defensible decision with conditions

## Scenario note

The exercises in this series used slightly different NexusGuard details in places (for example offices and headcount), so each document reflects the facts of its own scenario.

## Disclaimer

NexusGuard, its people, systems, incidents and figures are fictional and were created for skills practice and portfolio use. This is not legal advice or a compliance determination. Control and regulation references are paraphrased pointers, so verify them against the source text before relying on them.

## Author

