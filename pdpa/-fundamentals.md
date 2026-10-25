# PDPA Fundamentals: DataSafe Solutions (Fictional)

| | |
|---|---|
| **Document** | Singapore PDPA fundamentals and how they apply to DataSafe Solutions |
| **Version / date** | 1.0, 25 October 2026 |
| **Prepared by** | Martin Searle (simulated role: GRC analyst) |
| **Organisation** | DataSafe Solutions, a fictional Singapore-based fintech company |
| **Status** | Portfolio simulation |

> **Fictional portfolio project.** DataSafe Solutions does not exist. Every system, number and person below is invented for practice. This document is a learning exercise, not legal advice. Check every legal point against the current PDPA text and PDPC guidance (see [section 11](#11-limitations-and-references)) before relying on it.

[Back to GRC-Hub](https://github.com/martin-p-searle/GRC-Hub/blob/main/README.md)

## Contents

1. [Summary](#1-summary)
2. [The law at a glance](#2-the-law-at-a-glance)
3. [DataSafe Solutions: the scenario](#3-datasafe-solutions-the-scenario)
4. [The obligations applied to DataSafe](#4-the-obligations-applied-to-datasafe)
5. [Consent and its exceptions](#5-consent-and-its-exceptions)
6. [Data breach notification](#6-data-breach-notification)
7. [Roles and accountability](#7-roles-and-accountability)
8. [Penalties and enforcement](#8-penalties-and-enforcement)
9. [PDPA compared with GDPR](#9-pdpa-compared-with-gdpr)
10. [Mapping to ISO/IEC 27001:2022](#10-mapping-to-isoiec-270012022)
11. [Limitations and references](#11-limitations-and-references)

---

## 1. Summary

Singapore's Personal Data Protection Act 2012 (PDPA) sets the baseline rules for how organisations collect, use, disclose and look after personal data. This document explains the main obligations and applies each one to DataSafe Solutions, a fictional fintech that runs a digital wallet and merchant payment platform.

**Three points matter most for DataSafe:**

1. **Scale makes breach notification likely.** With about 900,000 consumer users, any incident that exposes the customer database would involve far more than 500 people, the usual threshold for a breach of "significant scale".
2. **Payment and identity data raises the stakes.** Financial data, identity numbers and verification photos need stronger protection than ordinary contact details.
3. **Suppliers carry a lot of the data.** Cloud, identity-verification and messaging providers all handle DataSafe's customer data, so DataSafe's duties continue through its supplier contracts.

The other documents in this project (the data protection policy, the implementation plan and the data protection measures) put these obligations into practice.

## 2. The law at a glance

| Item | Summary |
|---|---|
| **Law** | Personal Data Protection Act 2012, amended in 2020 (most amendments in force from 1 February 2021) |
| **Regulator** | Personal Data Protection Commission (PDPC) |
| **Who it covers** | Organisations that collect, use or disclose personal data in Singapore |
| **Personal data** | Data about an individual who can be identified from that data, or from that data combined with other information the organisation has or is likely to have access to |
| **Data intermediary** | An organisation that processes personal data on behalf of another organisation. Its own duties are limited to protection, retention and breach notification to the organisation it works for |
| **Do Not Call (DNC) rules** | Separate rules on sending marketing messages to Singapore telephone numbers |

Under the PDPC's framing there are eleven obligations. Ten are in force. The Data Portability Obligation was enacted in 2020, and its commencement should be checked on the PDPC website.

## 3. DataSafe Solutions: the scenario

**The company (fictional).** DataSafe Solutions is a Singapore-based fintech with about 150 staff. It offers a consumer wallet (about 900,000 users) and a payment service for about 12,000 merchants. As a payments business it also has to meet separate Monetary Authority of Singapore (MAS) requirements, including on technology risk and anti-money-laundering checks. This document covers the PDPA only.

**Personal data DataSafe handles:**

| Category | Examples | Sensitivity |
|---|---|---|
| Identity and verification | Name, date of birth, national identification number or passport number, address, verification photo | Very high |
| Contact | Mobile number, email address | Medium |
| Financial | Wallet balance, linked bank account, tokenised card details, transaction history | Very high |
| Device and technical | Device ID, IP address, location at login | Medium |
| Preferences | Marketing consent, notification settings | Low |
| Employee | HR records, payroll, access logs | High |

**A note on national identification numbers.** The PDPC has specific guidance limiting when organisations may collect these numbers. DataSafe's collection is justified by customer due diligence requirements for payment services, and it still has to collect only what is needed and protect it more strictly than other data.

## 4. The obligations applied to DataSafe

| Obligation (PDPA section) | What it requires in plain words | How DataSafe applies it |
|---|---|---|
| **Consent** (s13 to s17) | Get a person's consent before collecting, using or disclosing their data, unless deemed consent or an exception applies. Allow them to withdraw it | Clear sign-up consent screens, separate opt-in for marketing, a simple way to withdraw consent in the app, and a withdrawal process that takes effect within a reasonable time |
| **Purpose Limitation** (s18) | Only collect, use or disclose data for purposes a reasonable person would think appropriate and that the person has been told about | A register of purposes. Data collected for payments is not reused for unrelated marketing without a fresh basis |
| **Notification** (s20) | Tell people the purposes before or at the time of collection | A layered privacy notice at sign-up, and updates when purposes change |
| **Access and Correction** (s21, s22) | Give people their data and information on how it has been used in the past year, and correct errors, on request | A request form in the app, identity checks before release, and a reply within 30 days or a note of when the reply will be given |
| **Accuracy** (s23) | Make reasonable efforts to keep data accurate and complete, especially if it will be used to make decisions about the person or disclosed to others | Validation at entry, customer prompts to update details, and checks before data is shared with partners |
| **Protection** (s24) | Protect data with reasonable security arrangements | Encryption, access control, monitoring and supplier controls (see the data protection measures document) |
| **Retention Limitation** (s25) | Stop keeping data once it is no longer needed for legal or business purposes | A retention schedule by data type, with secure deletion. Some records, such as transaction records, are kept for the periods the law requires |
| **Transfer Limitation** (s26) | Only send data outside Singapore if the recipient gives comparable protection | Contracts with overseas suppliers that bind them to protect the data, plus a register of transfers |
| **Data Breach Notification** (s26A to s26E) | Assess suspected breaches, and tell the PDPC and affected people where required | A breach procedure with set deadlines (see [section 6](#6-data-breach-notification)) |
| **Accountability** (s11, s12) | Appoint someone responsible for compliance, set policies and practices, and publish contact details | A named Data Protection Officer, written policies, a complaints process and staff training |
| **Data Portability** (Part 6B) | On request, send a person's data to another organisation in a usable format | Enacted but commencement to be confirmed. DataSafe plans for it by building a standard export format |

### How the obligations follow the data

```mermaid
flowchart LR
  A[Collect] --> B[Use]
  B --> C[Disclose]
  C --> D[Store]
  D --> E[Transfer overseas]
  E --> F[Dispose]
```

| Stage | Main obligations |
|---|---|
| Collect | Consent, Purpose Limitation, Notification |
| Use | Purpose Limitation, Accuracy |
| Disclose | Consent, Purpose Limitation, Accuracy |
| Store | Protection, Retention Limitation, Access and Correction |
| Transfer overseas | Transfer Limitation, Protection |
| Dispose | Retention Limitation |

## 5. Consent and its exceptions

The PDPA is consent-based, but the 2020 amendments widened the ways consent can be given or avoided. DataSafe uses them as follows.

| Route | Meaning | DataSafe example |
|---|---|---|
| **Express consent** | The person actively agrees | Marketing messages, optional location sharing |
| **Deemed consent by conduct** | The person voluntarily gives data for a purpose that is obvious | Entering a mobile number to receive a one-time password |
| **Deemed consent by contractual necessity** | Data is needed to carry out a contract with the person | Processing a payment, and passing the details to the merchant's bank |
| **Deemed consent by notification** | The person is told about a new purpose and given a way to opt out, after DataSafe has assessed that the use will not harm them | Telling users about a new fraud-alert feature |
| **Legitimate interests exception** | Use without consent where the benefit outweighs any harm, after a documented assessment | Monitoring transactions to detect fraud |
| **Business improvement exception** | Use for improving products and operations in certain ways | Analysing how people use the app to fix problems |

Marketing to Singapore telephone numbers also needs a check against the Do Not Call register unless the person has given clear consent.

## 6. Data breach notification

A breach is notifiable if it is likely to cause **significant harm** to the people affected, or if it is of **significant scale** (the PDPC treats 500 or more individuals as significant scale).

| Step | Requirement | DataSafe process |
|---|---|---|
| 1. Contain | Act quickly to limit the damage | Incident team isolates affected systems |
| 2. Assess | Assess whether the breach is notifiable, in a reasonable and expeditious way. The PDPC expects this within 30 days of becoming aware | DPO leads and records the assessment, with timestamps |
| 3. Notify the PDPC | As soon as practicable, and no later than **3 calendar days** after assessing that the breach is notifiable | DPO files through the PDPC's notification channel |
| 4. Notify individuals | As soon as practicable, where the breach is likely to cause significant harm | Message in the app and by email, with advice on what to do |
| 5. Record and learn | Keep records of the breach and the decision | Breach register and post-incident review |

**Two points that often cause mistakes:**

- The three days run from the point the organisation **assesses the breach as notifiable**, not from the breach itself. Delaying the assessment to buy time is not an option, and the assessment must be prompt.
- Where DataSafe acts as a **data intermediary** (for example, processing data for a partner bank), it must tell that organisation without undue delay and leave the notification decision to them. The partner bank's own contract will usually set a much shorter deadline.

## 7. Roles and accountability

| Role | Responsibility |
|---|---|
| **Data Protection Officer (DPO)** | Required by the PDPA. Oversees compliance, handles complaints and access requests, leads breach assessments, reports to the board |
| **Chief Information Security Officer** | Owns security arrangements that meet the Protection Obligation |
| **Process owners** | Keep their part of the data inventory accurate and apply retention rules |
| **Procurement** | Makes sure supplier contracts include data protection terms |
| **All staff** | Complete training and report suspected incidents immediately |

Business contact information for the DPO is published so that customers can reach them.

## 8. Penalties and enforcement

| Item | Detail |
|---|---|
| **Financial penalties** | Up to 10% of annual turnover in Singapore for organisations with turnover above S$10 million, and up to S$1 million in other cases (for contraventions from 1 October 2022) |
| **Other PDPC powers** | Directions to stop, correct or destroy data, accept undertakings, and carry out investigations |
| **Private action** | Individuals harmed by a breach may also be able to bring a civil claim |
| **Factors that affect outcomes** | Quick containment, prompt notification, cooperation with the PDPC and good prior governance weigh in an organisation's favour |

For DataSafe the 10% cap is the relevant figure, which is why the breach process and board reporting are set up as they are.

## 9. PDPA compared with GDPR

| Topic | Singapore PDPA | EU/UK GDPR |
|---|---|---|
| Legal basis | Consent, with deemed consent and defined exceptions | Six lawful bases, consent is only one |
| Breach notification | PDPC within 3 calendar days of assessing a notifiable breach | Supervisory authority within 72 hours of becoming aware, where there is a risk to individuals |
| DPO | Someone must be appointed for compliance | Required in defined cases |
| Individual rights | Access and correction (portability enacted but pending) | Access, rectification, erasure, restriction, portability and objection |
| Maximum penalty | 10% of Singapore turnover or S$1 million | 4% of worldwide turnover or EUR 20 million (UK equivalent in sterling) |
| Overseas transfers | Recipient must give comparable protection | Adequacy decisions or approved safeguards |

A fintech serving customers in both places would need to meet whichever rule is stricter on each point. The GDPR part of this portfolio is in the [gdpr folder](../gdpr/).

## 10. Mapping to ISO/IEC 27001:2022

This table shows how a certified information security management system supports each PDPA obligation. Control numbers are from Annex A of the 2022 edition. The full ISO 27001 project is in the [iso27001 folder](../iso27001/).

| PDPA obligation | Supporting Annex A controls |
|---|---|
| Consent, Notification, Purpose Limitation | 5.34 Privacy and protection of PII, 5.31 Legal, statutory, regulatory and contractual requirements |
| Access and Correction, Accuracy | 5.34 Privacy and protection of PII, 5.12 Classification of information |
| Protection | 5.15 Access control, 8.5 Secure authentication, 8.12 Data leakage prevention, 8.15 Logging, 8.24 Use of cryptography |
| Retention Limitation | 5.33 Protection of records, 8.10 Information deletion |
| Transfer Limitation | 5.14 Information transfer, 5.19 to 5.23 Supplier and cloud service controls |
| Data Breach Notification | 5.24 to 5.28 Incident management, 6.8 Information security event reporting |
| Accountability | 5.1 Policies, 5.2 Roles and responsibilities, 5.35 Independent review, 6.3 Awareness and training |

## 11. Limitations and references

- All numbers, systems and people are invented.
- Legal points were written from the author's understanding of the PDPA and public PDPC guidance. They have not been reviewed by a lawyer. Check section numbers, thresholds and deadlines against the current text.
- The status of the Data Portability Obligation and the detail of the PDPC's advisory guidelines can change, so confirm both on the PDPC website.
- MAS requirements for payment service providers are outside the scope of this document.

**References**

- [Personal Data Protection Commission Singapore](https://www.pdpc.gov.sg/) for the PDPA overview, the data protection obligations, advisory guidelines and breach notification guidance.
- [Personal Data Protection Act 2012 on Singapore Statutes Online](https://sso.agc.gov.sg/Act/PDPA2012) for the legislation.

[Back to GRC-Hub](https://github.com/martin-p-searle/GRC-Hub/blob/main/README.md)

Last updated: October 2026
