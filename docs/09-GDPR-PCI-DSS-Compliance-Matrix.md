# GDPR & PCI DSS Compliance Matrix

**Document ID:** DOC-COMP-001
**Version:** 1.0
**Date:** 2023-10-27
**Owner:** Data Protection Officer (DPO) & CISO

## 1.0 Purpose
This document maps the controls implemented in the SecureBank Finance ISMS (ISO 27001:2022) to the key articles of the General Data Protection Regulation (GDPR) and the key requirements of the Payment Card Industry Data Security Standard (PCI DSS v4.0). This demonstrates how our integrated management system satisfies these critical legal and contractual obligations.

## 2.0 Compliance Mapping

### 2.1 GDPR Mapping

| GDPR Article / Principle | Requirement | ISMS Control / Document | Evidence / Implementation |
| :--- | :--- | :--- | :--- |
| **Art. 5** (Lawfulness, fairness, transparency) | Data is processed lawfully. | `policies/data-classification-policy.md` | Data classification ensures sensitive data is identified and handled correctly. |
| **Art. 15-22** (Data Subject Rights) | Right to access, rectification, erasure, etc. | `procedures/data-subject-request-procedure.md` | A defined procedure for handling requests within mandated timelines. |
| **Art. 24** (Responsibility of controller) | Implement appropriate technical measures. | **Entire ISMS.** The SoA (`04-Statement-of-Applicability.md`) demonstrates a systematic approach to implementing security controls. | |
| **Art. 25** (Data Protection by Design) | Integrate data protection into processing activities. | `procedures/change-management-procedure.md` | Security and privacy are mandatory considerations in all projects/changes. |
| **Art. 28** (Processor obligations) | Ensure processors provide sufficient guarantees. | `A.9.1.1` (Supplier relationships) in `04-SoA.md` | Vendor risk assessments and contracts mandate GDPR compliance. |
| **Art. 32** (Security of processing) | Implement appropriate security. | **Core of the ISMS.** Controls for encryption (`A.5.10.1`), confidentiality, integrity, availability, and resilience. | `04-SoA.md`, `03-Risk-Treatment-Plan.md` |
| **Art. 33** (Notification of a breach) | 72-hour breach notification mandate. | `policies/incident-response-plan.md` | The IRP includes specific procedures for assessing and reporting breaches to authorities. |

### 2.2 PCI DSS Mapping

| PCI DSS Requirement | Description | ISMS Control / Document | Evidence / Implementation |
| :--- | :--- | :--- | :--- |
| **Req 1** (Firewalls) | Install and maintain network security controls. | `A.8.20` (Networks security) in `04-SoA.md` | Firewall policy, network segmentation. |
| **Req 2** (System Configs) | Apply secure configurations to all system components. | `A.8.9` (Configuration management) in `04-SoA.md` | Secure baselines, change control. |
| **Req 3** (Protect Stored PAN) | Protect stored cardholder data (e.g., encryption). | `A.5.10.1` (Cryptographic controls) & `policies/data-classification-policy.md` | PAN is classified as Confidential and must be encrypted. |
| **Req 4** (Encrypt Transmission) | Encrypt transmission of cardholder data. | `A.5.10.1` (Cryptographic controls) | TLS 1.2+ mandated for all transmissions. |
| **Req 5** (Protect against malware) | Use anti-virus and anti-malware. | `A.8.7.1` (Protection against malware) in `04-SoA.md` | EDR solution deployed on all endpoints. |
| **Req 6** (Develop secure systems) | Develop and maintain secure systems and software. | `procedures/change-management-procedure.md` | Security testing is part of the change process. |
| **Req 7** (Access Control) | Restrict access by need-to-know. | `policies/access-control-policy.md` & `A.8.1.1` | Principle of least privilege enforced. |
| **Req 8** (Identify and authenticate) | Identify users and authenticate access. | `A.8.5.1` (Secure authentication) & `A.5.12.1` (Identity mgmt.) | MFA for all remote access and privileged users. |
| **Req 10** (Track and monitor access) | Log and monitor all access to cardholder data. | `A.8.15` (Logging) & `A.8.16` (Monitoring) | SIEM collects and correlates logs from critical systems. |
| **Req 12** (Security Policy) | Maintain a policy that addresses information security. | **The entire ISMS documentation suite.** | `02-Information-Security-Policy.md` and all supporting docs. |

## 3.0 Conclusion
The SecureBank Finance ISMS provides a comprehensive control framework that inherently addresses the core security requirements of both GDPR and PCI DSS. This integrated approach ensures consistent security management, avoids duplication of effort, and provides clear evidence of compliance to regulators and acquiring banks.