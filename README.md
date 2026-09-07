# Mediroza Hospital – Penetration Testing

## Overview

This repository contains the documentation and evidence from an
authorized penetration testing assessment performed against the
Mediroza Hospital training environment.

The assessment was conducted for educational purposes in a controlled
environment.

## Assessment Objectives

The assessment consisted of four milestones:

- M1 – Initial Access
- M2 – PDF Password Security Assessment
- M3 – Database Discovery
- M4 – Final Penetration Testing Report

## Methodology

### M1 – Initial Access

A SQL Injection vulnerability was identified in the authentication
functionality of the training application.

The vulnerability was used to demonstrate authentication bypass
within the authorized environment.

Following successful access, three protected PDF lab reports were
retrieved.
<img width="1920" height="982" alt="login" src="https://github.com/user-attachments/assets/fda43a64-5df3-4ddd-b06e-dd7a22b59f26" />


### M2 – PDF Password Security Assessment

The three retrieved PDF files were protected with passwords.

The provided Hash Calculator was used to generate the required PDF
hash information.

The provided Password Cracker was then used to perform the controlled
password-security assessment.

All three PDF passwords were successfully recovered during the
exercise.
<img width="1920" height="982" alt="pdf1" src="https://github.com/user-attachments/assets/1de3b270-7c57-4d53-873a-99879b12e886" />
<img width="1920" height="982" alt="pdf1_pass" src="https://github.com/user-attachments/assets/b93ed2c4-c170-41c8-a24c-9b6956e739ce" />
<img width="1920" height="982" alt="pdf2" src="https://github.com/user-attachments/assets/4691dd81-ff81-4e96-a41a-773ab6b94210" />
<img width="1920" height="982" alt="pdf2_pass" src="https://github.com/user-attachments/assets/4bd744cf-67f1-41f8-8013-01ca53146111" />
<img width="1920" height="982" alt="pdf3" src="https://github.com/user-attachments/assets/c6438c55-baec-4313-893d-75c878595f68" />
<img width="1920" height="982" alt="pdf3_pass" src="https://github.com/user-attachments/assets/6db47b4e-0a8b-458e-a853-e366b4c1806b" />


### M3 – Database Discovery

A database backup was discovered within the authorized training
environment.

The database information was reviewed to identify the required
staff and shareholder information.

The relevant results were documented separately in the M3 Excel
evidence file.
<img width="911" height="291" alt="M3-share-holders" src="https://github.com/user-attachments/assets/5b38c237-8100-4472-a0af-a0e0af4cd437" />

### M4 – Final Report

A professional penetration testing report was prepared containing:

- Scope
- Methodology
- Findings
- Impact
- Recommendations
- Evidence
- Conclusion

## Tools Used

- Kali Linux
- gobuster
- Network Walks Hash Calculator
- Network Walks Password Cracker
- Web Browser

## Project Status

| Milestone | Description | Status |
|-----------|-------------|--------|
| M1 | SQL Injection & Initial Access | Completed |
| M2 | PDF Password Assessment | Completed |
| M3 | Database Discovery | Completed |
| M4 | Final Report | Completed |

## Disclaimer

This assessment was performed only against an authorized training
environment for educational purposes.

No unauthorized systems should be tested using the techniques
described in this repository.
[MEDIROZA_FINAL_PENETRATION_TESTING_REPORT.docx](https://github.com/user-attachments/files/31920049/MEDIROZA_FINAL_PENETRATION_TESTING_REPORT.docx)

