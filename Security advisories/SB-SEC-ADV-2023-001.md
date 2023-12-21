# SB-SEC-ADV-2023-001: Reporting – Stored Cross-Site Scripting

**Date**: 19 December, 2023

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Session hijacking / Privilege escalation

**CVE**: In progress

---

## Executive Summary

A vulnerability has been detected within the reporting module of TheHive. This flaw, when exploited, poses a risk as it allows for the impersonation of any user account, including those with administrative privileges. The exploit is viable through an authenticated user account.

## Detailed Description

This vulnerability is categorized as a stored Cross-Site Scripting (XSS) issue. Stored XSS vulnerabilities enable an attacker to embed malicious JavaScript or HTML code into a trusted web application. In this instance, the vulnerability is present within the case reporting functionality of TheHive. Malicious JavaScript code can be inserted into a report template or its variables, which, when executed, impacts the integrity of the application. Such execution can lead to unauthorized actions being performed on the application, including modification of user permissions.

## Impacted Versions and Resolution

Affected Versions:
* TheHive versions 5.2.0 to 5.2.8

## Recommended Action

Immediate update to TheHive version 5.2.9 or higher is strongly advised to remediate this vulnerability.

The process for the CVE assignment is ongoing.

## Acknowledgments

We extend our gratitude to [Randorisec](https://randorisec.com) for their meticulous penetration testing services. Their expertise has significantly contributed to strengthening our cybersecurity measures.

## Support and Contact Information

For further inquiries or assistance regarding this security notice:
* Existing customers are encouraged to contact our support service.
* Others may reach out via email at security@strangebee.com.
