# Fantacalcio Viewer (GitHub Pages)

Viewer interattivo in singolo file HTML, mobile-friendly. Niente backend, nessuna installazione.

## 🚀 Pubblicazione su GitHub Pages (gratuita)

1. **Crea un nuovo repository** su GitHub (es. `fantacalcio-viewer`).  
2. Carica i file di questa cartella (`index.html`, `.nojekyll`) nella branch `main`.
3. Vai su **Settings → Pages**.
4. In **Build and deployment**, scegli **Deploy from a branch**.
5. Seleziona **Branch: `main`** e **Folder: `/ (root)`**, poi **Save**.
6. Entro poco, la pagina sarà raggiungibile a:
   - `https://<tuo-username>.github.io/fantacalcio-viewer/`

> Se vuoi un URL senza `/fantacalcio-viewer/`, crea un repo chiamato **`<tuo-username>.github.io`** e carica qui i file: la pagina sarà `https://<tuo-username>.github.io/`.

## 🔄 Aggiornare i dati in futuro

Questo viewer contiene i dati direttamente dentro `index.html`. Per aggiornare:
- Apri `index.html` e sostituisci l'array `const DATA = [...]` con i nuovi dati (puoi rigenerare il file con lo script originale).
- In alternativa, puoi aprire una **Pull Request** con il nuovo `index.html` generato e fare **merge**.

> Opzionale (per semplificare gli update): separa i dati in un file `data.js` con `window.DATA = [...]` e nel `index.html` sostituisci `const DATA = ...` con `window.DATA`. Ricorda di aggiungere `<script src="data.js"></script>` prima dello script principale.

## 🧪 Test locale
Apri `index.html` con un doppio click nel browser. Funziona anche **offline**.

## ℹ️ Note
- Il file usa CDN pubblici (Tabulator). Assicurati che la rete dei tuoi utenti non blocchi i CDN.
- Il file `.nojekyll` impedisce che GitHub Pages applichi Jekyll che, in alcuni casi, può interferire con asset in sottocartelle o file con underscore.

Buon fantacalcio! ⚽️
