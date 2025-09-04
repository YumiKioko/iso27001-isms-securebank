# User Access Review Procedure

**Procedure Identifier:** PROC-ACC-001
**Version:** 1.0
**Related Policy:** POL-ACP-003 (Access Control Policy)
**Owner:** Head of Identity & Access Management (IAM)

## 1.0 Purpose
To provide a consistent and auditable process for reviewing user access rights to ensure they remain appropriate for business needs and comply with the principle of least privilege. This is a key control for preventing insider threat and fraud.

## 2.0 Scope
Applies to all user accounts with access to in-scope systems and data.

## 3.0 Review Cycles
*   **Privileged Accounts** (Domain Admins, root, etc.): Quarterly
*   **Critical Systems** (Core Banking, SWIFT, DBs with PII): Semi-Annually
*   **Standard User Accounts:** Annually

## 4.0 Procedure

### 4.1 Preparation
1.  The IAM team generates an access report for the system in scope.
2.  The report is sent to the designated **System Owner** and the user's **Line Manager**.

### 4.2 Review
1.  The System Owner and Line Manager review each user's access.
2.  They confirm if access is still required for business purposes ("Approve") or if it should be revoked ("Revoke").
3.  Justification for continued access must be provided.

### 4.3 Certification
1.  The reviewers electronically sign the access review report, certifying its accuracy.

### 4.4 Remediation
1.  The IAM team executes the revocations as indicated in the certified report.
2.  All actions are documented in the IAM system.

### 4.5 Record Keeping
1.  The completed and signed access review report is archived as evidence for a period of three years.