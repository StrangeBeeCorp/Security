# SB-SEC-ADV-2024-001: Username Enumeration Vulnerability in TheHive

**Date**: 30 April, 2024

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Low

**Risks**: Information disclosure

---

## Executive Summary

A notable vulnerability has been identified in TheHive's authentication module. This flaw potentially enables attackers to list and identify registered users on the platform. It is pertinent to note that this issue is exclusive to instances utilizing local authentication.

## Detailed Description

This vulnerability manifests when local authentication is enabled. It allows an attacker to discern the existence of valid user accounts based on differential response during authentication processes when the sent password is empty.

## Impacted Versions and Resolution

Affected Versions:
* TheHive versions 5.1.0 to 5.1.10
* TheHive versions 5.2.0 to 5.2.12

## Recommended Action

We recommend all users to upgrade to the following versions that contain the necessary fixes for this vulnerability:
* TheHive version 5.2.13 or higher
* TheHive version 5.1.11 or higher

## Acknowledgments

We extend our heartfelt thanks to [Lap1nou](https://github.com/lap1nou) (@lapinousexy) from Orange Cyberdefense for his responsible reporting of the vulnerability, in alignment with our [Responsible Vulnerability Disclosure Policy](https://github.com/StrangeBeeCorp/Security/blob/main/Policies/Vulnerability%20Disclosure%20policy.md). We are deeply appreciative of his contribution to enhancing the safety and integrity of our systems.

## Support and Contact Information

For further inquiries or assistance regarding this security notice:
* Existing customers are encouraged to contact our support service.
* Others may reach out via email at security@strangebee.com.
