# SB-SEC-ADV-2025-004: Broken Access Control

**Date**: May 14, 2025

**Version**: 1.0

**Last update**: Initial advisory

**Severity**: Medium

**Risks**: Disclosure of case-related information

---

## Executive summary

A broken access control vulnerability was identified in one of TheHive’s API endpoints.

## Detailed description

A remote, authenticated, and unprivileged user can exploit a specific endpoint to retrieve alerts, cases, logs, observables, or tasks by ID—bypassing standard access controls and retrieving data regardless of their assigned permissions.

## Impacted versions and resolution

Affected versions:

* TheHive versions 5.2.0 to 5.2.15
* TheHive versions 5.3.0 to 5.3.10
* TheHive versions 5.4.0 to 5.4.9

## Recommended action

We recommend that all users upgrade to one of the following versions, which include the necessary fixes for this vulnerability:

* TheHive version 5.2.16 or higher
* TheHive version 5.3.11 or higher
* TheHive version 5.4.10 or higher

## Support and contact information

For further inquiries or assistance regarding this security notice:

* Existing customers should contact our support team.
* Others may reach us at security@strangebee.com.