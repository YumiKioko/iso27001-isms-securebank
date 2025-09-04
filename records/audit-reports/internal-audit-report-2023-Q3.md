# Internal Audit Report - ISMS

**Report ID:** AUDIT-ISMS-2023-02
**Audit Standard:** ISO/IEC 27001:2022
**Audit Dates:** 2023-09-10 to 2023-09-12
**Audit Scope:** ISMS Core Controls, Risk Management Process, and IT Operations
**Lead Auditor:** Anna Petrova
**Audit Team:** Michael Chen

## 1.0 Executive Summary
An internal audit of the ISMS was conducted to verify its conformity to ISO 27001:2022 and its effective implementation. The ISMS was found to be generally well-implemented and maintained. Two minor nonconformities and three opportunities for improvement were identified. The system is capable of achieving its intended outcomes.

## 2.0 Audit Findings

### 2.1 Conformities
*   The risk assessment process (Clause 6.1.2) is rigorously applied and well-documented.
*   The Incident Response Plan (POL-IRP-004) is comprehensive and understood by the SOC team.
*   Management review meetings are conducted regularly with clear outputs and actions.

### 2.2 Nonconformities

#### NC-2023-02-01 (Minor)
*   **Clause / Control:** 8.1 (Operational Planning) / A.5.7 (Threat intelligence)
*   **Finding:** The procedure for integrating threat intelligence feeds into the weekly vulnerability management process is not consistently documented or followed. Observed in two instances where high-risk threats were identified but not formally assessed for impact on existing assets within the mandated 48-hour window.
*   **Objective Evidence:** Interview with SOC Analyst J. Doe; Review of TI feed logs from 2023-08-15 and 2023-08-22.
*   **Requirement:** ISO 27001:2022 requires that processes needed for the ISMS are established, implemented, and maintained.

#### NC-2023-02-02 (Minor)
*   **Clause / Control:** 9.1 (Performance Evaluation) / A.7.2 (Training)
*   **Finding:** Records for security awareness training for three new contractors in the Finance Department were incomplete. The training was completed, but the signed acknowledgments were not filed in the central training records repository.
*   **Objective Evidence:** Review of HR onboarding list for 2023-08 and cross-reference with `/records/training-records/`.
*   **Requirement:** The organization shall retain documented information as evidence of the results of monitoring and measurement.

### 2.3 Opportunities for Improvement (OFI)
1.  **OFI-01:** Consider automating the access review reminder process (currently manual) to ensure timely reviews for all critical systems.
2.  **OFI-02:** The risk treatment plan could be enhanced with more specific, measurable objectives for risk reduction.
3.  **OFI-03:** Include a tabletop exercise with the Legal and Communications departments in the next incident response test.

## 3.0 Conclusion
The ISMS is effectively implemented and maintained. The identified nonconformities do not represent a systemic failure. Upon successful implementation of the corrective actions for the minor nonconformities, the system will demonstrate full conformity with ISO 27001:2022.

**Report Approved By:**
_________________________
Anna Petrova, Lead Auditor
2023-09-15

**Report Received By:**
_________________________
[Name of CISO], CISO
2023-09-15