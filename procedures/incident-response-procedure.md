# Incident Response Procedure

**Procedure Identifier:** PROC-IR-001
**Version:** 1.1
**Related Policy:** POL-IRP-004 (Incident Response Plan)
**Effective Date:** 2023-10-27
**Owner:** Security Operations Center (SOC) Manager

## 1.0 Purpose
This procedure provides detailed, step-by-step instructions for the triage, analysis, containment, eradication, and recovery from information security incidents at SecureBank Finance. It ensures a consistent, effective, and timely response to minimize operational, financial, and reputational damage.

## 2.0 Scope
This procedure applies to the SOC team, IT Operations, and all members of the Incident Response Team (IRT). It covers all in-scope systems, networks, and data.

## 3.0 Workflow
The overall workflow adheres to the NIST SP 800-61 framework:
`Preparation -> Detection & Analysis -> Containment -> Eradication & Recovery -> Post-Incident Activity`

## 4.0 Roles & Responsibilities during Incident
*   **SOC Analyst (Tier 1/2):** First responder; performs initial triage, containment, and evidence collection.
*   **SOC Manager / Incident Lead:** Confirms the incident, directs all technical response efforts, and communicates with the CISO.
*   **CISO (Incident Director):** Activates the full IRT, makes strategic decisions, and is the point of escalation.
*   **IT Operations Lead:** Coordinates resources for containment and recovery actions (e.g., network segmentation, system restoration).
*   **Legal Counsel / DPO:** Advises on regulatory reporting requirements (e.g., GDPR 72-hour mandate).

## 5.0 Procedure

### 5.1 Phase 1: Detection & Reporting
1.  **Initial Alert:** An alert is generated via:
    *   **SIEM Correlation Rule**
    *   **EDR/AV Alert**
    *   **User Report** (via `soc@securebank.example` or internal hotline)
    *   **Threat Intelligence Feed**
2.  **Create Ticket:** The SOC analyst must immediately create a ticket in the Incident Management System (e.g., Jira Service Desk, ServiceNow). The ticket must be classified with the initial priority.
    *   **P1 - Critical:** Confirmed breach of CIA; active ransomware; core system downtime.
    *   **P2 - High:** Likely malicious activity with significant impact (e.g., successful phishing).
    *   **P3 - Medium:** Suspicious activity requiring investigation.
    *   **P4 - Low:** False positive or minimal impact.

### 5.2 Phase 2: Triage & Analysis
1.  **Initial Triage:** The assigned SOC analyst investigates the alert to determine if it is a True Positive.
    *   **Actions:** Review logs (EDR, firewall, authentication), interview reporting user, analyze network traffic (PCAP).
    *   **Goal:** Confirm or deny the incident. Document all findings in the ticket.
2.  **Escalation:** If an incident is confirmed, the SOC analyst must:
    *   Immediately escalate to the SOC Manager.
    *   The SOC Manager notifies the **CISO** and begins activating the IRT for P1/P2 incidents.
3.  **Deep Analysis & Forensics:**
    *   **Isolate** the affected system(s) but **DO NOT POWER THEM OFF** to preserve volatile memory for forensics.
    *   **Capture Evidence:** Take a forensic disk image (`dd` or FTK Imager) and memory capture (Volatility, Belkasoft RAM Capturer).
    *   **IoC Hunting:** Search for related Indicators of Compromise (IPs, hashes, domains) across the enterprise using the SIEM.
    *   **Establish Scope:** Determine what data, systems, and user accounts are impacted.

### 5.3 Phase 3: Containment
The goal is to prevent further damage. Choose a containment strategy based on the incident type and scope.

#### 3.1 Short-Term Containment (Immediate)
*   **Compromised User Account:** Disable the account in Active Directory. Force logout of all sessions. Reset password.
*   **Compromised Endpoint:**
    *   **Primary Action:** Disconnect the machine from the network (disable switch port via NAC or have on-site staff unplug Ethernet).
    *   **Secondary Action:** If remote, isolate the host via EDR tool quarantine function.
*   **Malicious IP/Domain:** Block at the perimeter firewall and internal DNS sinkhole (Cisco Umbrella, etc.).
*   **Phishing Campaign:** Delete all instances of the email from user mailboxes using Microsoft 365 Compliance Center / Exchange Online PowerShell.

#### 3.2 Long-Term Containment
*   Apply patches to vulnerable systems.
*   Remove the attacker's persistence mechanisms (scheduled tasks, new services, registry keys).
*   Change passwords for any potentially compromised privileged accounts.

### 5.4 Phase 4: Eradication & Recovery
1.  **Eradication:** Remove all components of the incident.
    *   **Malware:** Use EDR to remove the malicious file. Rebuild the host from a known-good gold image if rootkit is suspected.
    *   **Attacker Access:** Identify and close all backdoors. Review all user and service accounts for anomalies.
2.  **Recovery:** Restore operations securely.
    *   **Restore Data:** Restore clean data from the most recent, verified backup. Validate data integrity.
    *   **Return to Service:** Reconnect the system to the network. Monitor closely for signs of re-infection.
    *   **User Communication:** Inform affected users they can resume normal activity.

### 5.5 Phase 5: Post-Incident Activity
1.  **Blameless Post-Mortem Meeting:**
    *   **Scheduled:** Within 1 week of incident resolution.
    *   **Attendees:** All involved IRT members and technical staff.
    *   **Agenda:** What happened? How was it handled? What went well? What can be improved?
2.  **Incident Report:** The SOC Manager drafts a formal report including:
    *   Executive Summary
    *   Timeline of Events
    *   Root Cause Analysis
    *   Impact Assessment (financial, operational, reputational)
    *   Lessons Learned and Action Items
3.  **Corrective Actions:** Convert Lessons Learned into actionable items in the Corrective Action Log (`records/corrective-action-log.csv`). Examples:
    *   "Update SIEM correlation rule to detect new TTP."
    *   "Implement stricter firewall rules for egress traffic."
    *   "Launch targeted security awareness training on phishing."

## 6.0 Appendix A: Common Incident Playbooks

### 6.1 Ransomware Playbook
1.  **ISOLATE** the infected host immediately.
2.  **DETERMINE** the variant (if possible) using ID Ransomware or vendor tools.
3.  **DO NOT PAY THE RANSOM.** Engage Legal and Communications.
4.  **IDENTIFY** patient zero and initial attack vector.
5.  **RESTORE** from backups after ensuring backups are clean and the vulnerability is patched.

### 6.2 Phishing (Credential Theft) Playbook
1.  **DELETE** the phishing email from all mailboxes.
2.  **DISABLE** the compromised user account.
3.  **RESET** the user's password and implement MFA if not already enabled.
4.  **CHECK** the user's mailbox for forwarding rules and sent items.
5.  **SEARCH** logs for any sign of lateral movement from the user's account.

## 7.0 Appendix B: Evidence Handling
*   All evidence must be handled in a manner that preserves its integrity for potential legal proceedings.
*   Maintain a **Chain of Custody** log for any physical evidence.
*   Store forensic images on a secure, write-protected drive.

## 8.0 Review
This procedure shall be reviewed and tested via tabletop exercises every six months.