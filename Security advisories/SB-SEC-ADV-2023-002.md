# SB-SEC-ADV-2023-002: Stored Cross-Site Scripting in TheHive's Attachment Functionality
 
**Date**: 25 January, 2024

**Version**: 1.1

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Session Hijacking / Privilege Escalation

**CVE**: [CVE-2024-22876](https://nvd.nist.gov/vuln/detail/CVE-2024-22876)

---

## Executive Summary

A vulnerability has been detected in TheHive's case attachment functionality. This issue, when exploited, can manipulate a victim account to perform unintended actions within the application, such as elevating the privileges of another user.

## Detailed Description

This vulnerability is a type of stored Cross-Site Scripting (XSS), a web security loophole that permits an attacker to insert malicious JavaScript or HTML code into a reputable web application. The vulnerability specifically affects the attachment preview feature. It allows an attacker to upload a malicious HTML file containing JavaScript code. When accessed through a specific URL, this code executes within the context of TheHive application, potentially leading to unauthorized administrative changes or other significant actions.

## Impacted Versions and Resolution

Affected Versions:
* TheHive versions 5.1.0 to 5.1.9
* TheHive versions 5.2.0 to 5.2.8

## Recommended Action

We urge all users to promptly upgrade to the following versions that contain the necessary fixes for this vulnerability:
* TheHive version 5.2.9 or higher
* TheHive version 5.1.10 or higher

## Acknowledgments

We extend our gratitude to [Randorisec](https://randorisec.com) for their meticulous penetration testing services. Their expertise has significantly contributed to strengthening our cybersecurity measures.

## Support and Contact Information

For further inquiries or assistance regarding this security notice:
* Existing customers are encouraged to contact our support service.
* Others may reach out via email at security@strangebee.com.
