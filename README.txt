TEAM OCTAESPORTS MOBILE APP — STARTER PROTOTYPE

WHAT IS INCLUDED
- Mobile-first black/red Octa-themed app UI
- Home dashboard, Scrims, Live Tracker, Team roster and Admin demo screens
- Sample free and paid scrims
- Admin demo can add sample events and update a sample match
- Local browser storage and basic PWA manifest/service worker

IMPORTANT LIMITATIONS
This is a FRONT-END PROTOTYPE. It does not have a secure admin login, shared database, real player registrations, payment collection, notifications, or a BGMI live-data integration. Data edited in Admin is saved only in the same browser/device. Do not use it to collect real payments or private room details.

HOW TO PREVIEW
1. Extract the ZIP.
2. Open index.html in a browser. Most UI works locally.
3. For install/PWA testing, serve the folder over HTTPS or localhost; service worker support is restricted for file:// URLs.

NEXT DEVELOPMENT PHASE BEFORE PUBLIC LAUNCH
1. Connect Firebase/Supabase (authentication, database, access rules).
2. Add a secure owner/admin role; never trust a hidden button as security.
3. Add server-side scrim registrations, slot limits, cancellation rules and notifications.
4. Add score entry + audit history and tournament leaderboard.
5. Decide lawful, Play-compliant handling of paid-entry scrims before adding payments or prize payouts.
6. Add privacy policy, support contact, account/data deletion process if accounts are created, app icons and store screenshots.
7. Package as an Android app with Capacitor or a native framework; generate a signed Android App Bundle (.aab) and test on real devices.

SUGGESTED ANDROID PACKAGING (requires Node.js and Android Studio)
- Install Node.js LTS and Android Studio.
- Create a Capacitor project following current official docs: https://capacitorjs.com/docs
- Copy the web app files into the configured web assets folder.
- Add Android platform, open in Android Studio, set app id such as com.octaesports.app, set icons/splash screen, test permissions and back navigation.
- Build a signed Android App Bundle (.aab) for Google Play. Exact commands can change by Capacitor version; follow its current Android guide.

This ZIP does not contain an APK or a Play-ready signed AAB.


TEAM ENROLLMENT FORM UPDATE
- Added an Enroll tab for outside teams to enter team name, owner real name/IGN, team email, player real names, BGMI IGNs, BGMI IDs, UIDs and screenshot proof files for four players plus an optional substitute.
- Important: the form is UI-only. It intentionally does not upload or save personal details/screenshots. Before collecting real submissions, connect a secure backend (e.g. Firebase/Supabase free tier), restrict admin access, store proof images privately, set retention/deletion rules, and publish a privacy notice.

ZERO-COST PUBLISHING REALITY
- Hosting the web app as a website/PWA on GitHub Pages can be free (use a public repository and github.io address).
- Publishing on Google Play is not free: Google currently charges a one-time US$25 Play Console registration fee, and new personal accounts have testing/verification requirements. If spending must be exactly zero, use the free website/PWA route and let Android users install it from the browser; it will not be listed in the Play Store.
