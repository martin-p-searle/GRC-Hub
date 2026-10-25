# UK / EU GDPR Gap Analysis

**Example Organisation (fictional)**

| | |
|---|---|
| **Document type** | Gap analysis and remediation plan |
| **Version** | 2.0 |
| **Assessment date** | 25 October 2026 |
| **Author** | Martin Searle |
| **Regimes assessed** | UK GDPR, Data Protection Act 2018, PECR, EU GDPR (for EU data subjects) |
| **Method** | Desktop review against regulatory requirements, with a risk-based rating of each gap |
| **Status** | Portfolio sample. The organisation, evidence and findings are simulated. Not legal advice. |

---

## 1. Executive summary

This assessment compares the current data protection practices of a fictional organisation with the requirements of the UK GDPR and EU GDPR. It identified **12 gaps**: **1 Critical, 6 High and 5 Medium**. No gap was rated Low.

The most urgent finding is the absence of a documented personal data breach process (G-04). The organisation cannot currently show that it could meet the 72-hour notification duty. The next priorities are lawful basis and consent, data subject access requests, records of processing, processor contracts, security of processing and DPIAs.

Most gaps stem from missing documentation and unclear ownership rather than missing technology. Closing the Critical and High gaps within 90 days is realistic with the owners named in section 6.

### Gaps by rating

| Rating | Count | Gap IDs |
|---|---|---|
| Critical | 1 | G-04 |
| High | 6 | G-01, G-03, G-05, G-06, G-07, G-08 |
| Medium | 5 | G-02, G-09, G-10, G-11, G-12 |

---

## 2. Scope

| Area | In scope |
|---|---|
| **Organisation** | All departments that process personal data of UK or EU residents |
| **Processes** | Collection, storage, use, sharing, retention and deletion of personal data |
| **Systems** | Customer database, CRM, marketing tools, HR systems, shared drives, third-party integrations |
| **Requirements** | Data protection principles (Art. 5), lawful basis (Art. 6-7), transparency (Art. 12-14), data subject rights (Art. 15-22), accountability and records (Art. 24, 30), data protection by design and DPIA (Art. 25, 35), processors (Art. 28), security (Art. 32), breach notification (Art. 33-34), DPO (Art. 37-39), international transfers (Chapter V) |

**Out of scope:** technical penetration testing, sector-specific regulation and a full review of every contract.

---

## 3. Method and rating criteria

Each requirement was assessed for its current state, the gap against the requirement, and the risk if the gap remains open.

**Risk score = Likelihood (1-5) x Impact (1-5)**

| Score | Rating | Remediation target |
|---|---|---|
| 20-25 | Critical | Within 30 days |
| 10-19 | High | Within 90 days |
| 5-9 | Medium | Within 180 days |
| 1-4 | Low | Next review cycle |

**Maturity scale:** 0 = None, 1 = Ad hoc, 2 = Defined but not implemented, 3 = Implemented, 4 = Monitored, 5 = Optimised.

**Target dates:** Critical by 24 Nov 2026, High by 23 Jan 2027, Medium by 23 Apr 2027.

---

## 4. Summary of gaps

| ID | Requirement | Gap | Maturity | L x I | Rating | Owner | Target |
|---|---|---|---|---|---|---|---|
| G-01 | Lawful basis and consent (Art. 5-7, PECR) | No documented lawful basis; consent not granular or easy to withdraw | 1 | 4 x 4 = 16 | High | DPO | 23 Jan 2027 |
| G-02 | Transparency (Art. 12-14) | Privacy notice incomplete and out of date | 2 | 3 x 3 = 9 | Medium | DPO | 23 Apr 2027 |
| G-03 | Data subject rights (Art. 12, 15-22) | No DSAR procedure or register; requests handled ad hoc | 1 | 4 x 4 = 16 | High | DPO | 23 Jan 2027 |
| G-04 | Breach notification (Art. 33-34) | No breach response plan or breach register | 1 | 4 x 5 = 20 | **Critical** | Security Lead | 24 Nov 2026 |
| G-05 | Records of processing (Art. 30) | No RoPA | 0 | 4 x 3 = 12 | High | DPO | 23 Jan 2027 |
| G-06 | Data protection by design and DPIA (Art. 25, 35) | No DPIA process; no minimisation or pseudonymisation | 1 | 3 x 4 = 12 | High | DPO / Head of IT | 23 Jan 2027 |
| G-07 | Security of processing (Art. 32) | Encryption and access controls inconsistent for personal data | 2 | 3 x 5 = 15 | High | Head of IT | 23 Jan 2027 |
| G-08 | Processors (Art. 28) | Some vendors have no DPA; no due diligence or audit process | 1 | 4 x 4 = 16 | High | Procurement | 23 Jan 2027 |
| G-09 | International transfers (Chapter V) | Transfers not mapped; safeguards unknown | 1 | 2 x 4 = 8 | Medium | DPO | 23 Apr 2027 |
| G-10 | Retention and minimisation (Art. 5(1)(c), (e)) | No retention schedule; CRM data kept indefinitely | 1 | 3 x 3 = 9 | Medium | Records Owner | 23 Apr 2027 |
| G-11 | Governance and DPO (Art. 24, 37-39) | No designated DPO or data protection lead; no reporting line to senior management | 1 | 3 x 3 = 9 | Medium | Managing Director | 23 Apr 2027 |
| G-12 | Training and awareness (Art. 24, 39(1)(b)) | No data protection training | 0 | 3 x 3 = 9 | Medium | HR | 23 Apr 2027 |

---

## 5. Detailed findings

### G-01 Lawful basis and consent (Art. 5(1)(a), 6, 7; PECR)

- **Requirement:** Every processing activity needs a documented lawful basis. Consent must be specific, informed, unambiguous and as easy to withdraw as to give. Electronic marketing must also meet PECR.
- **Current state (simulated):** Consent is collected for marketing emails using a pre-ticked box. Other uses, such as CRM retention, have no recorded justification.
- **Gap:** No lawful basis is documented per activity, and the consent mechanism does not meet the standard.
- **Risk:** L4 x I4 = 16 (High). Unlawful processing and unlawful marketing are both enforcement risks.
- **Action:** Record a lawful basis for each activity in the RoPA (G-05). Replace the pre-ticked box with an unticked, granular opt-in, add a one-click unsubscribe, and keep consent records. Document any legitimate interests assessments.
- **Owner / target:** DPO, 23 Jan 2027.

### G-02 Transparency (Art. 12-14)

- **Requirement:** Individuals must be told who is processing their data, why, on what basis, for how long, who receives it and what their rights are.
- **Current state (simulated):** A privacy notice exists on the website but omits retention periods, recipients and transfer safeguards, and has not been reviewed since launch.
- **Gap:** Notice does not contain the required information; there is no notice for employees.
- **Risk:** L3 x I3 = 9 (Medium).
- **Action:** Redraft the website privacy notice, create an employee privacy notice, and set an annual review.
- **Owner / target:** DPO, 23 Apr 2027.

### G-03 Data subject rights (Art. 12, 15-22)

- **Requirement:** Requests must be answered without undue delay and within **one month**, extendable by up to two further months for complex or numerous requests (Art. 12(3)). Staff must recognise requests made verbally or through any channel.
- **Current state (simulated):** No procedure and no register. Requests are handled ad hoc by whoever receives them. Staff are unaware of the deadline.
- **Gap:** No standard process for access requests or for the other rights (rectification, erasure, restriction, portability, objection).
- **Risk:** L4 x I4 = 16 (High). Late or incomplete responses are a common cause of ICO complaints.
- **Action:** Adopt the [DSAR Policy](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/data-subject-access-request-PWDCB4RBvOZSbnqG.pdf), set up a DSAR register, assign the DPO as owner, and brief all staff on how to recognise and forward a request on the same working day.
- **Owner / target:** DPO, 23 Jan 2027.

### G-04 Breach notification (Art. 33-34)

- **Requirement:** Notify the regulator (the ICO in the UK) **within 72 hours of becoming aware** of a breach, unless it is unlikely to result in a risk to individuals. Tell affected individuals without undue delay where the risk is high. Record **every** breach, including those not reported (Art. 33(5)).
- **Current state (simulated):** No documented process. Incident response is reactive and there is no breach register.
- **Gap:** The organisation could not currently show that it meets the 72-hour duty or the record-keeping duty.
- **Risk:** L4 x I5 = 20 (Critical). Late notification can attract a penalty in its own right, on top of the breach itself.
- **Action:** Adopt the [Personal Data Breach Response Plan](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/gdpr-personal-data-breach-response-plan-J49MyMcHwkTflq38.pdf), create a breach register, define a risk assessment template and escalation contacts, and run a tabletop exercise.
- **Owner / target:** Security Lead, 24 Nov 2026.

### G-05 Records of processing (Art. 30)

- **Requirement:** Maintain a record of processing activities covering purposes, categories of data and subjects, recipients, transfers, retention and security measures.
- **Current state (simulated):** No RoPA exists.
- **Gap:** The organisation cannot show what personal data it holds or why. This also blocks G-01, G-09 and G-10.
- **Risk:** L4 x I3 = 12 (High).
- **Action:** Build a RoPA using the [portfolio RoPA](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/iso-iec-27701-2019-records-of-processing-activities-ropa-M1DaCVmT1slIqdQp.pdf) as a model. Interview each department, then review the record every six months.
- **Owner / target:** DPO, 23 Jan 2027.

### G-06 Data protection by design and DPIA (Art. 25, 35)

- **Requirement:** Build data protection into systems and processes by default. Carry out a DPIA before any processing likely to result in a high risk.
- **Current state (simulated):** Customer data is collected without a minimisation review. No pseudonymisation is used. There is no DPIA screening step for new projects.
- **Gap:** No DPIA process and no design-stage privacy review.
- **Risk:** L3 x I4 = 12 (High).
- **Action:** Introduce a DPIA screening checklist for all new projects and systems. Use the [DPIA template](DPIA_Template.md) for high-risk processing. Review collection forms against a minimisation checklist and pseudonymise analytics data.
- **Owner / target:** DPO and Head of IT, 23 Jan 2027.

### G-07 Security of processing (Art. 32)

- **Requirement:** Apply technical and organisational measures appropriate to the risk, which can include encryption, access control, resilience and regular testing.
- **Current state (simulated):** Encryption is applied to some systems but not consistently. Access rights are not reviewed. Shared drives hold unrestricted personal data.
- **Gap:** Controls are inconsistent and not tested.
- **Risk:** L3 x I5 = 15 (High). This is the most likely route to a reportable breach.
- **Action:** Encrypt personal data at rest and in transit, introduce role-based access with quarterly access reviews, enforce MFA, and schedule annual security testing.
- **Owner / target:** Head of IT, 23 Jan 2027.

### G-08 Processors (Art. 28)

- **Requirement:** Use only processors that give sufficient guarantees, under a written contract containing the Art. 28(3) terms.
- **Current state (simulated):** Several vendors process personal data with no DPA. Nobody has checked the vendors' compliance status.
- **Gap:** Missing contracts, no due diligence, no audit process.
- **Risk:** L4 x I4 = 16 (High). The controller remains responsible for processor failures.
- **Action:** Build a vendor inventory, then put a DPA in place with every processor. Run due diligence using the [Article 28 assessment](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/iso-iec-27701-2019-third-party-processor-due-diligence-article-28-assessment-0tMvogD7JKXmY0ET.pdf) and add a DPA check to the procurement process.
- **Owner / target:** Procurement, 23 Jan 2027.

### G-09 International transfers (Chapter V)

- **Requirement:** Transfers outside the UK or EEA need an adequacy decision or appropriate safeguards (for example the UK IDTA or Addendum, or EU SCCs), supported by a transfer risk assessment where required.
- **Current state (simulated):** Several SaaS vendors are based outside the UK and EEA. Transfers are not mapped.
- **Gap:** No transfer inventory and no recorded safeguards.
- **Risk:** L2 x I4 = 8 (Medium).
- **Action:** Add transfers to the RoPA, confirm the mechanism for each vendor, and record the transfer risk assessments.
- **Owner / target:** DPO, 23 Apr 2027.

### G-10 Retention and minimisation (Art. 5(1)(c), (e))

- **Requirement:** Keep only the personal data needed, and no longer than needed.
- **Current state (simulated):** No retention schedule. CRM records are kept indefinitely.
- **Gap:** Excess data held, with no deletion process.
- **Risk:** L3 x I3 = 9 (Medium). Larger data stores increase the impact of any breach.
- **Action:** Create a retention schedule linked to the RoPA, apply it to the CRM, and run an annual deletion review.
- **Owner / target:** Records Owner, 23 Apr 2027.

### G-11 Governance and DPO (Art. 24, 37-39)

- **Requirement:** Controllers must be able to demonstrate compliance. Assess whether a DPO is mandatory and, if it is, appoint one with independence and a reporting line to the highest management level.
- **Current state (simulated):** No DPO or data protection lead. Nobody reports on data protection to senior management.
- **Gap:** No accountable owner and no management reporting.
- **Risk:** L3 x I3 = 9 (Medium).
- **Action:** Document the DPO assessment. Designate a DPO or data protection lead, and add a quarterly compliance report to the management agenda.
- **Owner / target:** Managing Director, 23 Apr 2027.

### G-12 Training and awareness (Art. 24, 39(1)(b))

- **Requirement:** Staff who handle personal data must understand their responsibilities.
- **Current state (simulated):** No data protection training at induction or afterwards.
- **Gap:** Staff cannot reliably recognise a DSAR or a breach.
- **Risk:** L3 x I3 = 9 (Medium).
- **Action:** Add data protection training to induction, require annual refreshers, and run targeted sessions on DSARs and breach reporting. Keep completion records.
- **Owner / target:** HR, 23 Apr 2027.

---

## 6. Remediation roadmap

| Phase | Deadline | Gaps | Key deliverables |
|---|---|---|---|
| 1 | 24 Nov 2026 | G-04 | Breach response plan, breach register, tabletop exercise |
| 2 | 23 Jan 2027 | G-01, G-03, G-05, G-06, G-07, G-08 | Consent redesign, DSAR procedure and register, RoPA, DPIA process, security controls, vendor DPAs |
| 3 | 23 Apr 2027 | G-02, G-09, G-10, G-11, G-12 | Privacy notices, transfer mapping, retention schedule, DPO decision, training programme |

## 7. Monitoring

- Review progress on every action at a monthly meeting chaired by the DPO.
- Report open Critical and High gaps to senior management each quarter.
- Re-run this assessment annually, or after a significant change in processing.
- Track closure evidence for every gap, such as the approved policy, the signed DPA or the training record.

## 8. Responsible roles

| Role | Responsibility |
|---|---|
| **Managing Director** | Sponsors the programme, decides on the DPO, receives quarterly reports |
| **DPO** | Owns lawful basis, DSARs, RoPA, DPIAs, notices and transfers |
| **Security Lead** | Owns breach response and incident handling |
| **Head of IT** | Owns security controls and technical measures |
| **Procurement** | Owns vendor contracts and due diligence |
| **HR** | Owns training and employee notices |
| **Records Owner** | Owns the retention schedule and deletion |

## 9. Related documents

- [DSAR Policy](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/data-subject-access-request-PWDCB4RBvOZSbnqG.pdf)
- [Personal Data Breach Response Plan](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/gdpr-personal-data-breach-response-plan-J49MyMcHwkTflq38.pdf)
- [Records of Processing Activities](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/iso-iec-27701-2019-records-of-processing-activities-ropa-M1DaCVmT1slIqdQp.pdf)
- [Third-Party Processor Due Diligence and Article 28 Assessment](https://assets.zyrosite.com/kXuD3r2Wsz3S8OVA/iso-iec-27701-2019-third-party-processor-due-diligence-article-28-assessment-0tMvogD7JKXmY0ET.pdf)
- [DPIA Template](DPIA_Template.md)

---

*Portfolio sample prepared in October 2026. The organisation, evidence and findings are fictional and for illustration only. This document is not legal advice.*
