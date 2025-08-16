# 📊 Riconferme FantaTaxo

Una web app statica per visualizzare e filtrare le rose del fantacalcio, con evidenziazione automatica dei giocatori potenzialmente **riconfermabili**.

## 🚀 Funzionalità

- Tabella interattiva realizzata con [Tabulator.js](https://tabulator.info/).
- Filtri per:
  - Proprietario
  - Ruolo
  - Club di appartenenza
  - Ricerca libera per nome
- Possibilità di **mostrare/nascondere colonne** tramite toggle.
- Evidenziazione automatica:
  - Giocatori con **prezzo ≤ 5** crediti
  - Esclusi i portieri
  - Questi sono segnalati come possibili **riconferme** (al doppio del prezzo d’asta).

## 📂 Struttura del progetto

```
.
├── index.html   # Pagina principale con la logica e l'interfaccia
├── data.js      # Dati delle rose, esportati come array di oggetti JS
└── README.md    # Questo file
```

## 🔧 Come funziona

- `index.html` importa i dati da `data.js` tramite `import`.
- La tabella viene renderizzata con **Tabulator**.
- Gli stili sono definiti inline in `<style>`.
- Tutto gira lato client: nessun backend richiesto.

## 📦 Deploy su GitHub Pages

1. Assicurati che la repo contenga almeno:
   - `index.html`
   - `data.js`
   - `README.md`
2. Vai su **Settings → Pages** nella tua repo GitHub.
3. In **Build and deployment**, seleziona `Deploy from a branch`.
4. Imposta il branch `main` e la cartella `/root` (cioè la root del repo).
5. Salva: la tua app sarà disponibile a un URL del tipo  
   ```
   https://<username>.github.io/<repo>/
   ```

## 📝 Aggiornare i dati

Per aggiornare le rose:
1. Sovrascrivi `data.js` con la nuova versione (può essere rigenerata a partire da un CSV).
2. Fai commit e push su GitHub.
3. GitHub Pages aggiornerà automaticamente la pagina.

## 👨‍💻 Requisiti

- Nessuna installazione necessaria.
- Basta un browser moderno (desktop o mobile).

---

✍️ Progetto creato per gestire in modo interattivo le riconferme del **FantaTaxo**.
