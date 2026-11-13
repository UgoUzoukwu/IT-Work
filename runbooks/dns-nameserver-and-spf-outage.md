# DNS outage: nameservers and SPF record restored

| | |
| --- | --- |
| **Area** | Public DNS, email authentication |
| **Date** | July 2026 |
| **Impact** | [FILL IN: what stopped working, for whom (staff and external clients), and for how long] |

## Symptom

[FILL IN: how the outage was first noticed, e.g. website unreachable, inbound or outbound mail failing, bounce messages mentioning SPF]

## Environment

- Public DNS zone for the organization's domain at [FILL IN: "a third-party DNS host" or "the registrar"; do not name the domain]
- Microsoft 365 (Exchange Online) for email

## Cause

[FILL IN: what happened to the nameserver delegation and the SPF record, and why (expired service, accidental change, provider issue)]

How it was diagnosed:

- [FILL IN: the checks you ran, e.g. `nslookup -type=ns`, `nslookup -type=txt`, an external DNS propagation checker, message trace in Exchange Online]

## Fix

1. Restored the correct nameservers for the domain. [FILL IN: where and how]
2. Restored the SPF TXT record. [FILL IN: the record's structure with the domain removed, e.g. `v=spf1 include:... -all`]
3. [FILL IN: anything else restored, e.g. MX, autodiscover, DKIM records]

## Verify

- [FILL IN: nameserver and TXT lookups returning the expected values from an outside resolver]
- [FILL IN: test email sent and received, SPF result shown as pass in the message headers]

## Prevention

- [FILL IN: e.g. exported a copy of the DNS zone, documented the records, added monitoring or renewal reminders]

## References

- [FILL IN: documentation used]
