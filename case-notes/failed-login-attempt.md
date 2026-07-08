# Failed Login Attempt - Basic Triage Notes

This document contains basic learning notes for reviewing a failed login attempt alert.

The example is generic and does not contain real user data, company data, or production logs.

## Scenario

A security alert reports one or more failed login attempts against a user account.

The goal of the first review is to understand whether the activity looks like a simple user mistake, unusual behavior, or a possible security incident.

## Initial Questions

* Which user account was affected?
* When did the failed login attempt happen?
* How many failed attempts were observed?
* What was the source IP address?
* Was the login attempt internal or external?
* Is the affected account a normal user account or a privileged account?
* Did the same source IP attempt to log in to other accounts?
* Did the user successfully log in shortly after the failed attempt?

## Basic Indicators to Review

Possible indicators that may increase suspicion:

* Multiple failed login attempts in a short time
* Failed login attempts against a privileged account
* Login attempt from an unknown source IP address
* Activity outside normal working hours
* Failed attempts followed by a successful login
* Similar activity against multiple accounts
* Repeated failed login attempts from the same source

## Initial Assessment

### Likely Low Severity

The activity may be low severity if:

* There are only one or two failed attempts
* The user successfully logged in from a known device afterward
* The source IP is expected
* There are no repeated attempts or related alerts

### Possible Medium Severity

The activity may be medium severity if:

* There are multiple failed attempts
* The source IP is unusual
* The activity happened outside normal hours
* Similar attempts were seen against other accounts

### Possible High Severity

The activity may be high severity if:

* A privileged account is targeted
* Failed attempts are followed by a successful login
* The source IP is suspicious or known for malicious activity
* Multiple users are targeted
* There are signs of account compromise

## Documentation Template

When documenting this alert, record:

* Alert name:
* Date and time:
* Affected user:
* Source IP address:
* Target system:
* Number of failed attempts:
* Related successful login:
* Initial severity:
* Summary:
* Recommended next steps:

## Example Summary

Multiple failed login attempts were observed against a user account. The source IP address, number of attempts, affected account type, and any related successful login should be reviewed to determine whether the activity is expected or suspicious.

## Possible Next Steps

* Review authentication logs
* Check whether the user recognizes the activity
* Look for successful login after failed attempts
* Search for other accounts targeted by the same source IP
* Check whether the account has elevated privileges
* Escalate if there are signs of compromise
