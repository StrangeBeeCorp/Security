# SB-SEC-ADV-2022-001: Authentication bypass due to incomplete checks in the Active Directory authentication module

**Date**: June 29, 2022
**Version**: 1.1
**Last update**: version of Cortex has been updated


Przemysław Mazurek reported a critical vulnerability in the Active Directory (AD) authentication module of TheHive.

Exploiting the vulnerability is only possible if the configured AD is on premise. When exploited, this vulnerability allows impersonating any account on the platform, including administrators. After investigations, we confirmed the issue and fixed it.

If your Active Directory authentication module is not enabled nor configured, or if you are using Azure AD, you are **NOT** at risk.

## Description
TheHive has an authentication vulnerability when the Active Directory module is enabled and used to authenticate users on the platform. 

Active Directory accepts connections as anonymous; if you do provide a username and an empty password while sending an authentication request to Active Directory, then you're authenticated as anonymous.

And that's how TheHive falls vulnerable: by sending an authentication request for an existing account without passwords through TheHive API, the Active Directory response to the request is "Success" and fools TheHive which accepts the user authentication.

This vulnerability also exists in Cortex, the exploitation process is similar and leads to same consequences.

## Affected versions, mitigation and resolution
This vulnerability affects TheHive from versions 3 to 5, and Cortex 3 as well. **We strongly recommend everyone to update to the latest versions available** that fix the vulnerability:
 
* TheHive ≥ 5.0.8;
* TheHive ≥ 4.1.21;
* Cortex ≥ 3.1.6;
* For remaining users of TheHive 3 (Already in EOL since December 31st, 2021), we exceptionally released TheHive 3.5.2 that fixes this vulnerability on this version as well.

If you are unable to update affected products, disabling the Active Directory authentication module prevents the vulnerability exploitation. Be careful to have local accounts enabled before disabling the AD authentication module to prevent locking yourself out of the platform.

CVE creation is in progress.

## Support
If you have any question about this security notice:
* Contact our support service if you are already a customer
* Or send us an email at [security@strangebee.com](mailto:security@strangebee.com)
