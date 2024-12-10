# BeFloral Security Report

## Overview
This project focuses on the security analysis of [BeFloral](https://github.com/exSnake/Befloral), an e-commerce web application designed for selling flowers. Developed as part of an academic exercise, the goal was to identify and evaluate potential security vulnerabilities that could compromise the system’s integrity, confidentiality, and availability.

The project involves testing critical areas of the application, including user authentication, product catalog management, and order processing, with an emphasis on identifying common web security vulnerabilities.

## Key Objectives
- Identify vulnerabilities that could affect BeFloral's security.
- Perform static, dynamic, and manual analyses to discover potential weaknesses.
- Focus on common security flaws such as:
  - SQL Injection
  - Cross-Site Scripting (XSS)
  - Cross-Site Request Forgery (CSRF)
  - Indirect Direct Object Reference (IDOR)
  - Client-Side Validation issues

## Tools Used
- **SpotBugs** for static code analysis.
- **ZAP** (**Zed Attack Proxy**) for dynamic analysis, including fuzzing and spidering techniques.
- Manual review of vulnerabilities to ensure reliability of results.

## Methodology
- **Static Analysis**: Using SpotBugs to inspect the code for common vulnerability patterns and potential security risks without executing the program.
- **Dynamic Analysis**: Utilizing ZAP to explore and test the web application in real-time, identifying vulnerabilities in execution.
- **Manual Analysis**: Reviewing critical areas of the application, especially those missed by automated tools, to uncover additional vulnerabilities.

## Key Findings
A total of 19 vulnerabilities were identified, of which 11 were confirmed as true positives. These included:
- **SQL Injection**: Vulnerabilities in the product sorting mechanism, exploitable with specially crafted queries.
- **XSS** (**Cross-Site Scripting**): Detected in the cart and review systems, allowing attackers to inject malicious scripts.
- **CSRF** (**Cross-Site Request Forgery**): Discovered in several API endpoints, lacking proper anti-CSRF tokens.
- **Client-Side Validation Bypass**: Bypassed security controls on user registration via client-side scripts.

## Conclusion
The BeFloral web application, while functional, was found to have several critical security vulnerabilities. These vulnerabilities, including SQL Injection and XSS, pose significant risks and would need remediation before the application could be used in a real-world environment.

This project highlights the importance of combining static, dynamic, and manual testing to thoroughly assess the security of a web application.

## Contacts

Matteo Beltrami - [matteo.beltrami-1@studenti.unitn.it](mailto:matteo.beltrami-1@studenti.unitn.it)

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/extras/dark.png">
    <img alt="https://www.unitn.it/" src="assets/extras/light.png" width="300px">
</picture>
