# Information Security Risk Assessment Procedure

**Procedure Identifier:** PROC-RA-001
**Version:** 1.0
**Related Policy:** POL-ISMS-001 (Information Security Policy)

## 1.0 Purpose
To define the systematic process for identifying, analyzing, evaluating, and treating information security risks related to the confidentiality, integrity, and availability of SecureBank Finance's information assets. This procedure aligns with ISO 27005.

## 2.0 Scope
This procedure applies to all in-scope information assets and processes defined in the ISMS Scope.

## 3.0 Roles and Responsibilities
*   **CISO:** Oversees the risk assessment process, facilitates workshops, and approves the final report.
*   **Risk Assessment Team:** Comprised of IT, Compliance, Legal, and Business Unit representatives.
*   **Asset Owners:** Responsible for providing information about their assets and participating in the assessment.

## 4.0 Procedure
### 4.1 Risk Assessment Schedule
A full risk assessment shall be conducted:
*   Annually (Q2 of each fiscal year).
*   Upon significant changes to the business, technology, or threat landscape.
*   Following a major security incident.

### 4.2 Risk Identification
1.  **Asset Identification:** The team will identify and create an inventory of critical assets (e.g., Customer DB, Core Banking System, SWIFT Gateway).
2.  **Threat Identification:** Identify potential threats (e.g., cyber-attacks, insider threats, system failures, natural disasters).
3.  **Vulnerability Identification:** Identify weaknesses that could be exploited by threats (e.g., unpatched software, lack of employee awareness).
4.  **Impact Criteria:** Define impact levels (1-5) based on financial loss, reputational damage, regulatory fines, and operational disruption. A "5" signifies a catastrophic impact (>€5M, major regulatory action).

### 4.3 Risk Analysis
1.  **Likelihood:** Assign a likelihood rating (1-5) based on historical data, threat intelligence, and expert judgment.
2.  **Risk Level:** Calculate the inherent risk level: `Risk = Likelihood x Impact`.
3.  **Risk Matrix:** Use a 5x5 matrix to categorize risks as Low (1-6), Medium (7-12), High (13-20), or Very High (21-25).

### 4.4 Risk Evaluation
Compare the calculated risk levels against the risk acceptance criteria defined by senior management. All "High" and "Very High" risks are deemed unacceptable and must be treated.

### 4.5 Output
The output of this process is the **Risk Assessment Report** (`02-Risk-Assessment-Report.md`), which is an input to the **Risk Treatment Plan** (`03-Risk-Treatment-Plan.md`).