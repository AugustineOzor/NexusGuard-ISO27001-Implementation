# NexusGuard Technologies Ltd. | Information Asset Register | IAR-001

| Field | Detail |
|---|---|
| **Document Title** | Information Asset Register (IAR) |
| **Doc Ref.** | IAR-001 |
| **Classification** | Internal |
| **Status** | Draft for ISSC review |
| **Release Date** | 12/10/2026 |
| **Owner** | Chief Information Security Officer (CISO) |
| **Prepared by** | Augustine Ozor, GRC Analyst |
| **Requested by** | Michael Chen |
| **Next Review Date** | 12 months from approval, or sooner on material change or acquisition |

**Version history:** 1.0 | 12/10/2026 | Augustine Ozor | Register expanded from 15 to 45 assets, including 8 provisional PayStream Analytics assets.

Companion files: `IAR_Template_NexusGuard_Completed.xlsx` (source workbook), `NexusGuard_IAR_Summary_ISSC.pptx` and `.pdf` (ISSC presentation), [presentation in Markdown](NexusGuard_IAR_Summary_ISSC.md).

## 1. Summary

The register holds **45 assets**: the 15 template assets (AST-001 to AST-015) plus 30 added (AST-016 to AST-045), of which **8 are PayStream Analytics assets** (AST-038 to AST-045).

**By category**

| Category | Assets | % of register |
|---|---|---|
| Software | 12 | 27% |
| Hardware | 7 | 16% |
| Data Asset | 7 | 16% |
| Infrastructure | 8 | 18% |
| Facility | 5 | 11% |
| IT Service | 6 | 13% |

**By data classification**

| Classification | Assets | % of register |
|---|---|---|
| Public | 0 | 0% |
| Internal | 14 | 31% |
| Confidential | 18 | 40% |
| Restricted | 13 | 29% |

**By business criticality**

| Criticality | Assets | % of register |
|---|---|---|
| Low | 0 | 0% |
| Medium | 4 | 9% |
| High | 13 | 29% |
| Critical | 28 | 62% |

**By risk level**

| Risk level | Assets | % of register |
|---|---|---|
| Low | 1 | 2% |
| Medium | 17 | 38% |
| High | 27 | 60% |

**Classification vs criticality (asset count)**

| Classification | Low | Medium | High | Critical |
|---|---|---|---|---|
| Public | 0 | 0 | 0 | 0 |
| Internal | 0 | 4 | 1 | 9 |
| Confidential | 0 | 0 | 11 | 7 |
| Restricted | 0 | 0 | 1 | 12 |

## 2. Classification Guide

| Data Classification | Definition | Business Criticality | Definition |
|---|---|---|---|
| Public | Approved for unrestricted public release. | Low | Loss or unavailability causes minimal operational impact. |
| Internal | For NexusGuard personnel and authorized third parties; unauthorized disclosure causes limited harm. | Medium | Disruption affects a business process but workarounds are available. |
| Confidential | Sensitive business, customer, security, or employee information requiring controlled access. | High | Disruption causes major operational, financial, contractual, or reputational impact. |
| Restricted | Highly sensitive or regulated information requiring the strongest access and handling controls. | Critical | Loss or unavailability stops essential operations or creates severe regulatory or safety impact. |

| Risk Level | Guidance |
|---|---|
| Low | Adequate controls are in place and residual impact and likelihood are limited. |
| Medium | Additional monitoring or planned treatment is required. |
| High | Immediate management attention and formal risk treatment are required. |

## 3. Information Asset Register

| Asset ID | Asset Name | Description | Category | Owner | Custodian | Business Unit | Data Classification | Business Criticality | Location | Regulatory Relevance | Dependencies | Risk Level | Review Date |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| AST-001 | Microsoft Active Directory | Centralized identity, authentication, group policy, and access-control service for corporate users and systems. | Software | IT Infrastructure Manager | Systems Administration Team | Information Technology | Confidential | Critical | NexusGuard HQ Data Center | ISO 27001; HIPAA | VMware Cluster; DNS; Core Network | High | 2027-01-15 |
| AST-002 | Microsoft 365 Tenant | Corporate email, Microsoft Teams, SharePoint Online, OneDrive, and Office productivity services. | IT Service | Head of IT | Cloud Operations Team | Enterprise Services | Confidential | Critical | Microsoft Cloud | ISO 27001; HIPAA; GDPR | Microsoft Entra ID; Internet Connectivity | High | 2027-01-15 |
| AST-003 | HR Employee Database | Database containing employee personal information, payroll records, contracts, performance data, and benefits information. | Data Asset | Human Resources Director | Database Administration Team | Human Resources | Restricted | High | NexusGuard HQ Data Center | GDPR; HIPAA; Employment Law | Microsoft SQL Server; Active Directory | High | 2027-01-15 |
| AST-004 | Finance ERP System | Enterprise financial management platform supporting general ledger, accounts payable, billing, budgeting, and financial reporting. | Software | Chief Financial Officer | ERP Administration Team | Finance | Confidential | Critical | NexusGuard HQ Data Center | SOX; PCI DSS; ISO 27001 | Finance Database; Active Directory; Backup Service | High | 2027-01-15 |
| AST-005 | Salesforce CRM | Cloud-based customer relationship management platform containing customer contacts, sales opportunities, contracts, and support history. | Software | Sales Director | CRM Administrator | Sales and Marketing | Confidential | High | Salesforce Cloud | GDPR; ISO 27001 | Microsoft 365; Internet Connectivity; SSO | Medium | 2027-01-15 |
| AST-006 | Palo Alto Perimeter Firewall | Next-generation firewall protecting the corporate network and controlling inbound, outbound, and inter-segment traffic. | Hardware | Network and Security Manager | Network Operations Team | Information Technology | Internal | Critical | NexusGuard HQ Server Room | PCI DSS; HIPAA; ISO 27001 | ISP Links; Core Switches; SIEM Platform | High | 2027-01-15 |
| AST-007 | Corporate VPN Gateway | Secure remote-access service used by employees and approved third parties to connect to internal systems. | Infrastructure | Network and Security Manager | Network Operations Team | Information Technology | Confidential | Critical | NexusGuard HQ Data Center | HIPAA; PCI DSS; ISO 27001 | Perimeter Firewall; Active Directory; MFA Service | High | 2027-01-15 |
| AST-008 | VMware vSphere Cluster | Virtualization platform hosting critical production, security, database, and business application servers. | Infrastructure | IT Infrastructure Manager | Virtualization Team | Information Technology | Internal | Critical | NexusGuard HQ Data Center | ISO 27001; HIPAA; PCI DSS | SAN Storage; Core Network; Backup Service | High | 2027-01-15 |
| AST-009 | Veeam Backup Repository | Central repository storing encrypted backups of production servers, databases, file shares, and cloud workloads. | Data Asset | IT Operations Manager | Backup and Recovery Team | Information Technology | Restricted | Critical | NexusGuard Disaster Recovery Site | HIPAA; PCI DSS; ISO 27001 | Veeam Backup Server; Storage Array; WAN Link | High | 2027-01-15 |
| AST-010 | Microsoft Sentinel SIEM | Cloud security information and event management platform used for centralized logging, threat detection, alerting, and incident investigation. | Software | Security Operations Center Manager | SOC Analysts | Cybersecurity | Confidential | High | Microsoft Azure Cloud | HIPAA; PCI DSS; ISO 27001 | Log Sources; Microsoft Entra ID; Internet Connectivity | High | 2027-01-15 |
| AST-011 | Microsoft Defender for Endpoint | Endpoint detection and response platform protecting corporate laptops, workstations, and servers from malware and advanced threats. | Software | Security Operations Center Manager | Endpoint Management Team | Cybersecurity | Confidential | High | Microsoft Cloud | HIPAA; PCI DSS; ISO 27001 | Corporate Endpoints; Microsoft Entra ID; SIEM Platform | Medium | 2027-01-15 |
| AST-012 | Cisco Catalyst Core Switch Stack | Core switching infrastructure connecting servers, network segments, wireless services, firewalls, and internet gateways. | Hardware | Network and Security Manager | Network Operations Team | Information Technology | Internal | Critical | NexusGuard HQ Server Room | ISO 27001; PCI DSS | Perimeter Firewall; Access Switches; UPS | High | 2027-01-15 |
| AST-013 | NexusGuard Primary Server Room | Restricted facility housing production servers, storage, network equipment, backup systems, and supporting environmental controls. | Facility | Facilities Manager | Facilities and Physical Security Team | Facilities | Internal | Critical | NexusGuard Headquarters | HIPAA; PCI DSS; ISO 27001 | UPS; Generator; HVAC; Physical Access Control | High | 2027-01-15 |
| AST-014 | AWS Production Account | Primary AWS account hosting NexusGuard customer-facing applications, APIs, databases, storage, and cloud security services. | Infrastructure | Cloud Operations Manager | Cloud Engineering Team | Information Technology | Restricted | Critical | AWS US East Region | HIPAA; PCI DSS; ISO 27001 | AWS IAM; VPC; CloudTrail; Production Applications | High | 2027-01-15 |
| AST-015 | Cloudflare DNS and DDoS Protection | Authoritative DNS, web application firewall, content delivery, and distributed denial-of-service protection for public services. | IT Service | Network and Security Manager | Cloud Operations Team | Information Technology | Internal | Critical | Cloudflare Global Network | PCI DSS; ISO 27001 | Domain Registrar; Public Web Applications; Internet Connectivity | Medium | 2027-01-15 |
| AST-016 | NexusGuard Client Security Portal | Customer-facing web application where healthcare and enterprise clients view security reports, alerts, and compliance evidence. | Software | Chief Technology Officer | Application Engineering Team | Product Engineering | Restricted | Critical | AWS US East Region | HIPAA; PCI DSS; GDPR; ISO 27001 | AWS Production Account; Cloudflare DNS and DDoS Protection; Client PHI Database; Microsoft Entra ID | High | 2027-01-15 |
| AST-017 | GitHub Enterprise Cloud | Source code hosting, pull-request review, and CI/CD workflows for NexusGuard products and infrastructure-as-code. | Software | Chief Technology Officer | DevOps Team | Product Engineering | Confidential | High | GitHub Cloud | ISO 27001; PCI DSS | Microsoft Entra ID; HashiCorp Vault Secrets Manager; AWS Production Account | Medium | 2027-01-15 |
| AST-018 | HashiCorp Vault Secrets Manager | Central secrets and encryption-key management for application credentials, API keys, and database passwords. | Software | Chief Information Security Officer | Platform Security Team | Cybersecurity | Restricted | Critical | AWS US East Region | HIPAA; PCI DSS; ISO 27001 | AWS Production Account; Microsoft Entra ID; Veeam Backup and Replication Service | High | 2027-01-15 |
| AST-019 | Microsoft Entra ID | Cloud identity provider delivering single sign-on, conditional access, and multi-factor authentication for staff and cloud applications. | Software | Head of IT | Identity and Access Management Team | Information Technology | Confidential | Critical | Microsoft Cloud | HIPAA; PCI DSS; GDPR; ISO 27001 | Microsoft Active Directory; Internet Connectivity | High | 2027-01-15 |
| AST-020 | Employee Laptop Fleet | Company-managed laptops used by staff in Dubai, London, and New York, with full-disk encryption and endpoint protection. | Hardware | Head of IT | End-User Computing Team | Information Technology | Confidential | High | Dubai, London, and New York Offices | HIPAA; PCI DSS; GDPR; ISO 27001 | Microsoft Defender for Endpoint; Microsoft 365 Tenant; Corporate VPN Gateway | Medium | 2027-01-15 |
| AST-021 | Dell PowerEdge Server Hosts | Physical servers running the VMware vSphere cluster for production, security, and business application workloads. | Hardware | IT Infrastructure Manager | Systems Administration Team | Information Technology | Internal | Critical | NexusGuard HQ Data Center | ISO 27001; HIPAA; PCI DSS | VMware vSphere Cluster; NetApp SAN Storage Array; NexusGuard HQ Data Center | Medium | 2027-01-15 |
| AST-022 | NetApp SAN Storage Array | Shared storage array holding virtual machine disks, databases, and file shares for the on-premises environment. | Hardware | IT Infrastructure Manager | Storage Team | Information Technology | Restricted | Critical | NexusGuard HQ Data Center | HIPAA; PCI DSS; ISO 27001 | Dell PowerEdge Server Hosts; Cisco Catalyst Core Switch Stack; Veeam Backup Repository | High | 2027-01-15 |
| AST-023 | Healthcare IoMT Test Lab Devices | Infusion pumps, patient monitors, and imaging gateways used in the security lab to test client medical-device defenses with synthetic data. | Hardware | Security Services Director | Security Lab Team | Security Services | Internal | Medium | NexusGuard HQ Security Lab | HIPAA; ISO 27001 | Isolated Lab Network Segment; Palo Alto Perimeter Firewall | Low | 2027-01-15 |
| AST-024 | Client PHI Database | Production database storing protected health information processed for healthcare clients' security monitoring and reporting. | Data Asset | Chief Technology Officer | Database Administration Team | Product Engineering | Restricted | Critical | AWS US East Region | HIPAA; GDPR; ISO 27001 | AWS Production Account; HashiCorp Vault Secrets Manager; AWS Cross-Region Backup Vault | High | 2027-01-15 |
| AST-025 | Corporate File Shares | Departmental network and SharePoint file shares holding internal documents, project files, and working papers. | Data Asset | Head of IT | Systems Administration Team | Enterprise Services | Confidential | High | NexusGuard HQ Data Center | ISO 27001; GDPR | Microsoft Active Directory; NetApp SAN Storage Array; Veeam Backup Repository | Medium | 2027-01-15 |
| AST-026 | Security Log Archive | Long-term archive of firewall, authentication, application, and cloud audit logs retained for investigations and compliance. | Data Asset | Security Operations Center Manager | SOC Analysts | Cybersecurity | Confidential | High | AWS US East Region | HIPAA; PCI DSS; ISO 27001 | Microsoft Sentinel SIEM; AWS CloudTrail; AWS Production Account | Medium | 2027-01-15 |
| AST-027 | AWS Cross-Region Backup Vault | Encrypted copies of production databases and storage snapshots replicated to a secondary region for disaster recovery. | Data Asset | IT Operations Manager | Cloud Engineering Team | Information Technology | Restricted | Critical | AWS US West Region | HIPAA; PCI DSS; ISO 27001 | AWS Production Account; Client PHI Database; HashiCorp Vault Secrets Manager | Medium | 2027-01-15 |
| AST-028 | AWS Staging Account | Pre-production AWS account used to test releases and integrations using masked or synthetic data. | Infrastructure | Cloud Operations Manager | Cloud Engineering Team | Information Technology | Internal | Medium | AWS US East Region | ISO 27001 | AWS Production Account; GitHub Enterprise Cloud; Microsoft Entra ID | Medium | 2027-01-15 |
| AST-029 | Segmented Production and PHI Network | VLAN and firewall-zone design isolating production servers, PHI systems, and payment-related systems from the corporate LAN. | Infrastructure | Network and Security Manager | Network Operations Team | Information Technology | Confidential | Critical | NexusGuard HQ Data Center | HIPAA; PCI DSS; ISO 27001 | Palo Alto Perimeter Firewall; Cisco Catalyst Core Switch Stack; VMware vSphere Cluster | High | 2027-01-15 |
| AST-030 | Site-to-Site VPN Tunnels | Encrypted tunnels linking the London and New York offices and cloud environments to the Dubai headquarters network. | Infrastructure | Network and Security Manager | Network Operations Team | Information Technology | Confidential | High | NexusGuard HQ Data Center | ISO 27001; HIPAA; GDPR | Palo Alto Perimeter Firewall; ISP Links; AWS Production Account | Medium | 2027-01-15 |
| AST-031 | NexusGuard HQ Data Center | On-premises data center at the Dubai headquarters housing core servers, storage, and network equipment with resilient power and cooling. | Facility | Facilities Manager | Facilities and Physical Security Team | Facilities | Internal | Critical | NexusGuard Headquarters, Dubai | HIPAA; PCI DSS; ISO 27001; UAE NESA | UPS; Generator; HVAC; Physical Access Control | High | 2027-01-15 |
| AST-032 | NexusGuard Disaster Recovery Site | Secondary site hosting backup repositories and standby recovery capacity for critical on-premises systems. | Facility | Facilities Manager | Facilities and Physical Security Team | Facilities | Internal | Critical | NexusGuard Disaster Recovery Site | HIPAA; PCI DSS; ISO 27001 | UPS; WAN Link; Veeam Backup Repository; Physical Access Control | Medium | 2027-01-15 |
| AST-033 | NexusGuard London Office | Regional office for sales, client support, and engineering staff serving UK and European clients. | Facility | Facilities Manager | Facilities and Physical Security Team | Facilities | Internal | Medium | London, United Kingdom | ISO 27001; UK GDPR | Site-to-Site VPN Tunnels; Employee Laptop Fleet; Physical Access Control | Medium | 2027-01-15 |
| AST-034 | NexusGuard New York Office | Regional office for sales, client support, and engineering staff serving North American clients. | Facility | Facilities Manager | Facilities and Physical Security Team | Facilities | Internal | Medium | New York, United States | ISO 27001; HIPAA | Site-to-Site VPN Tunnels; Employee Laptop Fleet; Physical Access Control | Medium | 2027-01-15 |
| AST-035 | Internal DNS and DHCP Services | Internal name resolution and IP address assignment services supporting servers, endpoints, and Active Directory. | IT Service | IT Infrastructure Manager | Network Operations Team | Information Technology | Internal | Critical | NexusGuard HQ Data Center | ISO 27001; PCI DSS | Microsoft Active Directory; Cisco Catalyst Core Switch Stack; VMware vSphere Cluster | Medium | 2027-01-15 |
| AST-036 | Veeam Backup and Replication Service | Backup orchestration service scheduling, monitoring, and restoring backups of servers, databases, and file shares. | IT Service | IT Operations Manager | Backup and Recovery Team | Information Technology | Confidential | Critical | NexusGuard HQ Data Center | HIPAA; PCI DSS; ISO 27001 | Veeam Backup Repository; VMware vSphere Cluster; NexusGuard Disaster Recovery Site | High | 2027-01-15 |
| AST-037 | Datadog Monitoring and Observability | Infrastructure and application monitoring service providing performance metrics, uptime alerts, and dashboards for cloud workloads. | IT Service | Cloud Operations Manager | Cloud Operations Team | Information Technology | Internal | High | Datadog Cloud | ISO 27001 | AWS Production Account; NexusGuard Client Security Portal; Internet Connectivity | Medium | 2027-01-15 |
| AST-038 | PayStream Payment Analytics Platform | Core PayStream application that analyzes merchant transaction data and delivers fraud and spend insights to clients. | Software | PayStream Head of Engineering | PayStream Platform Team | PayStream Analytics | Restricted | Critical | PayStream AWS Account | PCI DSS; GDPR; ISO 27001 | PayStream Transaction Data Warehouse; PayStream Cardholder Data Environment; PayStream Customer API Gateway | High | 2026-12-15 |
| AST-039 | PayStream Cardholder Data Environment | Segmented network and systems that store, process, or transmit payment card data within PayStream's PCI DSS scope. | Infrastructure | PayStream Head of Engineering | PayStream Platform Team | PayStream Analytics | Restricted | Critical | PayStream AWS Account | PCI DSS; GDPR; ISO 27001 | PayStream AWS Account; PayStream Payment HSM; PayStream Transaction Data Warehouse | High | 2026-12-15 |
| AST-040 | PayStream Transaction Data Warehouse | Data warehouse of merchant and cardholder transaction records used for analytics, reporting, and model training. | Data Asset | PayStream Head of Engineering | PayStream Data Engineering Team | PayStream Analytics | Restricted | Critical | PayStream AWS Account | PCI DSS; GDPR; ISO 27001 | PayStream AWS Account; PayStream Cardholder Data Environment; PayStream Payment Analytics Platform | High | 2026-12-15 |
| AST-041 | PayStream Payment HSM | Hardware security module protecting cryptographic keys used to encrypt and tokenize payment card data. | Hardware | PayStream Head of Engineering | PayStream Platform Team | PayStream Analytics | Restricted | Critical | PayStream Co-location Facility | PCI DSS; ISO 27001 | PayStream Cardholder Data Environment; Co-location Power and Cooling | High | 2026-12-15 |
| AST-042 | PayStream Customer API Gateway | Public API gateway exposing PayStream analytics and reporting endpoints to merchant and enterprise clients. | Software | PayStream Head of Engineering | PayStream Platform Team | PayStream Analytics | Confidential | High | PayStream AWS Account | PCI DSS; GDPR; ISO 27001 | PayStream Payment Analytics Platform; PayStream AWS Account; Internet Connectivity | High | 2026-12-15 |
| AST-043 | PayStream AWS Account | Cloud account hosting PayStream applications, data warehouse, and API services, not yet aligned to NexusGuard cloud baselines. | Infrastructure | PayStream Head of Engineering | PayStream Platform Team | PayStream Analytics | Restricted | Critical | AWS Cloud (PayStream-managed) | PCI DSS; GDPR; ISO 27001 | AWS IAM; CloudTrail; PayStream Cardholder Data Environment | High | 2026-12-15 |
| AST-044 | PayStream Legacy Active Directory | Separate PayStream directory service authenticating PayStream staff, pending migration into NexusGuard identity services. | Software | PayStream IT Lead | PayStream IT Team | PayStream Analytics | Confidential | High | PayStream Office | ISO 27001; GDPR | Microsoft Entra ID; PayStream Office Network | High | 2026-12-15 |
| AST-045 | PayStream Corporate Email Tenant | Separate Microsoft 365 tenant used by PayStream staff for email and collaboration until tenant consolidation. | IT Service | PayStream IT Lead | PayStream IT Team | PayStream Analytics | Confidential | High | Microsoft Cloud | ISO 27001; GDPR | Microsoft Entra ID; Internet Connectivity; Microsoft 365 Tenant | Medium | 2026-12-15 |

## 4. Notes

- PayStream entries (AST-038 to AST-045) are provisional. They were built from acquisition documentation and must be validated against PayStream asset discovery before the next review.
- Review Date is the next scheduled review. PayStream assets are set earlier (2026-12-15) because integration is unfinished.
- Risk Level follows the Classification Guide. Ratings are initial judgments pending formal risk assessment.
- All organizations, assets and ratings are fictional and created for skills practice and portfolio use.
