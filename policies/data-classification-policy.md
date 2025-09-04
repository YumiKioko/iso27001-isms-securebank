# Data Classification and Handling Policy

**Policy Identifier:** POL-DC-005
**Version:** 1.0
**Effective Date:** 2023-10-27
**Approval Authority:** Chief Information Security Officer (CISO)
**Policy Owner:** Head of Data Governance

## 1.0 Purpose
To establish a framework for classifying and handling SecureBank Finance's data based on its sensitivity and value to the organization. This policy ensures that data receives an appropriate level of protection against unauthorized access, modification, or disclosure, in compliance with GDPR, PCI DSS, and other regulatory requirements.

## 2.0 Scope
This policy applies to all data created, processed, stored, or transmitted by SecureBank Finance, including data handled by third-party service providers. It applies to all employees, contractors, and agents.

## 3.0 Data Classification Levels
All information assets must be classified into one of the following categories:

### 3.1 Confidential (High Sensitivity)
*   **Definition:** Data whose unauthorized disclosure, alteration, or destruction could cause severe or catastrophic financial, reputational, and/or regulatory impact to SecureBank Finance or its customers.
*   **Examples:**
    *   Customer Personally Identifiable Information (PII): National ID numbers, passport numbers.
    *   Customer Financial Data: Full bank account numbers, transaction records, portfolio details, credit card numbers (PAN).
    *   Authentication Data: Passwords, private cryptographic keys, biometric data.
    *   Internal Sensitive Data: Encryption keys, merger & acquisition plans, audit findings.
*   **Handling Requirements:**
    *   Must be encrypted at rest and in transit using approved strong encryption (AES-256, TLS 1.2+).
    *   Access is restricted to authorized individuals on a strict need-to-know basis.
    *   Must not be stored on unencrypted mobile devices or non-approved cloud services.
    *   Requires secure deletion (e.g., wiping, cryptographic shredding) when no longer needed.

### 3.2 Internal (Medium Sensitivity)
*   **Definition:** Data intended for internal use only. Unauthorized disclosure could cause moderate risk to the organization.
*   **Examples:** Internal policies, non-sensitive operational reports, internal emails, organizational charts.
*   **Handling Requirements:**
    *   Should not be disclosed to the public.
    *   Access is restricted to employees and authorized contractors.
    *   Recommended to be encrypted in transit.

### 3.3 Public (Low Sensitivity)
*   **Definition:** Data that has been approved for public disclosure.
*   **Examples:** Marketing brochures, published press releases, public website content.
*   **Handling Requirements:** No specific protection controls required.

## 4.0 Roles and Responsibilities
*   **Data Owner (Head of Department):** Ultimately responsible for classifying the data their department creates and uses.
*   **Data Custodian (IT Department):** Responsible for implementing and maintaining technical controls to protect data according to its classification.
*   **Data User (All Personnel):** Responsible for understanding and adhering to this policy for the data they access and handle.

## 5.0 Review
This policy shall be reviewed annually by the Head of Data Governance and the CISO.