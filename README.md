# NIDO — Spese di casa

NIDO V1 è una web app mobile-first per controllare esclusivamente le spese domestiche.

## Stack
- Vite + JavaScript
- Firebase Authentication (email/password)
- Cloud Firestore
- Netlify

## Sviluppo
Copia `.env.example` in `.env` e inserisci le variabili Firebase, poi `npm install` e `npm run dev`.

## Build
`npm run build` produce `dist/`.

## Firebase
Abilita Email/Password in Firebase Authentication e pubblica `firestore.rules` nel progetto `latorre-eaa29`. Tutti i documenti sono isolati sotto `users/{uid}` e le regole consentono accesso solo al relativo utente autenticato.

## Netlify
`netlify.toml` imposta `npm run build`, publish `dist` e il rewrite SPA. Le variabili `VITE_FIREBASE_*` vanno configurate nelle environment variables di Netlify; non inserire segreti o service account nel repository.
