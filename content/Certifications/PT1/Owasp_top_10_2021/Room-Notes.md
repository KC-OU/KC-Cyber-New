---
date: '2025-05-29T10:42:17-04:00'
draft: false
title: 'OWASP Top 10 - 2021 - Notes'
description: Learn about and exploit each of the OWASP Top 10 vulnerabilities; the 10 most critical web security risks.
categories:
  - "TryHackMe"
  - "OWASP"
  - "posts"
tags:
  - "OWASP"
  - "PT1"
toc: false
---
Learn about and exploit each of the OWASP Top 10 vulnerabilities; the 10 most critical web security risks.

## OWASP Top 10 - 2021 - Notes


This room will cover:

![OWASP](/images/owasp.png#floatright)

1. Broken Access Control
2. Cryptographic Failures
3. Injection
4. Insecure Design
5. Security Misconfiguration
6. Vulnerable and Outdated Components
7. Indentification and Authentication Failures
8. Software and Data Integrity Failures
9. Security Logging & Monitoring Failures
10. Server-side Regurest Forgery (SSRF)
 
## 1. Broken Access Control
Most websites have admin only sections like shops, portals and more. If a vistor acesses a admin only page or section, without **permission** is called broken access.

A regular vistor, who has regular acesss to protected pages can lead to the following:

- being able to view **sensitive information** from other users
- Accessing **unauthorised** functionality 

Simply put, Broken Access controls allows attackers to bypass **Authorisation**, but allows them access to **sensitive data**, like bank details, personal information or Proforming tasks that they are not allow to do. 

### Insecure Direct Object Referances

IDOR or Insecure Direct Object referance refers to an access to control **vulunabilites** were you can access resources you wouldn't ordinarily be able to see.

This occurs when the programmer exposses a Direct Object Referances which is jusr a identifier that refers to specific objects within the server by object, we could mean a file, a user, a bank account in a banking application, or anything really.