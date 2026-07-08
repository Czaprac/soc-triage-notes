# Basic Alert Triage Checklist

This checklist is a learning document for basic SOC alert triage practice.

It is intended to help structure the first review of a security alert in a clear and repeatable way.

## 1. Identify the Alert

Questions to answer:

* What is the alert name?
* When did the alert occur?
* Which user account is involved?
* Which host, IP address, or system is involved?
* What system or tool generated the alert?

## 2. Collect Basic Context

Check the following:

* Is the user account valid and known?
* Is the host or device known?
* Is the source IP internal or external?
* Is the activity expected for this user or system?
* Did similar alerts occur before?

## 3. Look for Suspicious Indicators

Examples of suspicious indicators:

* Multiple failed login attempts
* Login attempt from an unusual location
* Unknown or suspicious source IP address
* Activity outside normal working hours
* Repeated alerts from the same user or host
* Access attempts to unusual systems

## 4. Estimate Initial Severity

Use a simple initial classification:

### Low

The activity looks unusual, but there is limited evidence of malicious behavior.

### Medium

There are multiple suspicious indicators or repeated activity.

### High

There is strong evidence of malicious activity, compromise, or business impact.

## 5. Document the Findings

Record the following information:

* Alert name
* Date and time
* Affected user account
* Affected host or IP address
* Observed indicators
* Initial severity estimate
* Short summary of the activity
* Recommended next steps

## 6. Possible Next Steps

Depending on the alert, possible next steps may include:

* Review related logs
* Check user activity history
* Verify whether the activity was expected
* Search for repeated events
* Escalate to a senior analyst if needed
* Document the case clearly
