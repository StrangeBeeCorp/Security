# SB-SEC-ADV-2023-003: Reflected Cross-Site Scripting in TheHive's Branding Configuration
 
**Date**: 19 December, 2023

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Session Hijacking / Privilege escalation

**CVE**: In progress

---

## Executive Summary

A vulnerability has been discovered in the branding configuration functionality of TheHive. This issue, when exploited, enables the impersonation of any account on the platform, including those with administrative rights. It's important to note that exploitation is feasible only with a legitimate administrator account.

## Detailed Description

This vulnerability is classified as a stored Cross-Site Scripting (XSS) issue. Stored XSS vulnerabilities allow attackers to inject malicious JavaScript or HTML code into a trusted web application. In TheHive, administrators have the capability to customize the branding of the login page. The vulnerability arises due to the application's failure to validate the content type of uploaded files. A malicious administrator can exploit this by uploading an HTML file embedded with malicious JavaScript, and subsequently sharing the link to this corrupted branding logo.

## Impacted Versions and Resolution

Affected Versions:
* TheHive versions 5.1.0 to 5.1.9
* TheHive versions 5.2.0 to 5.2.8

## Recommended Action

We urge all users to promptly upgrade to the following versions that contain the necessary fixes for this vulnerability:
* TheHive version 5.2.9 or higher
* TheHive version 5.1.10 or higher

The process for the CVE assignment is ongoing.

## Acknowledgments

We extend our gratitude to [Randorisec](https://randorisec.com) for their meticulous penetration testing services. Their expertise has significantly contributed to strengthening our cybersecurity measures.

## Support and Contact Information

For further inquiries or assistance regarding this security notice:
* Existing customers are encouraged to contact our support service.
* Others may reach out via email at security@strangebee.com.

