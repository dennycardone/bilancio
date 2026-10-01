# 💶 Bilancio Mensile

Web app per gestire il bilancio mensile personale a **contenitori** (Spese Fisse, Divertimento, Risparmi, Sara + quelli che vuoi tu).
Pensata per lo smartphone, funziona anche su desktop e **offline**.

- Nessun account, nessun server, nessun costo
- I dati restano **solo nel tuo browser** (localStorage)
- Un unico file `index.html`, senza librerie esterne

## Come si usa

1. Apri l'app: vedi il mese corrente e quanto c'è in ogni contenitore.
2. Tocca un contenitore → inserisci **capitale iniziale**, **budget destinato**, entrate e uscite.
3. Oppure usa **＋ Movimento** per aggiungere velocemente una spesa o un'entrata.
4. Il saldo si aggiorna da solo: `Saldo finale = Capitale iniziale + Entrate − Uscite`.
5. A fine mese premi **↪ Riporta saldi al mese successivo**: i saldi finali diventano il capitale iniziale del mese dopo.
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
| `manifest.webmanifest`, `icon-192.png`, `icon-512.png` | Installazione sulla schermata Home |
| `sw.js` | Funzionamento offline |
