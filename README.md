# PokerRoll – gestione bankroll poker

App web installabile (PWA). I dati restano sul telefono di chi la usa: nessun server, nessun database, costo zero.

## File

- `index.html` – l'app completa
- `manifest.json` – nome e icona per l'installazione
- `sw.js` – funzionamento offline
- `icon-192.png`, `icon-512.png` – icone

## Pubblicazione (una volta sola)

1. Su GitHub crea un repository nuovo, per esempio `pokerroll`.
2. Carica i 5 file nella radice del repository (Add file → Upload files).
3. Su Vercel: Add New → Project → importa il repository → Deploy. Non serve configurare nulla.
4. Vercel ti dà un indirizzo tipo `https://pokerroll.vercel.app`: è il link da mandare agli amici.

## Aggiornamenti

1. Sostituisci i file su GitHub: Vercel ripubblica da solo.
2. In `sw.js` cambia `pokerroll-v1` in `pokerroll-v2` (poi v3, v4…) a ogni aggiornamento, così i telefoni scaricano la versione nuova.

I dati degli utenti non si perdono con gli aggiornamenti.

## Installazione sul telefono

- **Android (Chrome):** apri il link → menu ⋮ → "Installa app" o "Aggiungi a schermata Home".
- **iPhone (Safari):** apri il link → Condividi → "Aggiungi alla schermata Home".

## Da sapere

- I dati sono solo sul dispositivo: fare un backup periodico da Altro → Backup e dati.
- Per passare a un altro telefono: esporta il backup e importalo sul nuovo.
- Su iPhone l'app installata e Safari hanno dati separati: usare sempre l'icona sulla Home.
