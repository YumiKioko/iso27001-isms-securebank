# Access Control Policy

**Policy Identifier:** POL-ACP-003
**Version:** 1.0
**Effective Date:** 2023-10-27
**Approval Authority:** Chief Information Security Officer (CISO)
**Policy Owner:** Head of Identity & Access Management (IAM)

## 1.0 Purpose
To define the rules for granting, reviewing, and removing access to SecureBank Finance's information assets, networks, and systems. This policy enforces the principles of least privilege and segregation of duties to minimize risk and protect sensitive customer and corporate data.

## 2.0 Scope
This policy applies to all users, systems, and processes that are involved in requesting, approving, provisioning, reviewing, or deprovisioning access to any in-scope system or data set.

## 3.0 Policy

### 3.1 Access Control Principles
1.  **Least Privilege:** Users shall be granted the minimum level of access to systems and data necessary to perform their legitimate job functions.
2.  **Segregation of Duties (SoD):** Access shall be designed to prevent a single user from being able to complete a critical business function alone (e.g., initiating and approving a payment; creating a vendor and processing an invoice).
3.  **Need-to-Know:** Access to Confidential information is granted based on a verified business need, not just seniority or role.

### 3.2 User Access Management
#### 3.2.1 User Registration and De-registration
*   A formal user access request process must be followed for all new access.
*   All access requests must be approved by the relevant Data/System Owner and the user's manager.
*   Access for employees, contractors, and third-party users must be immediately revoked upon termination of employment or contract. The process is managed by HR initiating a workflow in the IAM system.

#### 3.2.2 User Authentication
*   **Standard Users:** Access to the corporate network and standard business applications requires a unique user ID and a strong password.
*   **Privileged Users:** Access to administrative accounts, core banking systems, and sensitive databases requires Multi-Factor Authentication (MFA).
*   **Remote Access:** All remote access to the corporate network must be via the approved VPN solution with MFA.

### 3.3 System and Application Access Control
1.  **Access Control Lists:** Access to shared network drives and databases must be controlled via Access Control Lists (ACLs) reviewed quarterly by the data owner.
2.  **Source Code Access:** Access to source code repositories for critical applications (e.g., online banking) is restricted to authorized development personnel only.
3.  **Default Passwords:** All default passwords on systems and software must be changed before deployment into a production environment.

### 3.4 Access Rights Review
*   Data and System Owners are required to review user access rights for their systems on a semi-annual basis.
*   Any discrepancies or inappropriate access must be revoked immediately.
*   Evidence of these reviews must be documented and retained.

## 4.0 Compliance
### 4.1 Enforcement
Violations of this policy may result in disciplinary action, revocation of access, and legal penalties.

### 4.2 Review
This policy shall be reviewed annually by the Head of IAM and the CISO.