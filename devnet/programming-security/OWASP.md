# Programming Security
- OWASP = Open Web Application Security Project
    - Non-profit org to help developers create more secure web apps
    - Regularly update "Top 10" vulnerability list
- Flagship Projects:
    - Top 10 proactive controls: initial awareness around building secure web applications.
        - C1: Define security requirements
        - C2: Leverage Security Frameworks and Libraries
        - C3:Secur Database Access
        - C4: Encode and Escape Data
        - C5: Validate all inputs
        - C6: Implement Digital Identity
        - C7: Enforce Access Controls
        - C8: Protect Data Everywhere
        - C9: Implement Security logging and monitoring
        - C10: Handle all errors and exceptions
    - Application Security Verification Standard (ASVS): list of requirements for developers to work against. While building/developing/testing.
        - Level 1: minimum amount of security for any application
        - Level 2: any sensitive data or logic is in play. Medium security.
        - Level 3: Critical applications and/or critical sectors: healthcare, government, etc.
    - Cheat Sheets Series: easily accessible summary of most valuable information regarding top 10 vulns.
        - Implementation and secure design resource.
    -Software Assurance Maturity Model (SAMM): prescriptive model to iteratively improve security in organization.
        - Each stream feature 3 maturity levels. 
        - https://owaspsamm.org/guidance/quick-start-guide/
        - SAMM Excel Toolbox
    - Web Security Testing Guide (WSTG)
        - Deploy > find issue > patch = wrong
        - A set of tests to use throughout the entire application development process.
        - "Secure Software Design Lifecycle"
        - Think CI/CD, can I automate this?
## "Top 10" vulnerability list:
- Injection attack
    - Attacker sends malicious code to web app via HTTP POST/PUSH
    - Input validation prevents code injects
    - MVC provides segmentation
- Broken Authentication
    - Authentication secrets are stored incorrectly
    - Auth systems are weekly implemented 
    - MFA, password complexity, retry attempt limits can protect auth systems
- Sensitive Data Exposure
    - HTTPS protects data in transit
    - Encrypted data at rest/remove old data
- XML External Entity (XXE)
    - Instead of referencing XML entity, server processes other code, file systems, code etc.
    - Disable XXX feature in XML
- Broken Access Control
    - App allowing free access to sensitive resources
    - Principle of least privilege, denied by default, reduce external accessibility, disabling accounts hiding metadata
- Security misconfiguration
    - Failing to remove default configs, credentials, week implementations
- Cross-site scripting
    - Attacker imbeds code on web server, user activates code when they access resource
    - Grants all info that browser knows, common to man in the middle attackers
- Cross-site Request Forgery
    - Requests can be activated by user interaction with other web pages, while first session is still authenticate
    - Refer header: ensure requests are coming from original site
    - Use hashes to nuance requests
- Insecure deserialization
    - Attacker deserializes data in transit, alters data to fulfill purpose, reserializes and sends it on its way.
    - Common with MITM attacks/remote code execution.
    - Log serialization/deserialization failures, catch attacker trial and error attempts.
    - Hashing to prevent unauth'd writes.
- Using known vulnerabilities
    - Delaying updates
    - Remove legacy/EOL/unsupported products.
- Insufficient logging and monitoring
    - Can't protect what you can't see
    - Good SIEM provides visibility
- Honorable mentions
    - Code Quality:
        - Conversion errors
        - Poor Debug practices
        - Time of Check/Use
            - Validation happens separately from use process, attacker bypasses validation
        - Use: Static Code analysis
    - Denial of Service
    - Memory Management:
        - Buffer overflow
