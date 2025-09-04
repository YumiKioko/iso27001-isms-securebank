Risk Treatment Plan

For each unacceptable risk, we select a treatment option (Avoid, Modify, Share, Retain).

Risk ID	Treatment Option	Selected Controls (from ISO 27002:2022)	Reason for Choice	Rationale for Exclusion (if applicable)
R-001	Modify	5.7 Threat intelligence
5.23 Information security for use of cloud services
8.12 Data leakage prevention	CSP security is shared responsibility. DLP and cloud-specific policies directly mitigate misconfigurations.	N/A
R-002	Modify	5.3 Segregation of duties
7.2 Phishing training (awareness)
8.7 Protection against malware (email filtering)	Multi-layered defense: training reduces click-rate, filtering reduces delivery, MFA prevents use of stolen creds.	N/A
R-003	Modify	5.26 Information security event reporting
7.13 Backup & Restore (Critical!)
8.16 Monitoring activities	Robust, tested backups are the primary mitigation. Monitoring allows for early detection.	N/A
R-004	Modify	5.3 Segregation of duties
8.1 User access management (least privilege)
8.12 Data leakage prevention	Least privilege and segregation limit what any single insider can access/do. DLP blocks exfiltration.	8.11 (Masking) was excluded for customer service reps who need to see full data to serve customers.
R-005	Modify	5.19 Information security in supplier relationships
5.22 Monitoring & review of supplier services
8.12 DLP (to protect data shared with them)	Contracts and audits are the primary levers to manage third-party risk.