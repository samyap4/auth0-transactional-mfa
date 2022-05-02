# auth0-transactional-mfa

This repo is leveraging the ability to perform step-up authentication with Auth0 from the front end.  The user can sign in with just their UN/PW to be granted access to their account.  When performing a sensitive operation, in this case transfering their balance, we will force the user to authenticate with a second factor without providing that UN/PW again.  This app leverages doing this from the front end by inspecting the ID token for whether the user has used MFA to login.  This can also be accomplished from the back-end by requesting a specific scope on the access token to force a second factor challenge.

You can read more about this here:
https://auth0.com/docs/secure/multi-factor-authentication/step-up-authentication/configure-step-up-authentication-for-web-apps
https://auth0.com/docs/secure/multi-factor-authentication/step-up-authentication/configure-step-up-authentication-for-apis

