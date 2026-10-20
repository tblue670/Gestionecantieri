# Contabilità Cantieri

Web app in un solo file (`index.html`) per presenze, personale, paghe, incassi, spese, preventivi, report e foto dei cantieri, con assistente integrato in linguaggio naturale.

Versione: **v03.1**

## Cosa contiene

| File | A cosa serve |
|---|---|
| `index.html` | L'app completa |
| `manifest.webmanifest` | Nome e icona per installarla come app |
| `sw.js` | Apertura veloce e utilizzo senza rete |
| `icon-192.png`, `icon-512.png` | Icone dell'app |

## Pubblicare su GitHub Pages

1. Crea un repository su GitHub (nome a piacere, es. `cantieri`).
2. Carica tutti i file di questa cartella nella radice del repository (**Add file → Upload files**), poi **Commit changes**.
3. Vai in **Settings → Pages**. In **Build and deployment** scegli **Deploy from a branch**, ramo **main**, cartella **/ (root)**, poi **Save**.
4. Dopo uno o due minuti l'indirizzo compare nella stessa pagina: `https://TUONOME.github.io/NOME-REPOSITORY/`.
5. Aprilo con Chrome: dal menu scegli **Installa app** (oppure **Aggiungi a schermata Home**).

## Dati e riservatezza

- Il file non contiene nessun dato aziendale: parte vuoto.
- I dati inseriti restano **nel browser del dispositivo** in cui li inserisci, non su GitHub. Ogni dispositivo ha il suo archivio.
- Per spostare i dati tra dispositivi: **Dati → Scarica backup JSON**, poi sull'altro dispositivo **Dati → importa il file**.
- Con un repository pubblico chiunque conosca l'indirizzo può aprire l'app, ma vede solo i propri dati (vuoti).
- Per il backup automatico su una cartella di Google Drive e per le foto su cartella Drive serve Chrome su computer o Android.

## Aggiornare l'app

Sostituisci `index.html` con la nuova versione (**Add file → Upload files**, stesso nome, conferma la sostituzione). L'app installata si aggiorna alla riapertura, anche con due aperture se la versione precedente era in cache.

Se cambia anche `sw.js`, aumenta il numero nella riga `const CACHE` per forzare l'aggiornamento della cache.
