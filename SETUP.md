# MoveTrack Multi-user setup

1. Create a Firebase project at the Firebase Console.
2. Add a Web app and copy its Firebase config.
3. In index.html replace the six PASTE_ values in firebaseConfig.
4. Firebase Console -> Authentication -> Sign-in method -> enable Email/Password.
5. Firebase Console -> Firestore Database -> Create database.
6. Firestore -> Rules: paste the contents of firestore.rules and publish.
7. Upload index.html, manifest.webmanifest, sw.js, icon.svg and firestore.rules to your GitHub repository root.
8. Open the GitHub Pages URL and create an account.

Each account gets its own UID, profile and daily history. The Firestore rules only allow a signed-in user to access documents under that user's UID.
Do NOT put a Firebase Admin SDK private key in this website.
