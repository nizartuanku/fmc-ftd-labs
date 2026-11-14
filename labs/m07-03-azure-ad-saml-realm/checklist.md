# Verification checklist

Work through this after Part 3 of the lab. Do not assume it works: confirm each item.

- [ ] Groups download from Entra ID into the realm, and `<TEST_GROUP>` is listed.
- [ ] The identity rule references the Microsoft Azure AD (SAML) realm and is deployed.
- [ ] A Decrypt - Resign rule exists for the users to be authenticated (active
      authentication / captive portal).
- [ ] A test user completes SSO and appears **by name** in the connection events.
- [ ] Rules exist for the special identities: Unknown, Failed Authentication, Guest and
      No Authentication Required.
- [ ] Certificates used by the SSO trust have not expired.
- [ ] You checked the platform user and group limits for your FMC/FTD model.

After Part 4 (break it on purpose):

- [ ] You saw the user classified as Unknown after the attribute change.
- [ ] After the fix, the user appears by name with their groups again.
