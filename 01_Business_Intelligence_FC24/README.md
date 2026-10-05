# ⚽ Football Analytics in FC 24: Business Intelligence & Algorithmic Scouting

Questo modulo documenta il progetto di **Business Intelligence** sviluppato all'interno del Corso di Laurea Magistrale in Ingegneria Informatica e dell'Automazione (UNIVPM).

* **Titolo Progetto:** *Vincere con i dati: football analytics in FC 24 tra grandi leghe e scouting dei giocatori*
* **Docenti di riferimento:** Prof. Domenico Ursino, Prof.ssa Federica Parlapiano
* **Studenti:** Andrea Altieri, Andrea Flaiani, Andrea Contursi, Luca Belardinelli

---

## 🎯 Obiettivi e Visione di Business
Il settore della Sports Analytics ha vissuto nell'ultimo decennio un'evoluzione senza precedenti, trasformando club calcistici e leghe in vere e proprie organizzazioni *data-driven*. L'obiettivo primario di questo progetto è superare l'intuito soggettivo nelle decisioni sportive ed economiche, strutturando un sistema completo di Business Intelligence a supporto di:
1. **Staff Tecnico & Match Analysis:** Oggettivazione delle scelte tattiche, gestione dello spogliatoio e strategie sui calci piazzati.
2. **Management & C-Level:** Monitoraggio degli equilibri finanziari (rapporto valore patrimoniale / monte ingaggi), sostenibilità delle rose e benchmark con i concorrenti.
3. **Area Scouting & Recruitment:** Individuazione automatica di talenti e sostituti ottimali tramite algoritmi di Machine Learning multidimensionali.

---

## 🏗️ Architettura e Piattaforme

Il sistema integra tre piattaforme leader di mercato in una pipeline analitica a tre fasi:

```text
               ┌────────────────────────────────────────────────────────┐
               │              Dataset EA Sports FC 24                   │
               │        (male_players, male_teams, male_coaches)        │
               └──────────────────────────┬─────────────────────────────┘
                                          │
                  ┌───────────────────────┼────────────────────────┐
                  ▼                       ▼                        ▼
       ┌─────────────────────┐ ┌────────────────────┐ ┌────────────────────────┐
       │     Qlik Sense      │ │   Tableau Public   │ │   Microsoft Power BI   │
       │    (Fase 1: Staff)  │ │ (Fase 2: Leghe/Eco)│ │ (Fase 3: Scouting ML)  │
       └─────────────────────┘ └────────────────────┘ └────────────────────────┘
```

### 1. Fase 1: Staff Tecnico (Qlik Sense)
* **Analisi dello Spogliatoio:** Mappatura della compatibilità per nazionalità, età ed esperienza per prevenire conflitti interni.
* **Simulatore Tattico:** Analisi predittiva sui moduli di gioco e scenari di pressing (es. contromisure e usura atletica nel *Pressing Alto*).
* **Specialist Calci Piazzati:** Matrice decisionale per oggettivare la scelta dei battitori di rigori, punizioni (vicino/lontano) e calci d'angolo in funzione di curvature, precisione balistica e posizionamento avversario.

### 2. Fase 2: Macro-Analisi dei Campionati (Tableau Public)
* **Benchmark Top 5 Leghe Europee:** Confronto multidimensionale tra Serie A, Premier League, LaLiga, Bundesliga e Ligue 1.
* **Metriche Finanziarie & Z-Score:** Normalizzazione statistica del rapporto tra valore dei cartellini e stipendi lordi annuali.
* **Focus Gender Pay Gap:** Analisi quantitativa del divario economico e retributivo tra calcio maschile ed élite femminile nei principali campionati.

### 3. Fase 3: Asset Management Juventus FC & Machine Learning (Power BI)
* **Focus Rosa Juventus:** Analisi del valore di mercato per reparto, monitoraggio scadenze contrattuali e confronto con le rivali dirette (Milan e Inter).
* **Curva del Declino Atletico:** Modello di correlazione tra età anagrafica e variazione dell'overall per identificare il momento ideale per il turnover o la cessione.
* **Motore di Scouting K-NN (K-Nearest Neighbors):**
  * Spazio vettoriale delle caratteristiche fisiche, tecniche e mentali.
  * Calcolo algoritmico della distanza tra il profilo target (es. titolare in scadenza) e l'intero bacino mondiale dei giocatori censiti.
  * Individuazione di profili ad altissima similarità (*Z-Score Affinity*) a costi di acquisizione sensibilmente inferiori.

---

## 📂 Contenuto della Cartella

```text
01_Business_Intelligence_FC24/
├── README.md                              <-- Questo documento
├── dashboards/
│   └── ProgettoFifa.pbix                  <-- Modello interattivo Power BI Desktop
├── docs/
│   └── FC24_Business Intelligence_2025_2026.pdf <-- Relazione accademica completa (76 pagine)
└── data/
    ├── male_coaches.csv                   <-- Dati anagrafici allenatori
    ├── male_teams.csv                     <-- Dati squadre, leghe e budget
    └── male_players.csv                   <-- Dataset principale calciatori (statistiche e contratti)
```

---

## 🚀 Come Consultare ed Eseguire il Progetto

1. **Relazione Ufficiale:**
   Per tutti i dettagli teorici, formule, tabelle comparative e interpretazioni metodologiche, consultare il documento PDF in [`docs/FC24_Business Intelligence_2025_2026.pdf`](./docs/FC24_Business%20Intelligence_2025_2026.pdf).
2. **Dashboard Interattiva Power BI:**
   * Aprire il file [`dashboards/ProgettoFifa.pbix`](./dashboards/ProgettoFifa.pbix) utilizzando **Microsoft Power BI Desktop**.
   * Se i percorsi dei dati necessitano di aggiornamento locale, impostare la cartella sorgente puntando alla cartella `data/`.
