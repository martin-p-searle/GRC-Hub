# SecureCorp Statement of Applicability (Fictional)

| | |
|---|---|
| **Document owner** | Information Security Manager |
| **Version** | 1.1 (status review) |
| **First approved** | 26 January 2026 (v1.0) |
| **Status as at** | 1 October 2026 |
| **Approved by** | Risk Committee (CEO, CFO, CIO, ISM) |
| **Next review** | Quarterly status review; full review January 2027 |
| **Standard** | ISO/IEC 27001:2022, clause 6.1.3 d) |

*SecureCorp is a fictional organisation created for training purposes.*

## 1. Purpose

This Statement of Applicability (SoA) records which of the 93 Annex A controls apply to SecureCorp's ISMS, why, and whether each is implemented. Controls were chosen to treat the risks in the [Risk Assessment Report](risk-assessment-report.md) (R1 to R8) and to meet legal, contractual and good-practice requirements. A summary of the main controls is in the [Security Controls](../security-measures/security-controls.md) document.

## 2. Summary

| Measure | Count |
|---|---|
| Controls assessed | 93 |
| Applicable | 91 |
| Not applicable | 2 |

| Status of applicable controls | Count |
|---|---|
| Implemented | 77 |
| In progress | 11 |
| Planned | 3 |

Open items to note: control 5.26 (incident response) is still in progress after the 30 June 2026 target in the risk assessment, so the residual score for R7 has not yet reached its target of 8. The Risk Committee extended the date to 31 December 2026 (see section 8 of the risk assessment). Controls 5.35 and 5.36 are planned for the first internal audit and management review in Months 10-12.

## 3. Key

**Justification:** R1 to R8 refer to the risks in the [Risk Assessment Report](risk-assessment-report.md). Legal and contractual drivers are named where they apply.

**Status:** Implemented (operating), In progress (partly in place), Planned (scheduled, not started), Not applicable (excluded, with reason).

**Owners:** ISM = Information Security Manager; CIO = Chief Information Officer; CEO = Chief Executive Officer; HoIT = Head of IT; HRD = HR Director; DPO = Data Protection Officer; PL = Procurement Lead; FM = Facilities Manager.

## 4. Organizational controls (5.1 to 5.37)

| Ref | Control | Applicable | Justification | Status | Owner |
|---|---|---|---|---|---|
| 5.1 | Policies for information security | Yes | Management direction; ISO 27001 clause 5.2 requirement; all risks | Implemented | ISM |
| 5.2 | Information security roles and responsibilities | Yes | Clause 5.3 requirement; named owners for R1 to R8 | Implemented | ISM |
| 5.3 | Segregation of duties | Yes | Reduces fraud and error; R8 | Implemented | CIO |
| 5.4 | Management responsibilities | Yes | Leadership must require staff to apply policy; R8 | Implemented | CEO |
| 5.5 | Contact with authorities | Yes | ICO breach notification (R7); law enforcement and NCSC contact | Implemented | DPO |
| 5.6 | Contact with special interest groups | Yes | Threat awareness for R1 and R3 (e.g., NCSC CiSP) | Implemented | ISM |
| 5.7 | Threat intelligence | Yes | Informs likelihood scoring for R1 to R3; feeds are live but not yet reviewed monthly | In progress | ISM |
| 5.8 | Information security in project management | Yes | New features and client onboarding projects affect R3 and R7 | Implemented | CIO |
| 5.9 | Inventory of information and other associated assets | Yes | Basis of the risk assessment; R6. Cloud assets still being added | In progress | HoIT |
| 5.10 | Acceptable use of information and other associated assets | Yes | R1, R8 | Implemented | HRD |
| 5.11 | Return of assets | Yes | R4, R6; part of the leaver process | Implemented | HRD |
| 5.12 | Classification of information | Yes | R7; UK GDPR; client contracts | Implemented | DPO |
| 5.13 | Labelling of information | Yes | Supports classification and DLP rules (R7); labels applied to new documents first | In progress | DPO |
| 5.14 | Information transfer | Yes | Client files move by secure transfer and email; R5, R7 | Implemented | HoIT |
| 5.15 | Access control | Yes | R4, R8 | Implemented | HoIT |
| 5.16 | Identity management | Yes | R4 | Implemented | HoIT |
| 5.17 | Authentication information | Yes | R1 | Implemented | CIO |
| 5.18 | Access rights | Yes | R4; quarterly access reviews | Implemented | HRD |
| 5.19 | Information security in supplier relationships | Yes | R5 | Implemented | PL |
| 5.20 | Addressing information security within supplier agreements | Yes | R5; client 48-hour breach notification flows down to suppliers | Implemented | PL |
| 5.21 | Managing information security in the ICT supply chain | Yes | R5; cloud and SaaS dependencies; fourth-party mapping under way | In progress | PL |
| 5.22 | Monitoring, review and change management of supplier services | Yes | R5; annual review of critical suppliers | Implemented | PL |
| 5.23 | Information security for use of cloud services | Yes | Production platform is cloud-hosted; R5 | Implemented | CIO |
| 5.24 | Information security incident management planning and preparation | Yes | R2, R7 | Implemented | ISM |
| 5.25 | Assessment and decision on information security events | Yes | R2, R7 | Implemented | ISM |
| 5.26 | Response to information security incidents | Yes | R2, R7; ICO 72-hour notification. Tabletop exercise outstanding | In progress | ISM |
| 5.27 | Learning from information security incidents | Yes | Clause 10 improvement; lessons-learned step added after first exercise | Planned | ISM |
| 5.28 | Collection of evidence | Yes | R2, R7, R8; forensic readiness | In progress | ISM |
| 5.29 | Information security during disruption | Yes | R2 | Implemented | CIO |
| 5.30 | ICT readiness for business continuity | Yes | R2; 99.9% availability objective | Implemented | CIO |
| 5.31 | Legal, statutory, regulatory and contractual requirements | Yes | UK GDPR; Data Protection Act 2018; client contracts; R7 | Implemented | DPO |
| 5.32 | Intellectual property rights | Yes | Licensed software and client-owned content | Implemented | HoIT |
| 5.33 | Protection of records | Yes | Retention obligations; R7 | Implemented | DPO |
| 5.34 | Privacy and protection of PII | Yes | UK GDPR; R7 | Implemented | DPO |
| 5.35 | Independent review of information security | Yes | Clause 9.2 internal audit; first cycle in Months 10-12 | Planned | ISM |
| 5.36 | Compliance with policies, rules and standards for information security | Yes | Clause 9.3 management review input; first review in Months 10-12 | Planned | ISM |
| 5.37 | Documented operating procedures | Yes | Consistent operations; R3, R4 | Implemented | HoIT |

## 5. People controls (6.1 to 6.8)

| Ref | Control | Applicable | Justification | Status | Owner |
|---|---|---|---|---|---|
| 6.1 | Screening | Yes | Staff with access to client data; R8 | Implemented | HRD |
| 6.2 | Terms and conditions of employment | Yes | Security responsibilities written into contracts; R8 | Implemented | HRD |
| 6.3 | Information security awareness, education and training | Yes | R1 | Implemented | HRD |
| 6.4 | Disciplinary process | Yes | R8 | Implemented | HRD |
| 6.5 | Responsibilities after termination or change of employment | Yes | R4 | Implemented | HRD |
| 6.6 | Confidentiality or non-disclosure agreements | Yes | R8; client contracts | Implemented | HRD |
| 6.7 | Remote working | Yes | Hybrid working; R1, R6 | Implemented | HoIT |
| 6.8 | Information security event reporting | Yes | R1, R7 | Implemented | ISM |

## 6. Physical controls (7.1 to 7.14)

| Ref | Control | Applicable | Justification | Status | Owner |
|---|---|---|---|---|---|
| 7.1 | Physical security perimeters | Yes | Head office and comms room; production is cloud-hosted (see 5.23) | Implemented | FM |
| 7.2 | Physical entry | Yes | Badge and biometric entry to head office and comms room | Implemented | FM |
| 7.3 | Securing offices, rooms and facilities | Yes | Comms room locked; R6 | Implemented | FM |
| 7.4 | Physical security monitoring | Yes | CCTV and intruder alarm at head office | Implemented | FM |
| 7.5 | Protecting against physical and environmental threats | Yes | Fire and flood at head office; R2 (offsite backups) | Implemented | FM |
| 7.6 | Working in secure areas | Yes | Comms room access restrictions | Implemented | FM |
| 7.7 | Clear desk and clear screen | Yes | R6, R8 | Implemented | HRD |
| 7.8 | Equipment siting and protection | Yes | Head office equipment | Implemented | FM |
| 7.9 | Security of assets off-premises | Yes | Laptops used remotely; R6 | Implemented | HoIT |
| 7.10 | Storage media | Yes | Removable media restricted; R6, R8 | Implemented | HoIT |
| 7.11 | Supporting utilities | Yes | Head office power and connectivity; production resilience is covered by the cloud provider (5.23) | Implemented | FM |
| 7.12 | Cabling security | Yes | Office network cabling in locked comms cabinet | Implemented | FM |
| 7.13 | Equipment maintenance | Yes | Head office equipment | Implemented | HoIT |
| 7.14 | Secure disposal or re-use of equipment | Yes | R6, R7 | Implemented | HoIT |

## 7. Technological controls (8.1 to 8.34)

| Ref | Control | Applicable | Justification | Status | Owner |
|---|---|---|---|---|---|
| 8.1 | User endpoint devices | Yes | R6; device management | Implemented | HoIT |
| 8.2 | Privileged access rights | Yes | R8 | Implemented | HoIT |
| 8.3 | Information access restriction | Yes | R4, R8 | Implemented | HoIT |
| 8.4 | Access to source code | Yes | Platform code is core IP; R8 | Implemented | CIO |
| 8.5 | Secure authentication | Yes | R1; phishing-resistant MFA | Implemented | CIO |
| 8.6 | Capacity management | Yes | 99.9% availability objective | Implemented | HoIT |
| 8.7 | Protection against malware | Yes | R1, R2 | Implemented | HoIT |
| 8.8 | Management of technical vulnerabilities | Yes | R3; critical patches within 14 days | Implemented | HoIT |
| 8.9 | Configuration management | Yes | R3 | Implemented | HoIT |
| 8.10 | Information deletion | Yes | UK GDPR storage limitation; R7. Automated deletion for older archives not yet in place | In progress | DPO |
| 8.11 | Data masking | No | No production client data is used outside production and test data is synthetic (see 8.33); no risk in the register needs masking. Review if analytics use cases arise | Not applicable | - |
| 8.12 | Data leakage prevention | Yes | R7 | Implemented | DPO |
| 8.13 | Information backup | Yes | R2; immutable offline copies tested quarterly | Implemented | HoIT |
| 8.14 | Redundancy of information processing facilities | Yes | 99.9% availability objective | Implemented | CIO |
| 8.15 | Logging | Yes | R8 | Implemented | HoIT |
| 8.16 | Monitoring activities | Yes | R1, R8 | Implemented | ISM |
| 8.17 | Clock synchronization | Yes | Reliable log timestamps for investigations | Implemented | HoIT |
| 8.18 | Use of privileged utility programs | Yes | R8 | Implemented | HoIT |
| 8.19 | Installation of software on operational systems | Yes | R3 | Implemented | HoIT |
| 8.20 | Networks security | Yes | R3 | Implemented | HoIT |
| 8.21 | Security of network services | Yes | R3, R5 | Implemented | HoIT |
| 8.22 | Segregation of networks | Yes | Production separated from corporate network; R3, R8 | Implemented | HoIT |
| 8.23 | Web filtering | Yes | R1 | Implemented | HoIT |
| 8.24 | Use of cryptography | Yes | R6, R7; AES-256 at rest | Implemented | CIO |
| 8.25 | Secure development life cycle | Yes | R3 | In progress | CIO |
| 8.26 | Application security requirements | Yes | R3, R7 | In progress | CIO |
| 8.27 | Secure system architecture and engineering principles | Yes | R3 | Implemented | CIO |
| 8.28 | Secure coding | Yes | R3; code review in place, static analysis being rolled out | In progress | CIO |
| 8.29 | Security testing in development and acceptance | Yes | R3 | In progress | CIO |
| 8.30 | Outsourced development | No | All platform development is carried out in-house; no outsourced development. Review if this changes | Not applicable | - |
| 8.31 | Separation of development, test and production environments | Yes | R3, R7 | Implemented | CIO |
| 8.32 | Change management | Yes | R3 | Implemented | CIO |
| 8.33 | Test information | Yes | R7; synthetic data only | Implemented | CIO |
| 8.34 | Protection of information systems during audit testing | Yes | Scans and audits touch production systems | Implemented | ISM |

## 8. Exclusions

| Ref | Control | Reason |
|---|---|---|
| 8.11 | Data masking | No production client data is used outside production; test data is synthetic. |
| 8.30 | Outsourced development | All platform development is in-house. |

Both exclusions will be revisited at the annual review or on any change that affects them.

## 9. Approval

| Role | Name | Date |
|---|---|---|
| Information Security Manager | A. Patel (fictional) | 26 Jan 2026 (v1.0); 1 Oct 2026 (v1.1) |
| Chair, Risk Committee | R. Okafor (fictional) | 2 Feb 2026 (v1.0); 8 Oct 2026 (v1.1) |
