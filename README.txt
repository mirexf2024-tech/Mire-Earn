MIRE EARN — GITHUB PAGES STARTER
================================

FILES
- index.html: existing landing page style preserved; founder photo replaces the hero illustration.
- assets/founder-photo.png: supplied portrait photo.
- firebase-config.js: paste your MIRE EARN Firebase Web App config here.
- firestore.rules: restrictive starter rules for user profiles, task submissions, withdrawals, tasks.

IMPORTANT STATUS
This package connects Firebase Email/Password registration/login, Google sign-in (if enabled), password reset, profile creation, and profile balance display. It does NOT yet provide a real paid task provider, real ad revenue, automated Telebirr/CBE payouts, or a secure admin approval backend. No real rewards should be promised or paid from placeholder tasks. Wallet balance is read from Firestore and cannot be edited by a normal member under the included rules.

SETUP
1. Open Firebase Console and select the MIRE EARN project (project ID mifu-b6c97 if that is the project you intend to use).
2. Authentication > Sign-in method: enable Email/Password. Enable Google only if you want Google sign-in.
3. Authentication > Settings > Authorized domains: add your exact GitHub Pages domain.
4. Project settings > Your apps > Web app: copy firebaseConfig into firebase-config.js, replacing PASTE_VALUE entries. Do not paste service-account private keys anywhere in this site.
5. Firestore Database: create the database if not already created; publish firestore.rules.
6. Upload index.html, firebase-config.js, firestore.rules, and assets/ to the repository root using the same folder layout. GitHub Pages must serve index.html from the selected branch/root.
7. Test account creation, email/password login, password reset, and sign-out using a test account.

NOT YET READY FOR PUBLIC PAYMENTS
A production earning platform still needs a trusted backend (for task verification, referral abuse prevention, admin claims, ledger transactions and withdrawal approval), a real revenue/task provider, and an approved payment-provider integration. Never let browser code directly add to a user's wallet balance. Do not use invented statistics or sample rewards as real earnings.
