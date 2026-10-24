# GRC: PCI DSS Compliance for PaySafe Retail (Fictional)

> **Fictional portfolio project.** PaySafe Retail does not exist. No real client, cardholder data or payment system is involved, and this is not an official PCI DSS assessment. It was written to practise governance, risk and compliance (GRC) work.

This project simulates a Payment Card Industry Data Security Standard ([PCI DSS](https://www.pcisecuritystandards.org/)) compliance effort for a fictional online retailer. It shows how a GRC analyst would assess current practice against the standard, record gaps, and plan remediation.

## Table of Contents

- [Overview](#overview)
- [Scenario and scope](#scenario-and-scope)
- [Repository structure](#repository-structure)
- [How to read this project](#how-to-read-this-project)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [Author](#author)

## Overview

PaySafe Retail is a fictional e-commerce company that accepts credit and debit card payments. Taking card payments means it must meet PCI DSS to protect cardholder data.

This repository holds the documents that support that effort. The main piece is a gap assessment that compares the company's current practice with the PCI DSS v4.0.1 requirements.

## Scenario and scope

- **Company:** PaySafe Retail, an online retailer (fictional).
- **In scope:** the processes and systems involved in accepting card payments for the online store.
- **Standard used:** PCI DSS v4.0.1.
- **Assumptions:** all assumptions used for the assessment are recorded in the gap assessment itself, so a reader can see what the findings depend on.

## Repository structure

| Path | What it contains |
|---|---|
| [`03-Compliance/PCI-DSS-Gap-Assessment`](03-Compliance/PCI-DSS-Gap-Assessment/) | Gap assessment against PCI DSS v4.0.1: requirements, findings and recommended actions |

Add a row to this table each time you add a folder or document, so the list always matches what is in the repository.

## How to read this project

1. Read the scenario and scope above.
2. Open the [gap assessment](03-Compliance/PCI-DSS-Gap-Assessment/). For each requirement it records what the standard asks for, what the fictional company does today, any gap, and the recommended action.
3. Check that each finding states the evidence it rests on and why it was rated as it was.

## Limitations

- All people, systems and evidence are invented.
- The assessment is a learning exercise. It is not a Report on Compliance, an Attestation of Compliance or a substitute for a Qualified Security Assessor.
- Requirements change between versions of the standard. Check the current text on the PCI Security Standards Council website before relying on any detail.

## Contributing

This is a personal portfolio project. Feedback and corrections are welcome: please open an issue.

## Author

Martin Searle, working towards a career in GRC and information security.

## Repository Structure

