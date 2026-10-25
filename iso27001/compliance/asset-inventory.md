# SecureCorp Asset Inventory (Fictional)

| | |
|---|---|
| **Document owner** | Head of IT |
| **Version** | 1.1 (status review) |
| **First approved** | 2 February 2026 (v1.0) |
| **Status as at** | 1 October 2026 |
| **Approved by** | Information Security Manager |
| **Next review** | Quarterly; full reconciliation each January |
| **Controls supported** | ISO/IEC 27001:2022 Annex A 5.9, 5.10, 5.11, 5.12, 5.13 |

*SecureCorp is a fictional organisation created for training purposes.*

Related documents: [Risk Assessment Report](risk-assessment-report.md) | [Statement of Applicability](statement-of-applicability.md) | [Access Control Policy](../policies/access-control-policy.md) | [Security Controls](../security-measures/security-controls.md)

## 1. Purpose and Status

This inventory lists the information and associated assets within the scope of SecureCorp's ISMS, who owns each one, how sensitive it is and which risks it relates to. It is the starting point for the [Risk Assessment Report](risk-assessment-report.md): a risk cannot be assessed on an asset nobody has recorded.

**Control 5.9 is In progress** in the [Statement of Applicability](statement-of-applicability.md). Hardware, applications and information assets are recorded and reconciled. Cloud resources are about 78% reconciled to tagged resources, and discovery of unapproved SaaS use is still under way (see section 6). Target for completion: **30 November 2026**.

## 2. Classification Scheme

| Level | Description | Examples | Minimum handling |
|---|---|---|---|
| **Restricted** | Client documents and personal data; damage would be severe and likely notifiable | Client documents, HR records, backups | Encrypted at rest and in transit; named-user access only; no copies to removable media; DLP enforced |
| **Confidential** | Business-sensitive information not for general release | Source code, contracts, financial records | Encrypted in transit; access by role; share only through approved tools |
| **Internal** | Information for staff use | Policies, internal procedures | Share within SecureCorp; not published externally |
| **Public** | Approved for release | Marketing material | No restriction after approval |

## 3. Criticality Scale

Criticality is the highest of the confidentiality, integrity and availability ratings, using the impact scale in the risk assessment.

| Criticality | Meaning | Matches impact score |
|---|---|---|
| **Critical** | Compromise or loss would mean client data exposure, an outage over 24 hours or regulatory action | 5 |
| **High** | Serious disruption or a contractual breach, limited exposure | 4 |
| **Medium** | Limited disruption, no client data exposed | 3 |
| **Low** | Negligible effect | 1-2 |

## 4. Asset Register

**Owner** is the role accountable for the asset. **Status:** Recorded means the entry is complete and reconciled; Pending means a field (usually the owner or location) still needs confirming.

### 4.1 Information assets

| ID | Asset | Owner | Classification | Criticality | Location | Risks | Status |
|---|---|---|---|---|---|---|---|
| INF-01 | Client documents (in processing and stored) | CIO | Restricted | Critical | Cloud production | R2, R5, R7, R8 | Recorded |
| INF-02 | Client contracts and data processing agreements | CFO | Confidential | High | Document management system | R5, R7 | Recorded |
| INF-03 | Staff HR records | HR Director | Restricted | High | HR system (SaaS) | R4, R7 | Recorded |
| INF-04 | Platform source code and build pipeline | CIO | Confidential | Critical | Code repository (SaaS) | R3, R8 | Recorded |
| INF-05 | Financial records | CFO | Confidential | High | Finance system (SaaS) | R8 | Recorded |
| INF-06 | Backup data (immutable offline copies) | Head of IT | Restricted | Critical | Offsite backup vault | R2 | Recorded |

### 4.2 Applications and cloud services

| ID | Asset | Owner | Classification | Criticality | Location | Risks | Status |
|---|---|---|---|---|---|---|---|
| APP-01 | Document-processing platform (production) | CIO | Restricted | Critical | Cloud production | R3, R5 | Recorded |
| APP-02 | Client and metadata database | CIO | Restricted | Critical | Cloud production | R3, R5, R7 | Recorded |
| APP-03 | Identity provider and MFA service | CIO | Confidential | Critical | SaaS | R1, R4 | Recorded |
| APP-04 | Email and collaboration suite | Head of IT | Confidential | High | SaaS | R1, R7 | Recorded |
| APP-05 | HR system | HR Director | Restricted | High | SaaS | R4, R7 | Recorded |
| APP-06 | Endpoint management and EDR | Head of IT | Internal | High | SaaS | R2, R6 | Recorded |
| APP-07 | SIEM and log store | ISM | Confidential | High | Cloud | R8 | Recorded |
| APP-08 | Cloud storage buckets (non-production) | CIO | To be classified | To be rated | Cloud | R5, R7 | Pending |

### 4.3 Hardware and facilities

| ID | Asset | Owner | Classification | Criticality | Location | Risks | Status |
|---|---|---|---|---|---|---|---|
| HW-01 | Corporate laptops (265, including 15 spares) | Head of IT | Confidential | High | Staff, remote and head office | R1, R6 | Recorded |
| HW-02 | Corporate mobile phones (about 60) | Head of IT | Confidential | Medium | Staff | R6 | Recorded |
| HW-03 | FIDO2 security keys (about 300, including spares) | CIO | Confidential | High | Staff and secure store | R1 | Recorded |
| NET-01 | Head office network and comms room equipment | Head of IT | Confidential | High | Head office comms room | R3 | Recorded |
| NET-02 | Production network and firewalls | Head of IT | Confidential | Critical | Cloud production | R3 | Recorded |
| FAC-01 | Head office and comms room | Facilities Manager | Internal | High | Head office | R6 | Recorded |

### 4.4 Supplier services

| ID | Asset | Owner | Classification | Criticality | Location | Risks | Status |
|---|---|---|---|---|---|---|---|
| SUP-01 | Cloud hosting provider (production) | Procurement Lead | Restricted (data hosted) | Critical | Provider | R5 | Recorded |
| SUP-02 | Payroll provider | CFO | Restricted (data shared) | High | Provider | R5, R7 | Recorded |
| SUP-03 | Secure shredding and media disposal provider | Facilities Manager | Restricted (data handled) | Medium | Provider | R6, R7 | Pending (owner review) |

## 5. How the Inventory Is Kept Accurate

| Source | Used for | Check |
|---|---|---|
| Endpoint management console | Laptops and mobiles | Reconciled to the register monthly; unmanaged devices investigated within 5 working days |
| Cloud account tags and resource listings | Cloud and production assets | Every resource must carry an owner and classification tag; untagged resources reported weekly |
| HR system leaver and joiner feed | Asset assignment and return | Devices and security keys recovered on the last working day (control 5.11) |
| Procurement records | Suppliers and SaaS | New services cannot be purchased without an inventory entry |
| Quarterly access review | Owners confirm their assets | Owners confirm entries as part of the review in the [Access Control Policy](../policies/access-control-policy.md) |

Owners are responsible for classifying their assets, labelling documents (control 5.13) and following the handling rules in section 2. Labelling is applied to new documents first; older material is being relabelled as it is touched.

## 6. Known Gaps and Actions

| Gap | Risk | Action | Owner | Target |
|---|---|---|---|---|
| About 22% of cloud resources are not yet reconciled to tagged resources | R5, R7 | Complete tagging and add an alert for untagged resources | CIO | 30 Nov 2026 |
| Unapproved SaaS use not fully discovered | R5, R7 | Review single sign-on logs and expense data; add findings to the register | Head of IT | 30 Nov 2026 |
| Owner for APP-08 and SUP-03 not confirmed | R5, R7 | Assign and record owners; classify APP-08 | ISM | 15 Nov 2026 |
| Legacy documents not yet labelled | R7 | Relabel during the quarterly access review cycle | DPO | 31 Mar 2027 |

## 7. Review Log

| Date | Version | Change |
|---|---|---|
| 2 Feb 2026 | 1.0 | First inventory approved; information, application and hardware assets recorded |
| 1 Oct 2026 | 1.1 | Quarterly review; cloud reconciliation status and known gaps recorded; completion target set for 30 Nov 2026 |
