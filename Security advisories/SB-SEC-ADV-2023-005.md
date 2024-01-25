# SB-SEC-ADV-2023-005: Username Enumeration Vulnerability in TheHive
 
**Date**: 25 January, 2024

**Version**: 1.1

**Last update**: Initial advisory

**Severity**: Low

**Risks**: Information disclosure

---

## Executive Summary

A notable vulnerability has been identified in TheHive's authentication module. This flaw potentially enables attackers to list and identify registered users on the platform. It is pertinent to note that this issue is exclusive to instances utilizing local authentication.

## Detailed Description

This vulnerability manifests when local authentication is enabled. It allows an attacker to discern the existence of valid user accounts based on differential response times during authentication processes, including password reset requests. Specifically, the application's response time varies, inadvertently indicating whether a user account is legitimate.

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
