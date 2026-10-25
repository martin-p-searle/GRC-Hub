# SecureCorp Risk Assessment Report (Fictional)

| | |
|---|---|
| **Document owner** | Information Security Manager |
| **Version** | 1.1 |
| **First approved** | 19 January 2026 (v1.0) |
| **Last reviewed** | 8 October 2026 |
| **Approved by** | Risk Committee (CEO, CFO, CIO, ISM) |
| **Next review** | January 2027 or on significant change |
| **Standard** | ISO/IEC 27001:2022, clauses 6.1.2 and 6.1.3 |

*SecureCorp is a fictional organisation created for training purposes.*

Related documents: [Statement of Applicability](statement-of-applicability.md) | [Security Controls](../security-measures/security-controls.md)

## 1. Scope

The ISMS covers SecureCorp's managed document-processing service, delivered to UK and EU business clients from its head office and a cloud-hosted production environment. It includes about 250 staff, their corporate laptops, the production platform, and the corporate network and SaaS tools.

**Out of scope:** the marketing website (hosted and managed by a third party; no client data) and staff personal devices (BYOD is not permitted).

## 2. Methodology

Risks were identified through asset-based analysis, workshops with the IT, HR and Compliance teams, and a review of recent threat reporting (NCSC guidance and sector incident trends). The method is a likelihood × impact approach aligned with ISO 31000.

**Scoring:** Risk = Likelihood (1-5) × Impact (1-5).

| Score | Rating | Response |
|---|---|---|
| 15-25 | High | Treatment required; escalate to Risk Committee |
| 8-14 | Medium | Treat unless the owner formally accepts |
| 1-7 | Low | Accept and monitor |

**Impact scale (examples):** 5 = loss of client data or outage over 24 hours, regulatory action, loss of a major client; 3 = limited disruption, no client data exposed; 1 = negligible.

**Risk appetite:** the Risk Committee will accept residual risk of 8 or below. Anything higher needs written acceptance from the CEO.

## 3. Risk Register

| ID | Risk | Likelihood | Impact | Inherent | Treatment | Owner |
|---|---|---|---|---|---|---|
| R1 | Phishing leads to staff credential compromise | 4 | 4 | **16 High** | Mitigate | CIO |
| R2 | Ransomware encrypts file servers and backups | 3 | 5 | **15 High** | Mitigate and transfer | CIO |
| R3 | Unpatched vulnerability in an internet-facing system is exploited | 4 | 4 | **16 High** | Mitigate | Head of IT |
| R4 | Excess or stale access after role change or leaver | 3 | 4 | **12 Medium** | Mitigate | HR Director |
| R5 | Cloud or supplier breach exposes client data | 3 | 4 | **12 Medium** | Mitigate | Procurement Lead |
| R6 | Loss or theft of an unencrypted laptop | 3 | 3 | **9 Medium** | Mitigate | Head of IT |
| R7 | Personal data breach or GDPR non-compliance | 3 | 5 | **15 High** | Mitigate | DPO |
| R8 | Insider misuse or data exfiltration | 2 | 4 | **8 Medium** | Mitigate | ISM |

## 4. Risk Treatment and Residual Risk

Control numbers are from ISO/IEC 27001:2022 Annex A. Applicability and status for every control are in the [Statement of Applicability](statement-of-applicability.md).

| ID | Treatment decision | Annex A controls (2022) | Target date | Residual (L × I) |
|---|---|---|---|---|
| R1 | Phishing-resistant MFA for all staff; mandatory awareness training with quarterly simulations | 6.3, 5.17, 8.5, 8.7 | 31 Mar 2026 | 2 × 4 = **8** |
| R2 | Immutable offline backups tested quarterly; EDR on all endpoints. **Transfer:** cyber insurance renewed with a £2m limit | 8.13, 8.7, 5.30, 5.29 | 30 Apr 2026 | 2 × 4 = **8** |
| R3 | Critical patches within 14 days; monthly authenticated scans; baseline configurations | 8.8, 8.9, 8.20 | 28 Feb 2026 | 2 × 4 = **8** |
| R4 | Joiner-mover-leaver process tied to HR system; quarterly access reviews | 5.18, 6.5, 5.15, 5.16 | 31 Mar 2026 | 2 × 3 = **6** |
| R5 | Supplier due-diligence questionnaire; security clauses and breach notification in contracts; annual review of critical suppliers | 5.19, 5.20, 5.22, 5.23 | 30 Jun 2026 | 2 × 4 = **8** |
| R6 | Full-disk encryption enforced by device management; remote wipe | 8.1, 8.24, 7.9 | 31 Jan 2026 | 1 × 3 = **3** |
| R7 | Data classification scheme; DLP on email and endpoints; breach response runbook with 72-hour ICO notification process | 5.34, 5.12, 8.12, 5.26 | 30 Jun 2026 (5.26 extended to 31 Dec 2026, see section 8) | 2 × 4 = **8** (not yet reached) |
| R8 | Privileged access logging and monitoring; least-privilege roles; confidentiality clauses | 8.15, 8.16, 8.2, 6.6 | 30 Apr 2026 | 1 × 4 = **4** |

## 5. Risk Acceptance

All target residual risks are at or below the Risk Committee's appetite threshold of 8. Risks R1, R2, R3, R5 and R7 sit at the threshold and are reviewed quarterly. No risk requires CEO exception sign-off. Until control 5.26 is complete, R7 is treated as still above target (see section 8).

## 6. Legal and Regulatory Context

UK GDPR and the Data Protection Act 2018 were the main drivers for R7 (and for the impact scores on R1, R2 and R5). Client contracts require breach notification within 48 hours, which informed the treatment of R5.

## 7. Review and Approval

| Role | Name | Date |
|---|---|---|
| Information Security Manager | A. Patel (fictional) | 12 Jan 2026 (v1.0); 1 Oct 2026 (v1.1) |
| Chair, Risk Committee | R. Okafor (fictional) | 19 Jan 2026 (v1.0); 8 Oct 2026 (v1.1) |

## 8. Review Log

| Date | Version | Change |
|---|---|---|
| 12 Jan 2026 | 1.0 | First risk assessment completed; submitted to Risk Committee |
| 19 Jan 2026 | 1.0 | Approved; risk appetite set at 8 |
| 1 Oct 2026 | 1.1 | Quarterly review of treatment status; Annex A references checked against ISO/IEC 27001:2022 |
| 8 Oct 2026 | 1.1 | Target date for control 5.26 (incident response) extended from 30 Jun 2026 to 31 Dec 2026. Reason: the tabletop exercise was postponed after an audit-readiness workload peak. Interim measure: ISM on-call rota and the draft runbook are in use. R7 stays on the quarterly watch list |

