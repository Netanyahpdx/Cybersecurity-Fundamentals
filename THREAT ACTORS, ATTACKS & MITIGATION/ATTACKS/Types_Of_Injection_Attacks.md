## TYPES OF INJECTION ATTACKS

### 1. (SQLi) SQL INJECTION:
**WHAT IT IS:** Injects malicious SQL queries into input fields to manipulate a database.
<br>**IMPACT:** Accesses sensitive data, modifies or deletes records, or gains administrative control.
<br>**EXAMPLE:** Entering ' OR '1'='1 in a login form to bypass authentication.
<br><br>
### 2. COMMAND INJECTION:
**WHAT IT IS:** Executes arbitrary system commands on a server through vulnerable applications.
<br>**IMPACT:** Attacker gains control over the server, steals data, or disrupts operations.
<br>**EXAMPLE:** Adding ; rm -rf / to input fields to delete system files.
<br><br>
### 3. (XSS) CROSS SITE SCRIPTING: 
**WHAT IT IS:** Injects malicious scripts into web pages viewed by other users.
<br>**IMPACT:** Steals session cookies, redirects users, or performs actions on behalf of victims.
<br>**EXAMPLE:** <script>alert('Hacked!')</script> displayed on a vulnerable webpage.
<br><br>
### 4. LDAP INJECTION:
**WHAT IT IS:** Manipulates Lightweight Directory Access Protocol (LDAP) queries to bypass authentication or retrieve unauthorized data.
<br>**IMPACT:** Grants access to sensitive directory information.
<br>**EXAMPLE:** (username=*/*) retrieves all users from a directory.
<br><br>
### 5. XML INJECTION:
**WHAT IT IS:** Injects malicious XML content into input fields.
<br>IMPACT: Disrupts XML-based systems or retrieves unauthorized data.
<br>EXAMPLE: Adding <!ENTITY xxe SYSTEM "file:///etc/passwd"> in XML input.
<br><br>
### 6. NoSQL INJECTION:
**WHAT IT IS:** Targets NoSQL databases by injecting malicious queries.
<br>**IMPACT:** Steals or manipulates unstructured data.
<br>**EXAMPLE:** { $ne: null } in a MongoDB query to bypass login.
<br><br>
### 7. EMAIL HEADER INJECTION:
**WHAT IT IS:** Injects malicious content into email headers.
<br>**IMPACT:** Sends spam or phishing emails from legitimate accounts.
<br>**EXAMPLE:** Adding \r\nBCC: victim@example.com in email inputs.
