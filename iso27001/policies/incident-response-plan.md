# SecureCorp Incident Response Plan (Fictional)

| | |
|---|---|
| **Document owner** | Information Security Manager |
| **Version** | 1.0 (plan); playbooks in Appendix A at v0.9 (draft) |
| **Approved** | 16 February 2026 |
| **Last reviewed** | 1 October 2026 |
| **Approved by** | Risk Committee |
| **Next review** | After the first tabletop exercise, then each January |
| **Controls supported** | ISO/IEC 27001:2022 Annex A 5.24, 5.25, 5.26, 5.27, 5.28, 5.29, 6.8 |

*SecureCorp is a fictional organisation created for training purposes.*

Related documents: [Risk Assessment Report](../compliance/risk-assessment-report.md) | [Statement of Applicability](../compliance/statement-of-applicability.md) | [Access Control Policy](access-control-policy.md) | [Security Awareness Training](security-awareness-training.md) | [Security Controls](../security-measures/security-controls.md)

## 1. Status

Control 5.26 (response to incidents) is **In progress** in the [Statement of Applicability](../compliance/statement-of-applicability.md). The plan is approved and in use. The playbooks in Appendix A are still drafts and have not yet been tested in an exercise. The first tabletop exercise, using a ransomware scenario, is scheduled for the **week of 7 December 2026**, inside the extended deadline of 31 December 2026 set by the Risk Committee (see section 8 of the risk assessment). Until then, the on-call rota and these draft playbooks are the interim measure.

## 2. Purpose and Scope

This plan describes how SecureCorp prepares for, detects, responds to and learns from information security incidents. It treats **R2 (ransomware)** and **R7 (personal data breach)** and supports R1, R3, R5, R6 and R8. It covers all systems and information in the ISMS scope, including the cloud production environment, and all staff, contractors and suppliers.

## 3. Definitions

| Term | Meaning |
|---|---|
| **Security event** | Something that might affect security, such as a suspicious email or an unusual log entry |
| **Security incident** | An event that has been assessed and confirmed as harming, or likely to harm, confidentiality, integrity or availability |
| **Personal data breach** | An incident that leads to accidental or unlawful destruction, loss, alteration, disclosure of or access to personal data |

## 4. Roles

| Role | Held by | Responsibility during an incident |
|---|---|---|
| Incident Manager | Information Security Manager | Leads the response, keeps the log, decides severity |
| Technical Lead | Head of IT | Containment, investigation, recovery |
| Executive Sponsor | CIO (CEO for Severity 1) | Authorises major decisions such as shutting down services |
| Data Protection Officer | DPO | Assesses personal data impact and advises on notifications |
| Communications Lead | CFO | Client, regulator and media messaging |
| People Lead | HR Director | Insider cases and staff welfare |
| Supplier Lead | Procurement Lead | Contact with suppliers and the cloud provider |

A deputy is named for each role on the on-call rota. The Incident Manager role passes to the CIO if the ISM is unavailable.

## 5. Severity Levels

Severity uses the impact scale in the [Risk Assessment Report](../compliance/risk-assessment-report.md).

| Level | Criteria | Examples | Response time | Who is told |
|---|---|---|---|---|
| **1 - Critical** | Impact 5: client data exposed, outage over 24 hours, or regulatory action likely | Ransomware on production; confirmed client data breach | Immediate, 24/7 | CEO, Risk Committee, DPO, insurer, affected clients |
| **2 - High** | Impact 4: serious disruption or contractual breach likely, limited data exposure | Credential compromise with access to client systems | Within 30 minutes | CIO, DPO, ISM |
| **3 - Medium** | Impact 3: limited disruption, no client data exposed | Malware contained on one laptop | Within 4 hours | Head of IT, ISM |
| **4 - Low** | Impact 1-2: negligible | Blocked phishing email | Next working day | ISM |

## 6. Response Process

### 6.1 Report (control 6.8)
Anyone who suspects an incident reports it at once to the security mailbox (security@securecorp.example) or the on-call number. No one is blamed for reporting in good faith. Reports are logged in the incident register.

### 6.2 Assess (control 5.25)
The Incident Manager decides within the response time whether the event is an incident, sets the severity, opens an incident record and starts the log. Any suspected personal data breach is passed to the DPO straight away.

### 6.3 Contain
Limit the spread: isolate affected devices, disable compromised accounts, block malicious addresses, and where needed take affected services offline with the Executive Sponsor's approval. Containment steps are recorded with times.

### 6.4 Preserve evidence (control 5.28)
Before systems are changed or rebuilt, capture logs, take disk images where needed, and record who handled what and when (chain of custody). Evidence is kept in a restricted location.

### 6.5 Eradicate and recover (controls 5.29, 8.13)
Remove the cause, rebuild from known-good images, restore data from the immutable offline backups, reset credentials, and monitor closely after service returns. Recovery priority follows the [Asset Inventory](../compliance/asset-inventory.md) criticality ratings.

### 6.6 Review (control 5.27)
A post-incident review is held within 10 working days for every Severity 1 to 3 incident. It records root cause, what worked, what did not, and actions with owners and dates. Lessons are added to [Security Awareness Training](security-awareness-training.md) and to the risk register where they change a score.

## 7. Notification Obligations

SecureCorp acts in two capacities, and the duties differ.

| Situation | Duty | Deadline |
|---|---|---|
| **Client documents (SecureCorp is the processor)** | Tell the affected client | Without undue delay and within **48 hours** of becoming aware, as set by client contracts. The client, as controller, decides about telling the ICO and individuals |
| **SecureCorp's own personal data, such as staff records (SecureCorp is the controller)** | Report to the ICO if there is a risk to individuals | Within **72 hours** of becoming aware (UK GDPR Article 33) |
| **High risk to individuals (controller cases)** | Tell the individuals | Without undue delay (UK GDPR Article 34) |
| **Cyber insurance (R2 transfer)** | Notify the insurer | Within 24 hours of a suspected ransomware or major incident, as required by the policy |
| **Criminal activity** | Report to Action Fraud and, for serious incidents, the NCSC | As soon as practical |

The 48-hour client deadline is the tighter of the two, so it sets the clock for most incidents. Every breach, including those not reported, is recorded with the reasons for the decision.

## 8. Communications

- One voice: the Communications Lead approves all external statements.
- Staff are told what they need to do, not speculation.
- Messages are factual: what happened, what data is affected, what has been done and what clients should do.
- Contact details for the response team are held in the on-call rota, stored outside the main systems so they are available if the network is down.

## 9. Testing and Exercises

| Activity | Frequency | Status |
|---|---|---|
| Tabletop exercise (ransomware scenario) | Annually | First exercise scheduled week of 7 Dec 2026 |
| Backup restore test | Quarterly | Operating (control 8.13) |
| Phishing simulation | Quarterly | Operating (see [Security Awareness Training](security-awareness-training.md)) |
| Contact list check | Quarterly | Operating |

## 10. Measures

| Measure | Target | Year to 1 Oct 2026 |
|---|---|---|
| Events reported by staff | Tracked | 31 |
| Events confirmed as incidents | Tracked | 4 (1 at Severity 2, 3 at Severity 3) |
| Severity 1 incidents | 0 | 0 |
| Notifiable personal data breaches | 0 | 0 |
| Time to assess a Severity 2 event | Under 30 minutes | 24 minutes |
| Post-incident reviews completed within 10 working days | 100% | 100% (4 of 4) |

## 11. Review Log

| Date | Version | Change |
|---|---|---|
| 16 Feb 2026 | 1.0 | Plan approved; draft playbooks issued |
| 1 Oct 2026 | 1.0 | Reviewed; status and exercise date added; notification table clarified to separate processor and controller duties |

---

## Appendix A: Draft Playbooks (v0.9, to be tested in the first exercise)

### A1. Ransomware (R2)
1. Isolate affected machines from the network; do not power them off.
2. Disable affected accounts and block known indicators.
3. Declare Severity 1 and start the incident log.
4. Check that offline backups are intact before any restore.
5. Notify the insurer within 24 hours and clients within 48 hours if client data is affected.
6. Preserve logs and disk images, then rebuild from clean images and restore data.
7. Do not pay any ransom without Risk Committee and legal advice.
8. Hold the post-incident review within 10 working days.

### A2. Phishing and credential compromise (R1)
1. Disable the account and revoke active sessions and tokens.
2. Reset credentials and re-register the security key.
3. Search mailboxes for the same message and remove it.
4. Review sign-in and mailbox rules for the account for the past 30 days.
5. Check whether client data was accessed; escalate to Severity 2 or higher if so.

### A3. Personal data breach (R7)
1. Contain the breach and stop further loss.
2. Pass to the DPO immediately; record what data and how many people are affected.
3. Decide the capacity (processor or controller) and apply the deadlines in section 7.
4. Notify clients within 48 hours, or the ICO within 72 hours where SecureCorp is the controller.
5. Record the decision, including when no notification is made.

### A4. Lost or stolen laptop (R6)
1. Report to IT immediately.
2. Lock and wipe the device remotely through endpoint management.
3. Confirm disk encryption was active (control 8.24); if so, the incident is normally Severity 4.
4. Revoke the user's sessions and security key and issue replacements.
5. Report any theft to the police.

### A5. Supplier or cloud breach (R5)
1. Contact the supplier's security team and request a written incident report.
2. Identify the SecureCorp data and systems affected.
3. Rotate any shared credentials and review supplier access.
4. Apply the client notification deadline from the time SecureCorp becomes aware, not from the supplier's report.
5. Review the supplier relationship at the next quarterly review.
