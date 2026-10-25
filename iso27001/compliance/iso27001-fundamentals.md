## Overview

This document outlines the ISO/IEC 27001:2022 fundamentals for SecureCorp, a fictional organization implementing an Information Security Management System (ISMS) to protect assets, including customer data, intellectual property, and IT systems. ISO27001 is the international standard for information security, providing a framework for managing risks and ensuring compliance. This supports SecureCorp’s compliance efforts as detailed in the [ISO27001 Project README](https://github.com/martin-p-searle/GRC-Hub/blob/main/iso27001/readme.md).

## ISO27001 Core Components

ISO27001:2022 consists of Clauses 4-10 (main requirements) and Annex A (controls). Below are the key components and SecureCorp’s approach:

### Clauses 4-10: ISMS Requirements

1. **Clause 4: Context of the Organization**
   * *Requirement*: Understand internal/external issues (including whether climate change is a relevant issue, per Amendment 1:2024), stakeholders, and ISMS scope.
   * *SecureCorp Approach*: Define ISMS scope covering IT systems, cloud services, and facilities. Conduct stakeholder analysis to identify compliance needs.
2. **Clause 5: Leadership**
   * *Requirement*: Leadership commitment, policy establishment, and role assignments.
   * *SecureCorp Approach*: Appoint an Information Security Manager and establish an ISMS policy approved by management.
3. **Clause 6: Planning**
   * *Requirement*: Address risks, set objectives, and plan ISMS implementation.
   * *SecureCorp Approach*: Perform risk assessments using a likelihood × impact method aligned with ISO31000, set security objectives (e.g., 99.9% uptime), and document risk treatment plans. See the [Risk Assessment Report](risk-assessment-report.md).
4. **Clause 7: Support**
   * *Requirement*: Ensure resources, competence, awareness, communication, and documentation.
   * *SecureCorp Approach*: Provide annual ISO27001 training with quarterly phishing simulations, allocate budget for security tools, and maintain documented procedures.
5. **Clause 8: Operation**
   * *Requirement*: Implement risk treatment plans and operational controls.
   * *SecureCorp Approach*: Deploy Annex A controls (e.g., encryption, access controls), perform a full risk assessment annually, and review the risk register quarterly.
6. **Clause 9: Performance Evaluation**
   * *Requirement*: Monitor, measure, analyze, and audit ISMS performance.
   * *SecureCorp Approach*: Conduct internal audits annually and management reviews twice a year to evaluate ISMS effectiveness.
7. **Clause 10: Improvement**
   * *Requirement*: Address nonconformities and improve ISMS.
   * *SecureCorp Approach*: Implement corrective actions for audit findings and update ISMS based on new threats.

### Annex A: Controls

Annex A provides 93 controls across four themes, tailored to SecureCorp’s needs. Applicability and implementation status for each control are recorded in the [Statement of Applicability](statement-of-applicability.md).

1. **Organizational Controls (37 controls)**
   * *Examples*: 5.1 (Policies for Information Security), 5.15 (Access Control).
   * *SecureCorp Approach*: Develop an Information Security Policy, review it annually, and define access rules by role.
2. **People Controls (8 controls)**
   * *Examples*: 6.1 (Screening), 6.7 (Remote Working).
   * *SecureCorp Approach*: Conduct background checks for employees and enforce secure remote work policies.
3. **Physical Controls (14 controls)**
   * *Examples*: 7.2 (Physical Entry), 7.3 (Securing Offices, Rooms and Facilities).
   * *SecureCorp Approach*: Install biometric access controls and secure server rooms.
4. **Technological Controls (34 controls)**
   * *Examples*: 8.2 (Privileged Access Rights), 8.24 (Use of Cryptography).
   * *SecureCorp Approach*: Implement role-based access control (RBAC) and AES-256 encryption.

## SecureCorp’s Compliance Strategy

* **Risk-Based Approach**: Use ISO31000 principles to identify and prioritize risks, applying Annex A controls as needed.
* **Documentation**: Maintain a Statement of Applicability (SoA) listing applicable controls and justifications.
* **Training**: Annual employee training on ISO27001 and security best practices, with quarterly phishing simulations.
* **Audits**: Annual internal audits and third-party certification audits to validate compliance.
* **Tools**: Deploy tools like firewalls, SIEM systems, and vulnerability scanners to support controls.

## Notes

* This is a fictional document for educational and portfolio purposes.
* Aligns with ISO/IEC 27001:2022 including Amendment 1:2024. Control numbering follows the 2022 edition.

[Back to ISO27001 Project](https://github.com/martin-p-searle/GRC-Hub/blob/main/iso27001/readme.md) | [Back to GRC-Hub](https://github.com/martin-p-searle/GRC-Hub/blob/main/README.md)

Last updated: October 2026
