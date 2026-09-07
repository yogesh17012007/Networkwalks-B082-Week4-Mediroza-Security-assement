# Penetration Testing Report

## 1. Executive Summary

An authorized penetration testing assessment was conducted against
the Mediroza Hospital training environment.

The assessment identified weaknesses in authentication, document
password protection, and exposure of sensitive database information.

The defined M1, M2 and M3 objectives were successfully completed.

---

## 2. Scope

**Target:** Mediroza Hospital Training Environment

**Assessment Type:** Authorized Educational Penetration Test

**Primary Areas Assessed:**

- Web application authentication
- Protected PDF documents
- Database exposure
- Sensitive information access

---

## 3. Methodology

The assessment followed the project-defined workflow:

1. Identify the authentication weakness.
2. Demonstrate SQL Injection-based authentication bypass.
3. Access the authorized patient portal.
4. Retrieve three protected PDF reports.
5. Perform a controlled PDF password-security assessment.
6. Identify the exposed database backup.
7. Review the relevant database information.
8. Document staff/shareholder information.
9. Prepare the final penetration testing report.

---

# 4. Findings

## F-01 – SQL Injection Authentication Bypass

**Severity:** High

### Description

The application's authentication functionality was found to be
susceptible to SQL Injection.

The vulnerability allowed authentication controls to be bypassed
during the authorized assessment.

### Impact

An attacker could potentially gain access to application resources
without valid authentication.

### Recommendation

- Use parameterized queries/prepared statements.
- Validate user input.
- Avoid dynamically constructed SQL queries.
- Implement secure authentication controls.
- Monitor and log suspicious authentication activity.

### Evidence

`Evidence/M1-Initial-Access/`

---

## F-02 – Weak PDF Password Protection

**Severity:** Medium

### Description

Three protected PDF lab reports were retrieved during the assessment.

The provided Hash Calculator and Password Cracker were used as part
of the controlled password-security assessment.

The passwords for all three PDF files were successfully recovered.

### Impact

Weak document passwords may allow sensitive documents to be accessed
if the files are obtained by an unauthorized party.

### Recommendation

- Use strong and unique passwords.
- Avoid predictable passwords.
- Implement appropriate access controls.
- Prefer application-level authorization for sensitive documents.

### Evidence

`Evidence/M2-PDF-Password-Assessment/`

---

## F-03 – Database Backup Exposure

**Severity:** High

### Description

A database backup was discovered within the authorized training
environment.

The database contained information relevant to the M3 assessment,
including staff and shareholder data.

### Impact

Exposure of sensitive organizational information could lead to
privacy, financial, reputational, or social-engineering risks.

### Recommendation

- Remove unnecessary database backups from public locations.
- Restrict access to backup files.
- Encrypt sensitive backups.
- Implement proper server-side authorization.
- Regularly review exposed files and directories.
- Monitor access to sensitive resources.

### Evidence

`Evidence/M3-Database-Discovery/`

---

# 5. Evidence Summary

| ID | Milestone | Evidence |
|----|-----------|----------|
| E01 | M1 | login.png |
| E02 | M1 | initial_access.png |
| E03 | M2 | pdf1.png |
| E04 | M2 | pdf1_pass.png |
| E05 | M2 | pdf2.png |
| E06 | M2 | pdf2_pass.png |
| E07 | M2 | pdf3.png |
| E08 | M2 | pdf3_pass.png |
| E09 | M3 | m3_staff_shareholders.xlsx |

---

# 6. Remediation Priority

### High Priority

1. Fix the SQL Injection vulnerability.
2. Protect database backups from public access.
3. Implement proper authentication and authorization.

### Medium Priority

4. Strengthen PDF password protection.
5. Improve logging and monitoring.
6. Conduct a security retest after remediation.

---

# 7. Conclusion

The authorized penetration testing assessment successfully
demonstrated the identified security weaknesses in the controlled
training environment.

The primary issues identified were SQL Injection, weak document
password protection, and database backup exposure.

Implementing the recommended security controls and conducting a
follow-up security assessment will help reduce the identified risks.

---

## Disclaimer

This report is intended solely for the authorized educational
assessment environment.

The techniques and findings must not be applied to systems without
explicit authorization.
