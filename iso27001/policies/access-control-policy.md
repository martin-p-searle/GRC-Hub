# SecureCorp Access Control Policy (Fictional)

| | |
|---|---|
| **Document owner** | Head of IT |
| **Version** | 1.1 |
| **First approved** | 9 February 2026 (v1.0) |
| **Last reviewed** | 1 October 2026 |
| **Approved by** | Risk Committee |
| **Next review** | January 2027, or on significant change |
| **Controls supported** | ISO/IEC 27001:2022 Annex A 5.15, 5.16, 5.17, 5.18, 6.5, 8.2, 8.3, 8.4, 8.5, 8.20, 8.22 |

*SecureCorp is a fictional organisation created for training purposes.*

Related documents: [Risk Assessment Report](../compliance/risk-assessment-report.md) | [Statement of Applicability](../compliance/statement-of-applicability.md) | [Asset Inventory](../compliance/asset-inventory.md) | [Security Awareness Training](security-awareness-training.md) | [Incident Response Plan](incident-response-plan.md) | [Security Controls](../security-measures/security-controls.md)

## 1. Purpose and Scope

This policy sets the rules for who may access SecureCorp's information and systems, and how that access is granted, used, reviewed and removed. It treats **R4 (excess or stale access)** and **R8 (insider misuse)** and supports R1 (credential compromise) in the [Risk Assessment Report](../compliance/risk-assessment-report.md).

It applies to all staff, contractors and suppliers with access to systems listed in the [Asset Inventory](../compliance/asset-inventory.md).

## 2. Principles

1. **Need to know:** people get access to the information they need for their role, and no more.
2. **Least privilege:** the lowest level of permission that lets the work be done.
3. **Default deny:** access is blocked unless it has been approved.
4. **Individual accountability:** every account belongs to one named person or service. Shared accounts are not allowed.
5. **Segregation of duties:** no one person can both request and approve their own access or complete a high-risk change alone (control 5.3).

## 3. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| Head of IT | Owns this policy; runs the technical processes for access |
| HR Director | Triggers joiner, mover and leaver processes; owns quarterly access reviews |
| Line managers | Request and justify access for their team; confirm it in reviews |
| System owners | Approve access to their systems and confirm user lists each quarter |
| Information Security Manager | Approves privileged access and exceptions; checks compliance |
| All users | Protect their credentials and report suspected misuse |

## 4. Requesting and Approving Access

- Access is requested through the IT ticketing system, giving the business reason.
- The line manager and the system owner both approve. Privileged access also needs ISM approval.
- Access is set up within 2 working days of approval and recorded in the ticket.
- Access to client documents is only given once the person has completed the induction module in [Security Awareness Training](security-awareness-training.md).

## 5. Joiners, Movers and Leavers

| Event | Requirement |
|---|---|
| **Joiner** | Access is based on a standard role profile and set up before the start date. Contractors have an end date, up to a maximum of 6 months, renewable on approval |
| **Mover** | Access from the previous role is removed within 5 working days of the change; new access follows the request process in section 4 |
| **Leaver** | HR notifies IT as soon as notice is given. Accounts are disabled by the end of the last working day, or immediately for dismissals. Laptop, phone and security key are returned (control 5.11). Accounts are deleted after 30 days once any data has been transferred |

## 6. Role-Based Access

| Role | Standard access | Client documents | Privileged access |
|---|---|---|---|
| Service delivery | Platform front end, ticketing, collaboration | Assigned clients only | No |
| Support engineer | Platform support tools, logs for assigned clients | Assigned clients, time-limited | No |
| Developer | Code repository, test environments | No (synthetic data only, control 8.33) | No production admin |
| IT administrator | Infrastructure consoles | Not by default | Yes, separate admin account |
| HR | HR system | No | No |
| Finance | Finance system, payroll provider portal | No | No |
| Security analyst | SIEM, endpoint management | Read-only logs | Yes, read-only plus incident access |

Access to source code (control 8.4) is limited to the engineering team. Changes to protected branches need peer review.

## 7. Authentication

- **Multi-factor authentication:** phishing-resistant MFA, using FIDO2 security keys, is required for all staff on all corporate and cloud systems (control 8.5).
- **Passwords:** a minimum of 14 characters, or a passphrase of three random words, checked against known breached passwords. Passwords are not changed on a schedule but are changed immediately if compromise is suspected. Staff use the approved password manager.
- **Lockout and sessions:** accounts lock after 10 failed attempts; devices lock after 15 minutes idle.
- **Service accounts:** each has a named owner, cannot be used to log in interactively, stores secrets in a vault and has secrets rotated at least every 90 days.

## 8. Privileged Access

- Administrators use a separate admin account, never their daily account.
- Privilege is raised only when needed, with approval, for a maximum of 8 hours.
- All privileged actions are logged to the SIEM and reviewed monthly by the ISM.
- Two break-glass accounts exist for emergencies. Credentials are sealed, any use raises an alert, and the accounts are tested each quarter.
- Privileged utility programs are limited to named administrators (control 8.18).

## 9. Access Reviews

| Review | Frequency | Done by | Evidence |
|---|---|---|---|
| User access to all systems | Quarterly | System owners and line managers | Signed review record in the ticketing system |
| Privileged accounts | Monthly | ISM | Review log |
| Client document repositories | Quarterly | CIO and DPO | Review record |
| Supplier and contractor accounts | Quarterly | Procurement Lead | Review record |

Access flagged as unnecessary is removed within 5 working days. Review results are reported to the Risk Committee in the quarterly R4 update.

## 10. Network Access

- Production is separated from the corporate network (control 8.22). Administration of production is only from managed devices through a controlled access point.
- Remote access uses the approved VPN or zero-trust gateway and a managed device. Personal devices are not allowed (BYOD is out of scope and prohibited).
- Guest Wi-Fi is isolated from corporate and production networks.

## 11. Third-Party Access

Suppliers get named accounts, limited to the systems and time period agreed. Each account has a SecureCorp sponsor and is covered by security terms in the supplier agreement (control 5.20). Access is logged and reviewed quarterly.

## 12. Logging and Monitoring

Authentication events, privilege use and access changes are logged to the SIEM and kept for 12 months. Alerts are raised for repeated failed logins, use of break-glass accounts, new privileged accounts and access from unusual locations. Suspected misuse is handled under the [Incident Response Plan](incident-response-plan.md).

## 13. Exceptions

Exceptions must be requested in writing, risk-assessed, and approved by both the ISM and the system owner. They last no more than 90 days and are listed in the quarterly report.

## 14. Compliance

Breaches of this policy may lead to disciplinary action (control 6.4). Compliance is checked through the access reviews, SIEM alerts and the internal audit planned for Months 10-12 (control 5.35).

## 15. Review Log

| Date | Version | Change |
|---|---|---|
| 9 Feb 2026 | 1.0 | Policy approved; security keys and role profiles introduced |
| 1 Oct 2026 | 1.1 | Annual review of role table; break-glass testing frequency set to quarterly |
