# SecureCorp Security Awareness Training (Fictional)

| | |
|---|---|
| **Document owner** | HR Director |
| **Content owner** | Information Security Manager |
| **Version** | 1.1 |
| **First approved** | 9 February 2026 (v1.0) |
| **Last reviewed** | 1 October 2026 |
| **Approved by** | Risk Committee |
| **Next review** | January 2027, or after any significant incident |
| **Controls supported** | ISO/IEC 27001:2022 Annex A 6.3, 6.8, 5.10; clause 7.3 |

*SecureCorp is a fictional organisation created for training purposes.*

Related documents: [Risk Assessment Report](../compliance/risk-assessment-report.md) | [Statement of Applicability](../compliance/statement-of-applicability.md) | [Access Control Policy](access-control-policy.md) | [Incident Response Plan](incident-response-plan.md) | [Security Controls](../security-measures/security-controls.md)

## 1. Purpose

This document sets out how SecureCorp makes sure every person with access to its systems understands their security responsibilities. Awareness is the main treatment for **R1 (phishing leading to credential compromise)**, which has the highest inherent score in the [Risk Assessment Report](../compliance/risk-assessment-report.md), and it supports R4, R6, R7 and R8.

It applies to all staff, contractors and temporary workers.

## 2. Programme Structure

| Element | Frequency | Audience | Owner |
|---|---|---|---|
| Induction module | Within 5 working days of joining, before access to client data | New starters and contractors | HR Director |
| Annual awareness training | Once a year, plus refresher when policies change | All staff | ISM |
| Phishing simulations | Quarterly | All staff | ISM |
| Role-based training | Annually, or on role change | Developers, IT administrators, HR, Finance, managers | ISM and role leads |
| Incident awareness briefing | After any significant incident | Affected teams | ISM |

## 3. Annual Curriculum

| Module | Content | Risks | Duration |
|---|---|---|---|
| 1. Phishing and social engineering | Spotting phishing, vishing and smishing; how to report | R1 | 20 minutes |
| 2. Authentication | Security keys, password manager, why shared accounts are not allowed | R1, R4 | 15 minutes |
| 3. Handling information | Classification levels, labelling, secure sharing, clear desk and screen | R7 | 20 minutes |
| 4. Working away from the office | Public Wi-Fi, device security, protecting client data at home | R6 | 15 minutes |
| 5. Reporting events | What to report, how, and why speed matters; no blame for reporting | R1, R7 | 10 minutes |
| 6. UK GDPR essentials | Personal data, client data as processor, breach recognition | R7 | 20 minutes |
| 7. Insider risk and acceptable use | Acceptable use, confidentiality and consequences of misuse | R8 | 15 minutes |
| 8. Suppliers and third parties | Sharing information with suppliers, verifying requests | R5 | 10 minutes |

Total: about two hours a year.

## 4. Role-Based Training

| Role | Additional topics |
|---|---|
| Developers | Secure coding, code review, secrets handling, dependency risks (supports controls 8.25 and 8.28) |
| IT administrators | Privileged access, change control, logging, incident handling |
| HR | Joiner-mover-leaver process, handling HR records, screening |
| Finance | Payment fraud, invoice redirection, business email compromise |
| Managers | Reviewing team access, spotting insider-risk indicators, handling reports from staff |

## 5. Phishing Simulations

- **Frequency:** one simulation each quarter, using realistic scenarios that vary in difficulty (for example fake invoices, shared-document requests and urgent messages from executives).
- **Purpose:** learning, not punishment. People who click receive immediate guidance and a short follow-up module.
- **Repeat clickers:** two or more clicks in four quarters leads to one-to-one coaching from the ISM, not discipline. Disciplinary action is reserved for deliberate or repeated breaches of policy, in line with control 6.4.
- **Reporting:** staff report suspicious messages using the report button in the email client. A reported simulation counts as a success.

## 6. Completion Rules

| Day after assignment | Action |
|---|---|
| 0 | Training assigned automatically through the learning platform |
| 30 | Reminder; line manager notified if not complete |
| 45 | HR Director notified |
| 60 | Access to client data suspended until the training is completed |

Pass mark for each assessment is 80%. Staff can retake as often as needed.

## 7. Measuring Effectiveness

| Measure | Target | Q1 2026 | Q2 2026 | Q3 2026 |
|---|---|---|---|---|
| Annual training completion (rolling) | 95% within 30 days | - | - | 96% |
| Phishing simulation click rate | Below 5% | 14% | 9% | 6% |
| Phishing simulation report rate | Above 60% | 22% | 41% | 58% |
| Median time to report a real suspicious email | Under 15 minutes | 40 minutes | 22 minutes | 12 minutes |

**Reading the results:** click rate has fallen each quarter but is still just above target, and the report rate is just below. The Q4 simulation will use a more targeted scenario for finance staff. These measures feed the quarterly review of R1, which is held at the residual score of 8 until click rate is consistently below target.

## 8. Records and Review

- Training and simulation records are held in the learning platform and kept for three years.
- Results are reported to the Risk Committee each quarter and used as evidence for control 6.3.
- Content is reviewed every year and updated after significant incidents, threat reports and policy changes. Lessons from incidents are included in the next simulation (control 5.27).

## 9. Review Log

| Date | Version | Change |
|---|---|---|
| 9 Feb 2026 | 1.0 | Programme approved; first annual cycle and quarterly simulations started |
| 1 Oct 2026 | 1.1 | Q3 results added; finance-targeted scenario planned for Q4 |
