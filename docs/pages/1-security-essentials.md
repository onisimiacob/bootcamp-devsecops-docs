# 🛡️ Security Essentials

- In this first module I learned that we need to secure:

    - Customer data.
    - Company data.
    - Internal applications.
    - User applications.

# Types of Security Attacks

- **Phising attack:** A human is the target, not a system
    - User will receive an email, or any other communication in order to get tricked and to give the attacker some sensitive information.

- **XSS - Cross Site Scripting**
    - Runs malicious code or scripts from malicious sources. When other users get connected, server serves the script which is executed on browser.

- **CSRF - Client Side Request Forgery**
    - This can steal session information and it happens on the user side, which allows the attacker to pretend be another user.

- **SSRF - Server Side Request Forgery**
    - This is executed on server which is more complicated, but often, much more dangerous as it can affect all users and can reach other resources, such as database or backend.

- **SQL Injection**
    - Allows users to inject malicious by exploits on libraries or more typically through unsanatized web applications, modifying the database.

- **Libraries**
    - They are thirdparty code, so they also have exploits or CVEs (Common Vulerability Exposures), to be identified and updated to stay protected.

- **Brute Force**
    - Some systems may allow very weak passwords, or does not have MFA (Multi-Factor Authentication) or more specifically, the lack of a ratelimit at API level to avoid brute force.

- **DoS** 
    - Here the lack of any ratelimit may be an issue as it can stress the server. It can be the frontend due to millions of calls, or backend if backend URL is reachable. In worse case scenarios, el Backend is open, attacker can even reach the database blocking new connections and denialing the service from the lowest layer (DB), not having any real Frontend traffic.

- **Security Principal**
    - We have to secure every possible entrypoint.

# OWASP and OWASP Top 10

1. Broken Control Access:
    - Users may run actions that shoud not be allowed to (violation of least priviledge principal).
2. Cryptographic Failures:
    - Hardcoded data, weak or lack of encryption of information, insecure protocols.
3. Injection
    - Allows to inject code such as JavaScript, SQL, NoSQL, OS commands.
4. Insecure Design
    - "Leave it like this, we will fix it later" and later never comes. Very typical situation on day to day projects...
5. Security Misconfiguration
    - Open ports, default passwords, infrastructure default values (public). It applies at every level; newwork, storage, application.
6. Vulnerable and Outdated Components
    - Everything is code, so if you fix you code, you also need to apply new versions of libraries.
7. Indentification and Authentication Failures
    - Errors at properly identify and authenticate users. Weak user confirmation, passwords, lack of mfa, sessions not invalidated.
8. Software and Data Integration Failures
    - Using libraries and plugins from unknown sources with weak digital signature.
9.  Security Logging and Monitoring Failures
    - Detect breaches and notify attach attempts.
10. Serverside Request Forgery (SSRF)
    - Malicious code executing from inside the server itself due to a vulnerability on both infrastructure or application.

