# YT Creator Hindi Android Starter

## Included
- Native Android WebView wrapper
- Responsive course-app prototype bundled in `app/src/main/assets/index.html`
- Home, courses, progress, pricing, demo OTP, demo coupons, admin preview
- GitHub Actions workflow that builds a **debug APK** after you upload this project to your own GitHub repository

## Build APK using GitHub Actions (phone-friendly, but requires a GitHub account)
1. Extract the ZIP.
2. Create a new repository on GitHub.
3. Upload the **contents of this `android-wrapper` folder** to the repository root (not the outer folder).
4. Open the repository's **Actions** tab and run **Build Android APK** (or wait for the workflow after pushing to `main`).
5. Open the completed workflow run, go to **Artifacts**, and download `YT-Creator-Hindi-debug-apk`.
6. Extract the artifact ZIP; it contains `app-debug.apk`. Install only on your own device after reviewing Android's install warning.

## Important
This produces a test/debug APK, not a Play Store release-signed APK. No hosted public website is created by this workflow.

### Live services are not implemented
- Phone OTP: the UI is a demo; it does not send SMS.
- Payments: buttons are demo-only; no money is charged.
- Coupons/admin: browser-local demo data only; not secure and not shared between users.
- Course video/photo content: sample interface only; add your own licensed assets and hosted video links.
- Production requires secure backend, Firebase/SMS setup, payment-gateway account and server-side signature/webhook validation, role-protected admin, privacy/terms/refund policies, and proper testing.
- Requested pricing shown: ₹19 for 7-day access and ₹199 per month. Do not enable auto-renewal without clear consent and transparent terms.
