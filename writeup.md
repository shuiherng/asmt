## Write-Up

This writeup answers both questions simultaneously.

From the extracted IOCs, we can cross-check the domains against known threat databases, whether it is in the form of a domain blacklist, or gathering data on the IP associated with the domain then checking against known blacklisted IPs.

Registrar names can also be used - for instance, if a threat is identified to be associated with a particular registrar, then other domains which are under this registrar are possibly new IOCs.

The whois data also includes a status code for the domain. Suspicious domains may have status codes which indicate that the domain is no longer valid, such as `serverHold`, which indicates that a DNS lookup will no longer function for this domain. These may be surfaced as potentially new IOCs as well.
