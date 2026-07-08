# Suspicious IP Review - Basic Triage Notes

This document contains basic learning notes for reviewing an alert or event involving a suspicious IP address.

The example is generic and does not contain real company data, user data, or production logs.

## Scenario

A security alert or log entry contains an IP address that requires review.

The goal of the first review is to understand whether the IP address is expected, unknown, suspicious, or related to potentially malicious activity.

## Initial Questions

- What IP address is involved?
- Is the IP address internal or external?
- Which user, host, or system communicated with this IP?
- When did the activity happen?
- What type of activity was observed?
- Was the connection inbound or outbound?
- Is this IP address expected for the user, host, or service?
- Are there repeated connections to or from this IP?

## Basic Context to Collect

- Source IP address:
- Destination IP address:
- Source hostname:
- Destination hostname:
- User account:
- Timestamp:
- Protocol or port:
- Alert source:
- Related events:

## Indicators to Review

Possible indicators that may increase suspicion:

- Unknown external IP address
- Repeated connections in a short period of time
- Connection to an unusual country or region
- Connection outside normal working hours
- Communication with uncommon ports
- Multiple internal hosts communicating with the same IP
- IP address reported by threat intelligence sources
- Failed login attempts from the same IP address

## Initial Assessment

### Likely Low Severity

The activity may be low severity if:

- The IP address is expected
- The destination service is known
- The activity matches normal business use
- There are no repeated or related suspicious events

### Possible Medium Severity

The activity may be medium severity if:

- The IP address is unknown
- The activity is unusual for the user or host
- There are repeated connections
- The IP appears in more than one alert

### Possible High Severity

The activity may be high severity if:

- The IP address is known for malicious activity
- Multiple internal hosts are involved
- The activity suggests possible command and control communication
- The activity is linked to malware, phishing, or account compromise
- There is evidence of data exfiltration or unauthorized access

## Documentation Template

When documenting this review, record:

- IP address:
- Internal or external:
- Related user:
- Related host:
- Date and time:
- Type of activity:
- Related alerts:
- Initial severity:
- Summary:
- Recommended next steps:

## Possible Next Steps

- Review related firewall, proxy, DNS, or authentication logs
- Check whether the IP is expected for a known service
- Search for other internal hosts communicating with the same IP
- Review the timeline of activity
- Check whether the user or system behavior is expected
- Escalate if the IP appears malicious or the activity suggests compromise

## Example Summary

An IP address was identified during basic alert review. The activity should be checked against related logs, affected hosts, and expected business activity before deciding whether escalation is required.
