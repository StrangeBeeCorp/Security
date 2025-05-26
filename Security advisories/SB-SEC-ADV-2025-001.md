# SB-SEC-ADV-2025-001: Cross-Site Request Forgery

**CVE**: [CVE-2025-48740](https://nvd.nist.gov/vuln/detail/CVE-2025-48740)

**Date**: May 14, 2025

**Version**: 1.1

**Last update**: May 26, 2025

**Severity**: Medium

**Risks**: Privilege escalation, account compromise

| Base score  | Vector          |
| :--------------- |:---------------|
| 5.9  | [CVSS:4.0/AV:N/AC:L/AT:P/PR:N/UI:A/VC:N/VI:H/VA:N/SC:N/SI:N/SA:N](https://www.first.org/cvss/calculator/4-0#CVSS:4.0/AV:N/AC:L/AT:P/PR:N/UI:A/VC:N/VI:H/VA:N/SC:N/SI:N/SA:N) |

---

## Executive summary

A vulnerability allows an unauthenticated remote attacker to perform a cross-site request forgery (CSRF) attack against TheHive.

## Detailed description

When basic authentication is enabled in TheHive, an attacker who lures a privileged user into visiting a malicious webpage can trigger requests on their victim’s behalf, without them noticing it. For example, the attacker may forge requests to change an account’s password or increase an account’s privileges.

## Impacted versions and resolution

Affected versions:

* TheHive versions 5.2.0 to 5.2.15
* TheHive versions 5.3.0 to 5.3.10
* TheHive versions 5.4.0 to 5.4.9
* TheHive version 5.5.0

## Recommended action

We recommend that all users upgrade to one of the following versions, which include the necessary fixes for this vulnerability:

* TheHive version 5.2.16 or higher
* TheHive version 5.3.11 or higher
* TheHive version 5.4.10 or higher
* TheHive version 5.5.1 or higher

## Acknowledgments

We sincerely thank Jean-Michel Huguet from the NATO Cyber Security Center for responsibly reporting this
vulnerability in accordance with our [Responsible Vulnerability Disclosure Policy](https://github.com/StrangeBeeCorp/Security/blob/main/Policies/Vulnerability%20Disclosure%20policy.md). We are truly grateful for his contribution to improving the security of our product and helping protect our users.

## Support and contact information

For further inquiries or assistance regarding this security notice:

* Existing customers should contact our support team.
* Others may reach us at security@strangebee.com.