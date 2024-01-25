# SB-SEC-ADV-2023-004: MFA Authentication Vulnerability Due to Lack of Lockout Policy in TheHive
 
**Date**: 25 January, 2024

**Version**: 1.1

**Last update**: Initial advisory

**Severity**: Low

**Risks**: Account Compromise
 
---

## Executive Summary

We have identified a security vulnerability in the Multi-Factor Authentication (MFA) functionality of TheHive. Notably, the system does not implement an account lockout mechanism after multiple incorrect MFA code submissions during authentication.

## Detailed Description

This vulnerability exists within the MFA system when used in conjunction with password-based authentication providers (local, LDAP, AD, etc.). An attacker, who has acquired compromised credentials of a legitimate account, can initiate a brute-force attack against the MFA code. Due to the absence of an account lockout policy, the application does not prevent an attacker from making repeated attempts to enter the correct MFA code, thereby increasing the risk of unauthorized access.

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