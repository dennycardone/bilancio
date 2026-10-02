# 💶 Bilancio Mensile

Web app per gestire il bilancio mensile personale a **contenitori** (Spese Fisse, Divertimento, Risparmi, Sara + quelli che vuoi tu).
Pensata per lo smartphone, funziona anche su desktop e **offline**.

- Nessun account, nessun server, nessun costo
- I dati restano **solo nel tuo browser** (localStorage)
- Un unico file `index.html`, senza librerie esterne

## Come si usa

1. Apri l'app: in alto c'è il **Saldo totale**, il portafoglio principale da cui distribuisci i soldi ai contenitori.
   Toccalo per impostare il capitale iniziale e registrare entrate (es. stipendio) e uscite.
2. Tocca un contenitore → inserisci **capitale iniziale**, **budget destinato**, entrate e uscite.
   Il budget destinato e le entrate del contenitore vengono **scalati automaticamente dal saldo totale**
   (togli la spunta "Prelevata dal saldo totale" per le entrate che arrivano da fuori, es. un rimborso).
3. Oppure usa **＋ Movimento** per aggiungere velocemente una spesa o un'entrata.
4. Il saldo si aggiorna da solo: `Saldo finale = Capitale iniziale + Entrate − Uscite`.
5. A fine mese premi **↪ Riporta saldi al mese successivo**: il saldo totale e i saldi dei contenitori diventano il capitale iniziale del mese dopo.

**Patrimonio complessivo** = saldo totale + tutti i contenitori. Gli spostamenti dal saldo totale ai contenitori non lo cambiano: contano solo le entrate e le uscite reali.
6. In **Storico** trovi tutti i mesi; toccane uno per riaprirlo e modificarlo.

## Installarla sul telefono

Apri il link di GitHub Pages dal telefono, poi:

- **iPhone (Safari):** Condividi → *Aggiungi alla schermata Home*
- **Android (Chrome):** menu ⋮ → *Installa app* / *Aggiungi a schermata Home*

Dopo la prima apertura funziona anche senza connessione.

## Backup

I dati sono legati al browser e al dispositivo. Da **Impostazioni → Esporta backup** scarichi un file `.json`;
con **Importa backup** lo ripristini (anche su un altro dispositivo). **Esporta CSV** apre i dati in Excel / Google Sheets.

## File

| File | A cosa serve |
|---|---|
| `index.html` | L'intera app (HTML + CSS + JavaScript) |
| `bilancio.webmanifest`, `icon-192.png`, `icon-512.png` | Installazione sulla schermata Home |
| `sw.js` | Funzionamento offline |
