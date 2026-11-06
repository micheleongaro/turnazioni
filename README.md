# turnazioni

Calendario turni del reparto Operation.

- **Sito:** https://micheleongaro.github.io/turnazioni/ (serve la password del sito)
- **Aggiornamento:** https://micheleongaro.github.io/turnazioni/aggiorna.html (serve la password di caricamento)

I turni sono cifrati (AES-256-GCM, chiave derivata dalla password con PBKDF2-SHA256): senza password il sito non mostra nomi né turni. Il repository contiene solo pagine cifrate, mai il file Excel.

## Come aggiornare il sito

1. Apri il file Excel dei turni (quello con il foglio **Dati**) in Excel, controlla che sia aggiornato e **salvalo**.
2. Apri la pagina **aggiorna.html** e inserisci la password di caricamento.
3. Trascina il file Excel nella pagina. Controlla il riepilogo (anno, persone, ultimo giorno con turni).
4. Premi **Scarica index.html**.
5. Qui su GitHub: **Add file → Upload files**, trascina `index.html`, premi **Commit changes**.
6. Dopo 1–2 minuti il sito mostra i nuovi turni.

Non caricare mai il file `.xlsx` in questo repository: è pubblico e il file contiene ferie e assenze in chiaro.

## Chi può aggiornare

Solo gli account GitHub aggiunti in **Settings → Collaborators**.
