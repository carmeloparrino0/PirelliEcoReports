# PirelliEcoReports – Archivio Report di Sostenibilità (2015–2024)

Interfaccia web one-page dedicata all’analisi e alla consultazione dei **report annuali** e dei **bilanci di sostenibilità** di Pirelli nel periodo **2015–2024**.

Il progetto si concentra su:

- visualizzazione chiara e moderna dei documenti;
- possibilità di **filtrare e cercare** i report;
- accesso diretto ai **PDF ufficiali** per lo studio delle politiche ESG nel tempo.

---

## Demo

Demo Demo [PirelliEcoReports](https://johnny9798.github.io/melo.github.io/ "Preview Demo").

---

## Contesto del progetto

Progetto realizzato nell’ambito di:

> **PW – Tecnologia Web per la Sostenibilità d’Impresa**

Obiettivo: costruire un’interfaccia front-end pulita, usabile e responsive, che permetta a studenti/analisti di:

- esplorare rapidamente i report di sostenibilità Pirelli;
- confrontare anni e periodi differenti;
- individuare temi chiave (ESG, climate strategy, Net Zero, supply chain, ecc.).

---

## Caratteristiche principali

- 🎯 **Hero “PirelliEcoReports”**
  - Presentazione del progetto, logo Pirelli in evidenza.
  - Metadati del progetto (corso, azienda, settore).

- 🔍 **Toolbar dei filtri**
  - Campo di ricerca testuale (per anno, parole chiave, contenuto).
  - Filtro per periodi:
    - 2015–2017 (early)  
    - 2018–2020 (mid)  
    - 2021–2024 (recent)
  - Contatore dinamico dei report visibili.

- 📚 **Griglia di card**
  - Una **card per ogni report** annuale (2015–2024).
  - Badge per settore, anno, paese.
  - Pillole tematiche (Climate strategy, Net Zero, Economia circolare, ecc.).
  - Pulsante con **link diretto al PDF** ufficiale Pirelli.

- 🧠 **Logica di filtro lato client (JavaScript puro)**
  - Ricerca full-text su:
    - data-attribute (name, year, keywords)
    - testo della card
  - Filtri combinati (periodo + testo).
  - Messaggio “Nessun report trovato” se i filtri non restituiscono risultati.

- 📱 **Design responsive**
  - Layout ottimizzato per desktop e mobile.
  - Hero che passa da colonna singola (mobile) a layout a due colonne (desktop).
  - Card e toolbar adattive, con griglia fluida.

---

## Tecnologie utilizzate

- **HTML5** – Struttura semantica della pagina (hero, toolbar, section, article).
- **CSS3** – Layout, tema scuro, gradiente, card e componenti UI.
  - Uso intensivo di **CSS custom properties** (variabili `:root`) per:
    - palette colori;
    - raggi di bordo;
    - ombre e transizioni.
- **JavaScript vanilla** – Logica di ricerca e filtraggio sulla pagina, senza framework.

---

## Struttura del progetto

```text
.
├── index.html   # Pagina principale con layout hero, toolbar, card e script di filtro
├── style.css    # Stile completo dell'interfaccia (tema, griglia, card, responsive)
└── favicon.ico  # Icona del progetto
