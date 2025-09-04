# Statement of Applicability (SoA)

**Organization:** SecureBank Finance
**ISMS Scope:** Retail banking and investment services for EU customers, including the Online Banking Platform, Core Banking System, and related infrastructure.
**SoA Version:** 1.2
**Date:** 2023-10-27
**Related Documents:** `02-Risk-Assessment-Report.md`, `03-Risk-Treatment-Plan.md`

## Introduction
This Statement of Applicability identifies the controls from ISO/IEC 27001:2022 Annex A that SecureBank Finance has decided to implement to treat its information security risks. The selection is based on the results of the risk assessment and treatment process.

**Legend:**
*   **I:** Implemented
*   **PI:** Partially Implemented
*   **P:** Planned (Target Date Q2 2024)
*   **NI:** Not Implemented
*   **E:** Excluded

---

### A.5: Organizational Controls

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.5.1** | **Policies for information security** | | |
| A.5.1.1 | Policies for information security | I | **Included.** Mandatory for the ISMS. Defined in `information-security-policy.md`. |
| A.5.1.2 | Review of the policies for information security | I | **Included.** All policies are scheduled for annual review by the CISO and relevant owners. |
| **A.5.2** | **Information security roles and responsibilities** | | |
| A.5.2.1 | Segregation of duties | I | **Included.** Critical financial control to prevent fraud. Applied in core banking and finance systems. |
| A.5.2.2 | Responsibilities for information security | I | **Included.** Defined in the InfoSec Policy and role descriptions for CISO, asset owners, etc. |
| A.5.2.3 | Contact with authorities | I | **Included.** Legal & Compliance team maintains formal contacts with financial regulators (ECB, [Local Authority]) and data protection authorities. |
| A.5.2.4 | Contact with special interest groups | I | **Included.** Membership and contact with industry groups (e.g., FS-ISAC) for threat intelligence sharing. |
| A.5.2.5 | Information security in project management | PI | **Included.** Security sign-off is required for all major projects. Formal "Secure by Design" methodology is being developed (Target: Q1 2024). |
| **A.5.7** | **Threat intelligence** | | |
| A.5.7.1 | Threat intelligence | I | **Included.** Critical for proactive defense. Subscribed to financial-sector specific TI feeds (e.g., FS-ISAC). Integrated into our SOC operations. |
| **A.5.9** | **Inventory of information and other associated assets** | | |
| A.5.9.1 | Inventory of information and other associated assets | PI | **Included.** A CMDB exists for IT hardware. Formal inventory of information assets (datasets) is in progress. |
| A.5.9.2 | Ownership of information and other associated assets | I | **Included.** All critical assets (e.g., Customer DB, CBS) have designated owners. |
| A.5.9.3 | Acceptable use of information and other associated assets | I | **Included.** Mandated by the `acceptable-use-policy.md`. All employees must acknowledge this annually. |
| A.5.9.4 | Return of assets | I | **Included.** Process managed by HR and IT for offboarding. Defined in the Asset Management Policy. |
| **A.5.10** | **Cryptography** | | |
| A.5.10.1 | Cryptographic controls | I | **Included.** Mandatory. TLS 1.2+ for all public-facing services and data in transit. AES-256 encryption for sensitive data at rest. Key management follows PCI DSS requirements. |
| **A.5.11** | **Physical security** | | |
| A.5.11.1 | Physical security perimeters | I | **Included.** Data centers and server rooms have access controls (keycards, logs, cameras). |
| A.5.11.2 | Physical entry controls | I | **Included.** Access is based on the principle of least privilege and is logged. |
| A.5.11.3 | Securing offices, rooms, and facilities | I | **Included.** Alarmed and monitored premises. |
| A.5.11.4 | Physical security monitoring | I | **Included.** 24/7 monitoring of critical facilities. |
| A.5.11.5 | Protecting against physical and environmental threats | I | **Included.** Data centers have environmental controls (AC, fire suppression). |
| A.5.11.6 | Working in secure areas | I | **Included.** Policies for clean desks and securing sensitive material in locked cabinets. |
| A.5.11.7 | Clear desk and clear screen | I | **Included.** Policy enforced and part of security awareness training. |
| **A.5.12** | **Identity management** | | |
| A.5.12.1 | Identity management | I | **Included.** Formal joiner-mover-leaver process managed by HR and IAM team. Unique user IDs for all personnel. |
| A.5.12.2 | Access provisioning | I | **Included.** Access is granted based on formal requests approved by managers and data owners. |
| **A.5.15** | **Access control** | | |
| A.5.15.1 | Access control policy | I | **Included.** Defined in the `access-control-policy.md`. | This control also satisfies PCI DSS Req 3 and GDPR Art. 32.
| A.5.15.2 | User access provisioning | I | **Included.** Follows a formal request and approval workflow. |
| A.5.15.3 | Application access control | I | **Included.** Role-Based Access Control (RBAC) is implemented in critical applications (CBS, online banking). |
| **A.5.16** | **Identity and access governance** | | |
| A.5.16.1 | Identity and access governance | I | **Included.** Access reviews are conducted semi-annually for privileged accounts and annually for standard users. |
| A.5.16.2 | User access reviews | I | **Included.** Conducted by system owners. Evidence is retained. |
| A.5.16.3 | Removal of access rights | I | **Included.** Automated de-provisioning process initiated by HR upon termination. |

### A.6: People Controls

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.6.1** | **Screening** | | |
| A.6.1.1 | Screening | I | **Included.** Background checks are mandatory for all employees and contractors, as per HR policy, especially for roles with access to financial systems. |
| **A.6.2** | **Terms and conditions of employment** | | |
| A.6.2.1 | Terms and conditions of employment | I | **Included.** Employment contracts include clauses on confidentiality and adherence to security policies. |
| **A.6.3** | **Information security awareness, education, and training** | | |
| A.6.3.1 | Information security awareness, education, and training | I | **Included.** Mandatory annual training for all staff. Additional targeted training for roles with higher risk. |
| **A.6.4** | **Disciplinary process** | | |
| A.6.4.1 | Disciplinary process | I | **Included.** HR policies define the process for handling security violations. |

### A.7: Physical Controls
*(Note: Many physical controls are in A.5.11)*

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.7.1** | **Physical entry controls** | | |
| A.7.1.1 | Physical entry controls | I | **Included.** See A.5.11.2. |
| **A.7.2** | **Physical security monitoring** | | |
| A.7.2.1 | Physical security monitoring | I | **Included.** See A.5.11.4. |
| **A.7.3** | **Protecting against physical and environmental threats** | | |
| A.7.3.1 | Protecting against physical and environmental threats | I | **Included.** See A.5.11.5. |
| **A.7.4** | **Secure areas** | | |
| A.7.4.1 | Secure areas | I | **Included.** See A.5.11.1 and A.5.11.6. |

### A.8: Technological Controls

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.8.1** | **User endpoint devices** | | |
| A.8.1.1 | User endpoint devices | I | **Included.** Corporate devices are secured with mandated EDR, hard disk encryption, and are managed by an MDM. |
| **A.8.2** | **Privileged access rights** | | |
| A.8.2.1 | Privileged access rights | I | **Included.** Privileged accounts are managed via a PAM solution. Sessions are logged and monitored. MFA is required. |
| **A.8.3** | **Information access restriction** | | |
| A.8.3.1 | Information access restriction | I | **Included.** Implemented through network segmentation, ACLs, and application-level controls following the principle of least privilege. |
| **A.8.4** | **Access to source code** | | |
| A.8.4.1 | Access to source code | I | **Included.** Access to source code for critical applications (e.g., online banking) is restricted to authorized developers only and managed in a version control system. |
| **A.8.5** | **Secure authentication** | | |
| A.8.5.1 | Secure authentication | I | **Included.** MFA is mandatory for all remote access, privileged users, and customer-facing online banking. |
| **A.8.6** | **Capacity management** | | |
| A.8.6.1 | Capacity management | I | **Included.** Critical systems are monitored for capacity (CPU, memory, storage). Thresholds trigger alerts for proactive management. |
| **A.8.7** | **Protection against malware** | | |
| A.8.7.1 | Protection against malware | I | **Included.** Advanced malware protection (EDR) is deployed on all endpoints and servers. Email filtering blocks malicious attachments/links. |
| **A.8.8** | **Management of technical vulnerabilities** | | |
| A.8.8.1 | Management of technical vulnerabilities | I | **Included.** Formal patch management policy. Critical patches are applied based on risk, typically within 14 days of release. |
| **A.8.9** | **Configuration management** | | |
| A.8.9.1 | Configuration management | I | **Included.** Secure baselines exist for all major OS and network device types. Changes are managed via a formal ITIL-based change management process. |
| **A.8.10** | **Information deletion** | | |
| A.8.10.1 | Information deletion | I | **Included.** Data retention policies define secure deletion methods. Secure erasure tools are used for decommissioned hardware. |
| **A.8.11** | **Data masking** | PI | **Included.** Used in non-production environments (e.g., development, testing) that use copies of production data. **Excluded for customer service reps** who require full data visibility to assist customers. |
| **A.8.12** | **Data leakage prevention** | PI | **Included.** DLP is implemented on endpoints and email to prevent exfiltration of customer PII. **Cloud DLP for IaaS/PaaS is planned for implementation in Q2 2024.** |
| **A.8.13** | **Information backup** | I | **Included.** **Critical control.** Daily backups are performed. They are encrypted, stored offsite, and tested weekly for restore capability. |
| **A.8.14** | **Redundancy of information processing facilities** | I | **Included.** Critical systems (CBS, core networking) have redundant components to ensure availability. |
| **A.8.15** | **Logging** | I | **Included.** Logs from critical systems are forwarded to a central SIEM for correlation and analysis. Retention policy is 1 year for most logs, 7 years for critical financial transactions. |
| **A.8.16** | **Monitoring activities** | I | **Included.** The SOC team performs 24/7 monitoring of the SIEM for suspicious activities. |
| **A.8.17** | **Clock synchronization** | I | **Included.** All servers and network devices synchronize with internal NTP servers for accurate timestamping in logs, which is critical for forensic investigations. |
| **A.8.18** | **Use of privileged utility programs** | I | **Included.** Use of privileged utilities (e.g., PowerShell, WinRM) is restricted, logged, and monitored via the EDR/SIEM. |
| **A.8.19** | **Installation of software on operational systems** | I | **Included.** Users cannot install software. Software deployment is managed centrally by IT via the change management process. |
| **A.8.20** | **Networks security** | I | **Included.** Network is segmented (e.g., PCI DSS zone, corporate zone, DMZ). Firewalls and ACLs enforce segmentation rules. |
| **A.8.21** | **Security of network services** | I | **Included.** Security requirements are defined for all network services (e.g., provided by telecom providers). |
| **A.8.22** | **Segregation of networks** | I | **Included.** See A.8.20. Critical networks (e.g., SWIFT) are physically and logically segregated. |
| **A.8.23** | **Web filtering** | I | **Included.** Corporate internet access is filtered to block malicious and non-business related websites. |
| **A.8.24** | **Use of cryptography** | I | **Included.** See A.5.10.1. |

### A.9: Relationship Controls

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.9.1** | **Information security in supplier relationships** | | |
| A.9.1.1 | Information security in supplier relationships | I | **Included.** **Critical for finance.** Third-party risk management process includes security assessments and contractual obligations for key suppliers (e.g., cloud providers, payment processors). |
| A.9.1.2 | Addressing security within supplier agreements | I | **Included.** Contracts with suppliers include clauses mandating compliance with our security policies and right to audit. |
| A.9.1.3 | Information and communication technology supply chain | PI | **Included.** Security requirements are defined for hardware/software procurement. A formal process for assessing supply chain risk for critical vendors is in development. |
| **A.9.2** | **Supplier service delivery management** | | |
| A.9.2.1 | Monitoring and review of supplier services | I | **Included.** Performance and security of key suppliers (e.g., SaaS availability) are reviewed quarterly. |
| A.9.2.2 | Managing changes to supplier services | I | **Included.** Changes to supplier services that impact our security are assessed via the change management process. |

### A.10: Operational Controls

| Ref. | Control Title | Status | Justification for Inclusion/Exclusion |
| :--- | :--- | :--- | :--- |
| **A.10.1** | **Information transfer policies and procedures** | | |
| A.10.1.1 | Information transfer policies and procedures | I | **Included.** Policies define secure methods for transferring sensitive information (e.g., encrypted email, secure file transfer portals). |
| **A.10.2** | **Agreements on information transfer** | | |
| A.10.2.1 | Agreements on information transfer | I | **Included.** Data sharing agreements are in place with partners and third parties, specifying security requirements. |

## Summary of Exclusions
Controls may be excluded for the following reasons:
1.  **No Identified Risk:** The control does not address any risk identified in our risk assessment.
2.  **Not Applicable:** The control is not relevant to our business context, technology stack, or legal environment.
3.  **Implemented Elsewhere:** The control objective is achieved through an alternative method or managed under a different framework (e.g., physical security of ATMs).

**Note:** This SoA is a living document. It will be reviewed and updated at least annually, or in response to significant changes, as part of the management review process.