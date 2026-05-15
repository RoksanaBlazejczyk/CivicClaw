# Resolver Notes

## Suspected Cause

Possible identity or authentication synchronisation delay between the password reset process and the School Learning Portal.

## Similar Past Incidents

Similar incidents were previously recorded as P2 and linked to identity synchronisation delays:

- INC-003: Multiple school staff unable to login after password reset.
- INC-006: Multiple schools reported login failures after password changes.
- INC-008: Several staff across two schools unable to login after password resets.

## Suggested Checks

1. Confirm whether the password reset system is operating normally.
2. Check whether account changes are synchronising correctly to the School Learning Portal.
3. Check authentication logs for repeated failed login attempts after successful password reset.
4. Confirm whether the issue is limited to Example Primary School or affects multiple schools.
5. Check whether there is any planned or unplanned maintenance affecting authentication services.
6. Review whether any recent change was made to identity, authentication or portal configuration.

## Escalation Recommendation

Escalate to the Identity team if more than one staff account is affected or if logs indicate delayed synchronisation.

## What Not To Do

- Do not close the incident until the login issue has been confirmed as resolved.
- Do not advise repeated password resets without checking synchronisation.
- Do not publish a public status update without human approval.
- Do not include personal data or pupil information in user-facing updates.

## Human Approval Points

Human approval is required before:

- Changing the live incident priority.
- Escalating to another team.
- Sending the user update.
- Publishing a service status update.
- Creating or updating a live knowledge base article.