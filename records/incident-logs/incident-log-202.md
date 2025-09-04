Incident_ID,Date_Time_Detected,Reported_By,Description,Category,Severity,Status,Containment_Actions,Root_Cause,Resolution_Date,CAR_Linked
INC-2023-007,2023-08-04 14:22,SIEM Alert,"Multiple failed login attempts (brute force) against a public-facing developer VPN gateway from a foreign IP block. No successful logins.",Attempted Intrusion,Medium,Closed,"1. Blocked source IP at firewall.
2. No accounts compromised, so no reset required.","Misconfiguration: VPN gateway did not have geoblocking enabled for non-essential countries.",2023-08-04,CAR-2023-003
INC-2023-008,2023-09-01 09:15,User Report,"User in Marketing department reported a phishing email impersonating the HR team requesting password verification. One user clicked the link but did not enter credentials.",Phishing,Low,Closed,"1. Email deleted from all mailboxes via EOP.
2. Blocked malicious URL via DNS filtering.
3. Sent department-wide comms alerting of the scam.","User lacked awareness of latest phishing tactics. The email filter ruleset needed updating.",2023-09-01,CAR-2023-004
INC-2023-009,2023-10-05 03:18,EDR Alert,"EDR detected and blocked ransomware (Strain: LockBit) on a test engineering workstation. The machine was isolated from the production network as per policy.",Malware,High,Closed,"1. EDR automatically quarantined file and isolated host.
2. Machine was wiped and reimaged as a precaution.
3. Scanned network shares for any signs of lateral movement; none found.","Engineer downloaded a compromised software crack from an unofficial website for a personal project on a company device.",2023-10-05,CAR-2023-005
