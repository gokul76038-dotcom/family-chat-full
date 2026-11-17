FAMILY CHAT - FRESH SETUP (English app)

STEP 1 - Firebase (console.firebase.google.com)
  a) Build > Authentication > Get started > Sign-in method > Email/Password > Enable > Save
  b) Build > Firestore Database > Create database (production mode) > Rules tab > paste firestore.rules > Publish
  c) Build > Storage > Get started > Rules tab > paste storage.rules > Publish
     (Firebase may ask for the Blaze plan. Normal family use stays inside the free quota.)
  d) Project settings (gear icon) > Your apps > Add app > Web (</>) > Register app
     > copy the firebaseConfig values

STEP 2 - Edit www/firebase-config.js
  Replace every PASTE_HERE with your values. Keep the quotes.

STEP 3 - GitHub
  a) Create a NEW repository, set it to PRIVATE.
  b) Upload ALL files and folders from this package (www folder, package.json,
     capacitor.config.json, firestore.rules, storage.rules, README.txt).
  c) Make sure the folder .github/workflows/build.yml exists in the repo.
     If it is missing (hidden folders sometimes do not upload):
       Add file > Create new file > name it:  .github/workflows/build.yml
       Open BUILD-WORKFLOW.txt from this package, copy everything, paste it, Commit.

STEP 4 - Build the APK
  GitHub > Actions tab > "Build APK" runs automatically (5-10 minutes).
  When it shows a green tick, open it and download "family-chat-apk" from Artifacts.
  Unzip it to get app-debug.apk and install it on both phones.

STEP 5 - Use the app
  Each person taps "Create new account" and signs up with their own email and password.

  Keep the APK and the repository private.
