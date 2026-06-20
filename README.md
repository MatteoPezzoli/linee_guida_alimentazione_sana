# 🥗 Mangio Bene

Webapp single-page basata sulle **Linee Guida per una Sana Alimentazione CREA 2018** (revisione novembre 2019).

> ⚕️ Questa app è a scopo informativo e **non sostituisce il parere di un medico o nutrizionista.**

## Demo

🌐 **[https://matteopezzoli.github.io/linee_guida_alimentazione_sana/](https://matteopezzoli.github.io/linee_guida_alimentazione_sana/)**

Oppure scarica il repository e apri `index.html` direttamente nel browser — nessuna configurazione necessaria.

## Funzionalità

### 🗓️ Consiglio del Giorno
- 33 consigli nutrizionali suddivisi in 8 categorie (Frutta e Verdura, Cereali e Legumi, Proteine, Grassi e Condimenti, Sale e Zucchero, Idratazione, Attività Fisica, Sicurezza Alimentare, Sostenibilità, Diete e Integratori)
- Seed giornaliero: lo stesso utente vede lo stesso consiglio per tutta la giornata
- Pulsante "Altro consiglio" per scorrerne altri

### 📋 Pianifica la Settimana
- Generatore di piano alimentare Lunedì–Domenica
- 4 profili: Adulto, Anziano / Over 65, Sportivo, In gravidanza
- Rispetta i vincoli settimanali CREA:
  - Pesce: ≥ 2 cene
  - Legumi: 2–3 tra pranzo e cena
  - Carne rossa: max 1 volta
  - Carne bianca: 2–3 volte
  - Uova: 2–4 a settimana (CREA 2018, cap. 5)
  - Nessuna ripetizione nella stessa settimana
  - Filtro stagionalità automatico (primavera / estate / autunno / inverno)
- Riepilogo visivo con semaforo: porzioni verdura/frutta (≥ 35/sett.), pesce (2–3), legumi (4–6)
- Pulsante **Esporta come testo** → scarica `piano-alimentare-mangio-bene.txt`
- Piano salvato in `localStorage` (cache 7 giorni)

### 📖 Le 13 Direttive CREA
Tutte e 13 le direttive del documento ufficiale, nella struttura corretta:

| # | Direttiva |
|---|---|
| 1 | Controlla il peso e mantieniti sempre attivo |
| 2 | Più frutta e verdura |
| 3 | Più cereali integrali e legumi |
| 4 | Bevi ogni giorno acqua in abbondanza |
| 5 | Grassi: scegli quali e limita la quantità |
| 6 | Zuccheri, dolci e bevande zuccherate: meno è meglio |
| 7 | Il sale? Meno è meglio |
| 8 | Bevande alcoliche: il meno possibile |
| 9 | Varia la tua alimentazione: come e perché |
| 10 | Consigli speciali per categorie particolari |
| 11 | Attenti alle diete e agli integratori senza basi scientifiche |
| 12 | La sicurezza degli alimenti dipende anche da te |
| 13 | Sostenibilità delle diete: tutti possiamo contribuire |

## Tecnologia

| Aspetto | Scelta |
|---|---|
| Stack | HTML + CSS + JavaScript puro (nessun framework) |
| Dipendenze esterne | Google Fonts (Playfair Display + Inter) — solo CDN usata |
| Dati nutrizionali | Hardcoded nel file JS — nessuna chiamata API |
| Persistenza | `localStorage` (profilo utente + piano corrente) |
| Funziona offline | ✅ dopo il primo caricamento dei font |
| Deploy | Un singolo `index.html` — pronto per GitHub Pages |

## Struttura del progetto

```
index.html   ← tutta l'app (HTML + CSS inline + JS inline)
README.md
```

## Fonte

Centro di Ricerca Alimenti e Nutrizione (CREA)  
*Linee Guida per una Sana Alimentazione* — Revisione 2018, aggiornamento novembre 2019  
Approvate dal Consiglio Scientifico del CREA il 3 aprile 2019

---

*Realizzata da Matteo Pezzoli*
