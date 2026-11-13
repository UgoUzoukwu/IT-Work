# Users signed out of a federated app every 90 minutes

| | |
| --- | --- |
| **Area** | Entra ID, SAML single sign-on |
| **Date** | [FILL IN: month and year] |
| **Impact** | [FILL IN: which group of users, how often they were interrupted] |

## Symptom

Users of a SAML-federated application were signed out about every 90 minutes and had to sign in again, even while actively working.

[FILL IN: what the user saw, e.g. redirect to sign-in page, an error message, lost unsaved work]

## Environment

- Entra ID as the identity provider, SAML SSO to a third-party application
- [FILL IN: type of application, without naming the vendor if that identifies the firm]

## Cause

The application ended its session after 90 minutes because the SAML response from Entra ID did not tell it how long the session should last.

[FILL IN: how you found this. Which logs or SAML trace did you look at, what did you rule out first (Conditional Access sign-in frequency, token lifetime policy, the app's own settings)?]

## Fix

Added a session timeout claim to the application's SAML configuration in Entra ID.

1. [FILL IN: where in the Entra admin center you made the change]
2. [FILL IN: the claim or attribute name and the value you set]
3. [FILL IN: any change needed on the application side]

## Verify

- [FILL IN: how you confirmed it, e.g. captured a new SAML response and checked the attribute, then watched a test session past 90 minutes]

## Prevention

- [FILL IN: e.g. added this check to the steps for onboarding a new SAML application]

## References

- [FILL IN: the Microsoft or vendor documentation you used]
