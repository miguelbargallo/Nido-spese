# NIDO — Spese di casa

NIDO V1 è una web app mobile-first per controllare esclusivamente le spese domestiche.

## Stack
- Vite + JavaScript
- Firebase Authentication (email/password)
- Cloud Firestore
- Netlify

## Sviluppo
Copia `.env.example` in `.env` e inserisci le variabili Firebase, poi:

```bash
npm install
npm run dev
```

## Build
`npm run build` produce `dist/`.

Le variabili Firebase sono pubbliche di natura client-side, ma non vengono hardcodate nel repository: usa le environment variables locali/Netlify.
