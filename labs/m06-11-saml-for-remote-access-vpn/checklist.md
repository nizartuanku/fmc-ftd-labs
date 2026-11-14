# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The SSO server object matches the IdP metadata (entity ID, SSO URL, certificate).
- [ ] The base URL matches what users actually reach.
- [ ] IdP and device certificates are valid and expiry dates are tracked.
- [ ] NTP is synchronized on the threat defense.
- [ ] A test login with Secure Client succeeds and `show vpn-sessiondb anyconnect` shows the session.
