# SafeCircle — Installable PWA

A functional browser-based SafeCircle prototype that can be installed on Android, iPhone (supported browsers), Windows and other PWA-capable platforms.

## Included
- Emergency SOS countdown and activation flow
- Trusted Circle contact management
- Safe Journey with expected-arrival tracking/check-in
- Community Alerts stored locally
- South African emergency call shortcuts
- Profile and privacy controls
- Current-location sharing using browser geolocation when permitted
- PWA manifest + service worker for installation/offline shell

## Run locally
A service worker requires HTTP(S), so do not open index.html directly with file://.

Option 1:
  python -m http.server 8080

Then open:
  http://localhost:8080

Option 2:
Deploy the folder to any HTTPS static host. HTTPS is required for browser geolocation and service-worker installation in normal production use.

## Important production work
This project is a working local PWA prototype. For a production safety service, add a secure backend for authenticated users, trusted-contact notifications (SMS/push), server-side emergency events, moderation/verification for community alerts, encrypted data handling, audit logs, abuse prevention, and verified emergency-service information. Do not represent a browser demo as an automatic emergency-dispatch system.
