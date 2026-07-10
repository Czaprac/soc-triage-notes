# Failed Login Alert - Example Notes

This is a fictional example created for learning purposes only.

It does not contain real user data, company data, or production logs.

## Alert Information

- Alert name: Multiple failed login attempts
- Alert source: Authentication logs
- Date and time: 2026-07-08 09:42
- Analyst: Łukasz Czapracki
- Initial severity: Medium

## Affected Assets

- User account: user.example
- Hostname: workstation-01
- IP address: 203.0.113.45
- Operating system: Windows
- Application or service: User login

## Alert Summary

Multiple failed login attempts were observed against a user account. The activity should be reviewed to determine whether it was caused by a user mistake, password issue, or possible unauthorized access attempt.

## Observed Indicators

- Several failed login attempts occurred in a short period of time.
- The source IP address was not confirmed as expected.
- The affected account was a normal user account, not a privileged account.
- No confirmed successful login was identified at this stage.

## Questions to Answer

- Does the user recognize the activity?
- Is the source IP address expected?
- Were there similar failed attempts against other accounts?
- Was there a successful login after the failed attempts?
- Did the activity happen during normal working hours?

## Initial Assessment

Medium

Reason for assessment:

The alert contains repeated failed login attempts and an unconfirmed source IP address. There is not enough evidence to confirm compromise, but the activity should be reviewed further.

## Recommended Next Steps

- Review related authentication logs.
- Check if the user recognizes the login attempts.
- Search for similar failed login attempts from the same source IP address.
- Check whether a successful login occurred after the failed attempts.
- Escalate if related suspicious activity is found.

## Final Notes

At this stage, the activity is suspicious but not confirmed as malicious. Further log review and user verification are recommended.
