# ISMS Scope and Context
Document ID: DOC-SCOPE-001
Version: 1.1
Effective Date: October 26, 2023
Approval Authority: Chief Information Security Officer (CISO)

# 1.0 Context of the Organization
SecureBank Finance operates within a complex environment shaped by internal capabilities and external pressures. Understanding this context is essential for establishing a relevant and effective ISMS.

# 1.1 Internal Issues
Factor	Description	Implication for the ISMS
Business Model	Provision of retail banking and investment services.	The ISMS must prioritize the protection of highly sensitive customer financial data.
Organizational Structure	Centralized HQ with branch networks.	Security policies and controls must be consistently applicable and enforceable across all locations.

Technology Landscape	Mix of modern digital platforms and legacy core banking systems (CBS).	The ISMS must account for different risk profiles and security capabilities across the technology estate.
Cultural Context	A established culture of security awareness and regulatory compliance.	Provides a strong foundation for implementing and maintaining the ISMS.

Strategic Direction	Increasing demand for and investment in digital services.	The ISMS must be agile to securely enable digital transformation and cloud adoption.

# 1.2 External Issues
Factor	Description	Implication for the ISMS
Legal & Regulatory	Subject to strict regulations (GDPR, PCI DSS, PSD2, and oversight from [e.g., FCA, ECB]).	The ISMS is a critical tool for demonstrating compliance and avoiding significant financial penalties.
Competitive Environment	Highly competitive financial services sector.	Security is a key competitive differentiator; breaches cause significant reputational damage.

Technological Environment	Sophisticated cyber threats from organized crime and state-sponsored actors targeting the financial sector.	Requires a robust, intelligence-driven security posture with advanced defensive controls.
Social & Customer	Customers have high expectations for both digital convenience and the security of their assets and data.	The ISMS must balance security controls with user experience to maintain trust and satisfaction.
Economic	Economic pressures to optimize costs.	The ISMS must implement cost-effective security controls that provide clear risk reduction.
2.0 Interested Parties

The ISMS is designed to meet the needs and expectations of the following key interested parties:

Interested Party	Needs and Expectations
Customers	Privacy, confidentiality, and availability of their financial data and services.

Regulators (e.g., FCA, SEC, Data Protection Authority)	Compliance with all applicable financial and data protection regulations and laws.
Employees	Clear security guidelines, training, and tools to perform their jobs securely and efficiently.

Partners & Suppliers (e.g., SWIFT, VISA, Cloud Providers)	Adherence to contractual and industry security standards (e.g., PCI DSS, SWIFT CSP).
Shareholders	Protection of corporate assets and brand value; avoidance of financial losses from incidents.

# 3.0 ISMS Scope Statement
The scope of the Information Security Management System is defined below and has been established to manage information security risks to the defined business processes and assets.

# 3.1 Business Processes & Services In Scope
Retail banking services for EU customers.

Investment and wealth management services for EU customers.

Management of the customer relationship lifecycle (onboarding, servicing, offboarding).

# 3.2 Organizational Boundaries In Scope
SecureBank Finance headquarters.

All retail branch locations within the European Union.

Key third-party suppliers that process, store, or transmit in-scope data (see 3.4).

# 3.3 Information Assets In Scope
Data: All customer Personally Identifiable Information (PII) and financial data.

Applications: The Online Banking Platform (web and mobile applications), the Core Banking System (CBS), and all supporting internal applications.

Technology Infrastructure: The internal corporate network, data centers, and servers hosting in-scope applications and data.

Physical Assets: End-user devices (laptops, workstations) and network equipment within the organizational boundaries.

# 3.4 Third Parties In Scope
The ISMS extends to governing the security of services provided by third parties that interact with in-scope assets, including:

Cloud Infrastructure as a Service (IaaS) providers hosting in-scope systems.

Payment processing partners.

Software as a Service (SaaS) providers handling customer data.

# 3.5 Exclusions from Scope
The following are explicitly excluded from the scope of this ISMS:

Marketing Data: The marketing department's social media analytics data, provided it has been fully anonymized and contains no PII.

Physical Security of ATMs: The physical security and management of Automated Teller Machines (ATMs) are governed by a separate physical security framework managed by the Facilities department.

Group-Level Systems: Group-wide HR and financial reporting systems that do not process customer PII from in-scope services.

Justification for Exclusions: The exclusions listed above have been assessed and present a significantly lower risk to the confidentiality, integrity, and availability of in-scope customer financial data. Their management under separate, dedicated frameworks is a more efficient and effective control structure.

