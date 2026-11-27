# Calendario dell'Avvento

## Dove mettere il materiale
- `img/`   → un'immagine per giorno: `01.jpg`, `02.jpg` ... `24.jpg` (vanno bene anche .png / .webp)
- `audio/` → una canzone per giorno: `01.mp3`, `02.mp3` ... `24.mp3` (anche .m4a)
- `frasi.js` → la frase di ogni giorno (apri il file e scrivi il testo tra le virgolette)

Se per un giorno manca l'immagine o l'audio, quell'elemento semplicemente non compare.

## Tagliare le canzoni (ffmpeg)
Esempio: dal secondo 30, durata 45 s, mp3 a 128 kbps:
    ffmpeg -i originale.mp3 -ss 30 -t 45 -b:a 128k audio/05.mp3
In alternativa Audacity (Taglia, poi Esporta come MP3).

## Pubblicare su GitHub Pages
1. Crea un repository su GitHub e carica tutto il contenuto di questa cartella (con "Add file > Upload files" va bene).
2. Settings > Pages > "Deploy from a branch" > branch `main`, cartella `/ (root)` > Save.
3. Dopo un minuto il sito è su `https://TUOUTENTE.github.io/NOMEREPO/`

## Provare il sito prima di dicembre
Aggiungi `?test` all'indirizzo (es. `.../NOMEREPO/?test`): compare l'interruttore che sblocca tutte le caselle.
