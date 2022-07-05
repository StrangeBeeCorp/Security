# SB-SEC-ADV-2022-002: Unauthentified API endpoint leaking data

**Date**: July 4, 2022

**Version**: 1.0

---

Rayen Messaoudi reported us a critical vulnerability in a TheHive API endpoint.

The API endpoint is leaking information about the ongoing events in TheHive. An attacker exploiting the vulnerability will be able to get all the details of current activities in TheHive (creation, modification, deletion of any object).

This endpoint is accessible without authentication.

## Description
TheHive API has a weak endpoint which is accessible without authentication that can be exploited to listen current events. 

Once exploited, the API endpoint provides details of ongoing events. The events can be of any nature (creation, modification, deletion) and concern every entities _(Cases, Alerts, Observables, Tasks, Jobs...)_. 

The vulnerability is not exploited in the wild.

## Affected versions, mitigation and resolution
This vulnerability affects TheHive from versions 4 to 5. We strongly recommend everyone to update to the latest versions available that fix the vulnerability:

* TheHive ≥ 5.0.9;
* TheHive ≥ 4.1.22;

CVE creation is in progress.

## Support

If you have any question about this security notice:

* Contact our support service if you are already a customer
* Or send us an email at [security@strangebee.com](mailto:security@strangebee.com). 
