# Mobile Firebase Authentication Starter

An attributed React Native/Expo starter demonstrating email/password registration, login, persisted Firebase sessions, and authenticated navigation.

## Included flow

```text
app start -> loading screen -> existing Firebase session?
                              | yes -> home
                              ` no  -> login / registration
```

The repository includes validation and Firebase-error helpers with Jest tests, plus screens for loading, login, registration, and the authenticated home state.

## Local setup

Create a Firebase project, enable email/password authentication, and replace the placeholder configuration in `src/firebase/config.js` with local project settings.

```bash
npm install
npx expo start
```

Run utility tests with:

```bash
npm test
```

## Attribution and boundaries

This repository is based on a React Native Firebase starter rather than presented as a from-scratch product. The upstream promotional image is illustrative and is not proof of this copy's current runtime state.

- Firebase configuration is bundled client-side by design; access must be controlled with Firebase Authentication and security rules.
- The repository does not demonstrate production Firestore rules, account recovery, email verification, or abuse controls.
