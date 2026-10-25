# Security Controls

## Overview

This document summarises the security controls selected for SecureCorp's ISO/IEC 27001:2022 Information Security Management System (ISMS). Controls come from Annex A (aligned with ISO/IEC 27002:2022) and are chosen from the [Risk Assessment Report](../compliance/risk-assessment-report.md). The full applicability decision for all 93 controls is in the [Statement of Applicability](../compliance/statement-of-applicability.md). These measures protect the confidentiality, integrity and availability of information assets.

*SecureCorp is a fictional organisation created for training purposes.*

## Control Selection Process

- **Risk Assessment**: Controls are selected to treat the risks in the [Risk Assessment Report](../compliance/risk-assessment-report.md) (R1 to R8).
- **Statement of Applicability (SoA)**: Applicability, justification and implementation status for each control are recorded in the [SoA](../compliance/statement-of-applicability.md).
- **Training**: Staff are trained on these controls through the [Security Awareness Training](../policies/security-awareness-training.md).

## Controls by Theme

### Organizational controls (Annex A.5)

- **5.1 Policies for information security**: Information security policy approved by management, published and reviewed annually.
  - *Implementation*: Policy documented and communicated to all staff. Related risks: all.
- **5.9 Inventory of information and other associated assets**: Maintain an inventory of information assets with named owners.
  - *Implementation*: Held in the [Asset Inventory](../compliance/asset-inventory.md). Related risks: R6.
- **5.12 Classification of information**: Classify information by sensitivity (public, internal, confidential, restricted).
  - *Implementation*: Classification scheme published; underpins DLP rules. Related risks: R7.
- **5.15 Access control**: Role-based access rules for information and systems.
  - *Implementation*: See the [Access Control Policy](../policies/access-control-policy.md). Related risks: R4, R8.
- **5.26 Response to information security incidents**: Respond to incidents in a timely, documented way.
  - *Implementation*: Procedures in the [Incident Response Plan](../policies/incident-response-plan.md). Related risks: R2, R7.
- **5.31 Legal, statutory, regulatory and contractual requirements**: Identify and meet applicable legal obligations (e.g., UK GDPR).
  - *Implementation*: Reviewed during risk assessment (see section 6 of the [Risk Assessment Report](../compliance/risk-assessment-report.md)). Related risks: R7.
- **5.35 Independent review of information security**: Review the ISMS independently at planned intervals.
  - *Implementation*: Internal audit scheduled for Months 10-12, see the [security-measures README](README.md).

### People controls (Annex A.6)

- **6.3 Information security awareness, education and training**: All staff receive regular training.
  - *Implementation*: Annual training plus quarterly phishing simulations, using the [Security Awareness Training](../policies/security-awareness-training.md). Related risks: R1.
- **6.5 Responsibilities after termination or change of employment**: Remove access promptly when people leave or change role.
  - *Implementation*: Joiner-mover-leaver process linked to the HR system. Related risks: R4.
- **6.8 Information security event reporting**: Staff report suspected incidents promptly.
  - *Implementation*: Reporting route defined in the [Incident Response Plan](../policies/incident-response-plan.md). Related risks: R1, R7.

### Technological controls (Annex A.8)

- **8.3 Information access restriction**: Restrict access to information according to the access control policy.
  - *Implementation*: Role-based access enforced on critical systems. Related risks: R4, R8.
- **8.5 Secure authentication**: Strong authentication, including MFA.
  - *Implementation*: Phishing-resistant MFA for all staff. Related risks: R1.
- **8.20 Networks security**: Restrict and monitor network access.
  - *Implementation*: Segmented networks; access rules documented in the [Access Control Policy](../policies/access-control-policy.md). Related risks: R3.

## Implementation Status

*Status as at 1 October 2026.*

| Control | Theme | Status | Owner | Related risks |
|---------|-------|--------|-------|---------------|
| 5.1 | Organizational | Implemented | Information Security Manager | All |
| 5.9 | Organizational | In progress | Head of IT | R6 |
| 5.15 | Organizational | Implemented | Head of IT | R4, R8 |
| 5.26 | Organizational | In progress | Information Security Manager | R2, R7 |
| 5.31 | Organizational | Implemented | DPO | R7 |
| 5.35 | Organizational | Planned (Months 10-12) | Information Security Manager | All |
| 6.3 | People | Implemented | HR Director | R1 |
| 6.5 | People | Implemented | HR Director | R4 |
| 8.3 | Technological | Implemented | Head of IT | R4, R8 |
| 8.5 | Technological | Implemented | CIO | R1 |

## Next Steps

- **Timeline**: Full implementation of controls by Month 9, as outlined in the [security-measures README](README.md).
- **Monitoring**: Review control effectiveness quarterly, alongside the risk register review.
- **Training**: Ensure all staff are trained on these controls using the [Security Awareness Training](../policies/security-awareness-training.md).

## Responsible Roles

- **Information Security Manager**: Oversees control implementation and monitoring.
- **Head of IT**: Implements technical controls (access control, asset inventory).
- **HR Director**: Owns training and employee-related controls.
- **DPO**: Owns legal and data protection obligations.
- **CIO**: Accountable for authentication and endpoint security.
