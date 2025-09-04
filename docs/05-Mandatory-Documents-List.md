# Index of Mandatory Documents & Records
Document ID: DOC-INDEX-001
Version: 1.0
Date: 2023-10-27

# Introduction
This document serves as a master index for all mandatory documents and records required by ISO/IEC 27001:2022 for the SecureBank Finance ISMS. It provides a mapping between ISO clauses and the corresponding controlled documents or evidence locations within this repository and other organizational systems.

# Definitions:

Mandatory Document: A policy, procedure, or plan that establishes requirements and rules.

Mandatory Record: Evidence that proves activities have been performed and requirements met. Records are time-bound and cannot be updated once created.

# Part 1: Mandatory Documents (Policies, Plans, Procedures)
These documents define the "rules" of the ISMS and are subject to version control.

ISO 27001:2022 Clause	Document Title	Document ID	Location in Repository	Status

# 4.3	Scope of the ISMS	DOC-SCOPE-001	docs/01-ISMS-Scope.md	✅ Implemented

# 5.2	Information Security Policy	POL-ISMS-001	policies/information-security-policy.md	✅ Implemented

# 5.3	Organizational Roles, Responsibilities, and Authorities	(Covered in IS Policy)	-	✅ Addressed

# 6.1.2	Information Security Risk Assessment Process	PROC-RA-001	procedures/risk-assessment-procedure.md	✅ Implemented

# 6.1.3	Information Security Risk Treatment Process	DOC-RTP-001	docs/03-Risk-Treatment-Plan.md	✅ Implemented

# 6.2	Information Security Objectives	(Documented in Section 3.2 of 01-ISMS-Scope.md)	docs/01-ISMS-Scope.md	✅ Addressed

# 7.2	Competence Awareness & Training Procedure	(Covered in HR processes)	-	✅ Addressed

# 7.5	Documented Information Control Procedure	(Inherent in Git version control)	-	✅ Addressed

# 8.1	Operational Planning and Control	(Covered in various procedures e.g., incident-response-procedure.md)	procedures/	✅ Addressed

# 8.2	Information Security Risk Assessment Report	*(Output of PROC-RA-001)*	docs/02-Risk-Assessment-Report.md	✅ Implemented

# 8.3	Information Security Risk Treatment Plan	DOC-RTP-001	docs/03-Risk-Treatment-Plan.md	✅ Implemented

# 9.1	Monitoring, Measurement, Analysis & Evaluation Procedure	(Covered in internal-audit-procedure.md)	procedures/internal-audit-procedure.md	✅ Addressed

# 9.2.2	Internal Audit Procedure	PROC-IA-001	procedures/internal-audit-procedure.md	✅ Implemented

# 9.3	Management Review Agenda & Inputs/Outputs	(Defined in Management Review Minutes)	records/management-review-minutes.md	✅ Addressed

# 10.1	Nonconformity and Corrective Action Process	(Defined in Corrective Action Log)	records/corrective-action-log.csv	✅ Addressed
Part 2: Mandatory Records (Evidence)

These records provide evidence of implementation and performance. They are stored in designated locations, often with retention periods.

ISO 27001:2022 Clause	Record Description	Example / Format	Primary Storage Location	Retention Period

# 7.2	Records of training, skills, experience, and qualifications	Training certificates, signed acknowledgments, skills matrix	HR Management System (HRMS)

Indexed in: records/training-records/	5 years

# 8.1	Records of the monitoring and measurement of results	KPI dashboards, security tool reports, compliance scans	SIEM / Dashboarding Tools

Summary in: Management Review	2 years

# 8.2	Logs of activities performed by users and administrators	Authentication logs, change logs, SIEM events	Centralized SIEM	1 year (General)
7 years (Critical)

# 8.3	Results of the information security risk assessment and treatment	Risk Register, Risk Assessment Report	docs/02-Risk-Assessment-Report.md
docs/03-Risk-Treatment-Plan.md	Duration of ISMS + 3 years

# 9.2.2	Internal audit program and results	Audit schedule, audit reports, evidence checklists	records/audit-reports/
procedures/internal-audit-procedure.md	3 years

# 9.3	Results of management reviews	Meeting minutes, attendance, presented reports	records/management-review-minutes.md	Duration of ISMS + 3 years

# 10.1	Records of nonconformities and subsequent corrective actions	Corrective Action Requests (CARs), root cause analysis, evidence of closure	records/corrective-action-log.csv	3 years after closure

Part 3: Document Control & Repository Notes
Version Control: This Git repository serves as the primary system for managing the version history of all mandatory documents. The git log provides a full audit trail of authors, dates, and changes.

Records Storage: This repository contains indexes and summaries of records (e.g., training summaries, audit report conclusions). The actual evidentiary records (e.g., individual training certificates, raw SIEM logs) are stored in dedicated, secure systems (HRMS, SIEM, etc.) as indicated in the table above. This ensures a single source of truth and manages privacy/security concerns.

Retention: The defined retention periods comply with relevant legal, regulatory, and contractual requirements (e.g., GDPR, financial regulations).

Access Control: Access to this repository and the linked record storage systems is controlled based on the principle of least privilege.

This index shall be reviewed annually during the management review process.