# Comprehensive Guide to Cybersecurity Frameworks

## 1. NIST Framework

The National Institute of Standards and Technology (NIST) Cybersecurity Framework is a voluntary framework consisting of standards, guidelines, and best practices to manage cybersecurity risk.

### Core Components
- **Identify**: Develop organizational understanding to manage cybersecurity risk
- **Protect**: Implement safeguards to ensure delivery of critical services
- **Detect**: Implement activities to identify cybersecurity events
- **Respond**: Take action regarding a detected cybersecurity incident
- **Recover**: Maintain resilience and restore capabilities impaired by cybersecurity incidents

### Key Publications
- **NIST SP 800-53**: Security and privacy controls for information systems
- **NIST SP 800-171**: Protecting controlled unclassified information
- **NIST SP 800-61**: Computer security incident handling guide

### Implementation Tiers
The framework defines implementation tiers from Partial (Tier 1) to Adaptive (Tier 4), measuring an organization's cybersecurity risk management practices.

## 2. ISO 27000 Series

### ISO 27001
The international standard for information security management systems (ISMS).

**Key Components**:
- Risk assessment methodology
- Security policy
- Organization of information security
- Human resource security
- Asset management
- Access control
- Cryptography
- Physical security
- Operations security
- Communications security
- System acquisition and development
- Supplier relationships
- Incident management
- Business continuity
- Compliance

### ISO 27017
Focuses specifically on information security controls for cloud services.

**Key Focus Areas**:
- Shared roles between cloud service providers and customers
- Removal/return of assets at contract termination
- Protection of virtual environments
- Cloud service customer data segregation
- Virtual machine hardening
- Administrator operational security

### ISO 27018
Addresses the protection of personally identifiable information (PII) in public cloud environments.

**Key Focus Areas**:
- Consent for use of PII
- Control over PII processing
- Transparency of PII processing
- Data minimization
- PII disclosure limitations
- Data breach notification requirements
- Data retention and deletion practices

## 3. CIS Controls & Benchmarks

### CIS Top 20 Controls
A prioritized set of actions to protect organizations from known cyber-attack vectors, organized in three implementation groups:

**Basic Controls (1-6)**:
1. Inventory and control of hardware assets
2. Inventory and control of software assets
3. Continuous vulnerability management
4. Controlled use of administrative privileges
5. Secure configuration for hardware and software
6. Maintenance, monitoring, and analysis of audit logs

**Foundational Controls (7-16)**:
7. Email and web browser protections
8. Malware defenses
9. Limitation and control of network ports
10. Data recovery capabilities
11. Secure configuration for network devices
12. Boundary defense
13. Data protection
14. Controlled access based on need to know
15. Wireless access control
16. Account monitoring and control

**Organizational Controls (17-20)**:
17. Security awareness and training program
18. Application software security
19. Incident response and management
20. Penetration tests and red team exercises

### CIS Benchmarks
Detailed configuration guidelines for various technology products and environments including:
- Operating systems (Windows, Linux, macOS)
- Cloud providers (AWS, Azure, GCP)
- Databases (SQL, Oracle, MongoDB)
- Web servers (Apache, Nginx, IIS)
- Network devices (Cisco, Juniper)
- Containers (Docker, Kubernetes)
- Mobile devices (iOS, Android)

## 4. MITRE ATT&CK Framework

A globally-accessible knowledge base of adversary tactics and techniques based on real-world observations.

### Structure
- **Tactics**: The adversary's technical goals (the "why")
- **Techniques**: How those goals are achieved (the "how")
- **Procedures**: Specific implementations of techniques

### Matrix Categories
- **Enterprise Matrix**: Covers Windows, macOS, Linux, cloud, and network environments
- **Mobile Matrix**: Focuses on iOS and Android
- **ICS Matrix**: Industrial Control Systems specific threats

### Key Tactics (Enterprise)
1. Initial Access
2. Execution
3. Persistence
4. Privilege Escalation
5. Defense Evasion
6. Credential Access
7. Discovery
8. Lateral Movement
9. Collection
10. Command and Control
11. Exfiltration
12. Impact

### Applications
- Threat modeling
- Security gap analysis
- Red team/blue team exercises
- Security control mapping
- Detection and response strategy

## 5. OWASP (Open Web Application Security Project)

### OWASP Top 10 Web Application Security Risks (2021)
1. Broken Access Control
2. Cryptographic Failures
3. Injection
4. Insecure Design
5. Security Misconfiguration
6. Vulnerable and Outdated Components
7. Identification and Authentication Failures
8. Software and Data Integrity Failures
9. Security Logging and Monitoring Failures
10. Server-Side Request Forgery

### OWASP Mobile Top 10 (2016)
1. Improper Platform Usage
2. Insecure Data Storage
3. Insecure Communication
4. Insecure Authentication
5. Insufficient Cryptography
6. Insecure Authorization
7. Client Code Quality
8. Code Tampering
9. Reverse Engineering
10. Extraneous Functionality

### OWASP API Security Top 10 (2023)
1. Broken Object Level Authorization
2. Broken Authentication
3. Broken Object Property Level Authorization
4. Unrestricted Resource Consumption
5. Broken Function Level Authorization
6. Unrestricted Access to Sensitive Business Flows
7. Server Side Request Forgery
8. Security Misconfiguration
9. Improper Inventory Management
10. Unsafe Consumption of APIs

### Additional OWASP Resources
- OWASP Testing Guide
- OWASP Code Review Guide
- OWASP Application Security Verification Standard (ASVS)
- OWASP Software Assurance Maturity Model (SAMM)
- OWASP Developer Guide
