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

### M2 – PDF Password Security Assessment

The three retrieved PDF files were protected with passwords.

The provided Hash Calculator was used to generate the required PDF
hash information.

The provided Password Cracker was then used to perform the controlled
password-security assessment.

All three PDF passwords were successfully recovered during the
exercise.

### M3 – Database Discovery

A database backup was discovered within the authorized training
environment.

The database information was reviewed to identify the required
staff and shareholder information.

The relevant results were documented separately in the M3 Excel
evidence file.

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
