# SB-SEC-ADV-2025-002: Server-Side Request Forgery

**Date**: May 14, 2025

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Information disclosure

| Base score  | Vector          |
| :--------------- |:---------------|
| 4.6  | [CVSS:4.0/AV:N/AC:L/AT:N/PR:H/UI:A/VC:L/VI:N/VA:N/SC:N/SI:N/SA:N](https://www.first.org/cvss/calculator/4-0#CVSS:4.0/AV:N/AC:L/AT:N/PR:H/UI:A/VC:L/VI:N/VA:N/SC:N/SI:N/SA:N) |

---

## Executive summary

A vulnerability allows an authenticated, privileged remote attacker to perform a server-side request forgery (SSRF) attack against TheHive.

## Detailed description

An authenticated attacker with admin permissions allowing them to access specific API endpoints can manipulate URLs to direct requests to unexpected hosts or ports. This allows the attacker to use TheHive server as a proxy to reach internal or otherwise restricted resources. The vulnerability could be exploited to access other servers on the internal network.

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