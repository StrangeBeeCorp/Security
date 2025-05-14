# SB-SEC-ADV-2025-003: Email Bombing Through Password Reset API Feature

**Date**: May 14, 2025

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Capacities exhaustion, loss of reputation of SMTP server

---

## Executive summary

The password reset API feature can be abused.

## Detailed description

An unauthenticated remote attacker can abuse the password reset feature to trigger unlimited password reset emails to legitimate users. This vulnerability can lead to several consequences, including:

* Mailbox storage exhaustion for targeted users
* Reputation damage to the SMTP server, potentially causing it to be blacklisted
* Overload of the SMTP server’s outbound mail queue

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