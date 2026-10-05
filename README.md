# Project Management e Business Intelligence
Progetto universitario per i corsi di **Business Intelligence** e **Project Management per l'ICT** (Corso di Laurea Magistrale in Ingegneria Informatica e dell'Automazione, Università Politecnica delle Marche, A.A. 2025/2026).

L'obiettivo del repository è documentare e strutturare due progetti ingegneristici complementari:
* **Business Intelligence & Sports Analytics**: estrazione, pulizia, modellazione dimensionale (*Star Schema*) e visual analytics sui dati di FC 24, integrando dashboard analitici multi-piattaforma (Qlik Sense, Tableau, Power BI)
* **Project Management & Operations Governance**: pianificazione integrata e formalizzazione metodologica secondo lo standard **PMI / PMBOK** di una rete logistica a guida autonoma con droni per la città di Ancona (*Progetto Cicogna*), comprensiva di schedulazione deterministica con percorso critico su **Microsoft Project (`.mpp`)**, calcolo quantitativo dei rischi (**EMV**) e ingegneria finanziaria (CAPEX, Payback, Transizione 5.0 / PNRR).

---

## 🚀 Consultazione Rapida & Deliverable Chiave

### Prerequisiti
* [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) (per l'esplorazione del modello `.pbix`).
* [Microsoft Project](https://www.microsoft.com/it-it/microsoft-365/project/project-management-software)
* Qualsiasi lettore PDF per le relazioni accademiche integrali.

### 1. Accesso Rapido ai File di Progetto
* 📊 **Dashboard Power BI Interattiva**: [`01_Business_Intelligence_FC24/dashboards/ProgettoFifa.pbix`](./01_Business_Intelligence_FC24/dashboards/ProgettoFifa.pbix)
* ⏱️ **Schedulazione Gantt & Percorso Critico**: [`02_Project_Management_Cicogna_Delivery/ms_project/Progetto Definitivo (1).mpp`](./02_Project_Management_Cicogna_Delivery/ms_project/Progetto%20Definitivo%20(1).mpp)
* 📑 **Relazione Business Intelligence (76 pag.)**: [`01_Business_Intelligence_FC24/docs/FC24_Business Intelligence_2025_2026.pdf`](./01_Business_Intelligence_FC24/docs/FC24_Business%20Intelligence_2025_2026.pdf)
* 📑 **Project Management Plan Integrale (355 pag.)**: [`02_Project_Management_Cicogna_Delivery/docs/Drone Delivery - Project Management 2025-2026.pdf`](./02_Project_Management_Cicogna_Delivery/docs/Drone%20Delivery%20-%20Project%20Management%202025-2026.pdf)

---

## 📊 Sintesi Tecnica: 01. Business Intelligence (FC 24)

Pipeline analitica multilivello progettata per coprire le esigenze informative di uno staff calcistico professionistico e dell'area dirigenziale.

### Architettura Multi-Piattaforma & Analytics

| Piattaforma | Target Utente | Modulo Analitico | Algoritmi / Metriche Chiave | Output Prodotto |
| :--- | :--- | :--- | :--- | :--- |
| **Qlik Sense** | Staff Tecnico & Match Analyst | Analisi Tattica & Spogliatoio | Simulazione Pressing Alto; Calcolo compatibilità anagrafica/linguistica | Matrice decisionale per 11 titolare e gestione spogliatoio |
| **Qlik Sense** | Tattico Specialistico | Specialisti Calci Piazzati | Filtri di traiettoria, distanze di tiro, indici di pericolosità balistica | Algoritmo per la selezione oggettiva del tiratore ottimale |
| **Tableau Public** | Direzione Sportiva | Macro-Analisi Top 5 Leghe | *Z-Score* Valore/Stipendi; Distribuzione fasce d'età nei campionati UE | Benchmark economico-sportivo europeo |
| **Tableau Public** | C-Level / Governance | Parità di Genere & Valore | Ratio retributivo medio maschile vs femminile nei top campionati | Analisi quantitativa sul Gender Pay Gap |
| **Power BI** | Management Juventus FC | Monitoraggio Rosa & Valore | Curve del declino atletico (Overall vs Età); Monitoraggio scadenze contratti | Cruscotto economico-finanziario e confronto vs Inter/Milan |
| **Python / ML** | Area Scouting | Algorithmic Scouting Engine | **K-Nearest Neighbors (K-NN)** su spazio vettoriale N-dimensionale | Individuazione profili simili (*Player Similarity*) a costo budget |

---

## 📈 Sintesi Tecnica: 02. Project Management (Cicogna Delivery)

Piano di Project Management formalizzato secondo lo standard **PMI/PMBOK** per l'avvio e la gestione esecutiva di un'infrastruttura di logistica aerea autonoma (*Hub-to-Locker*) nel comune di Ancona.

### Parametri & Metriche di Governance Operativa

| Dominio | Parametro di Progetto | Valore / Strategia Assunta | Rationale Ingegneristico |
| :--- | :--- | :--- | :--- |
| **Architettura Logistica** | Modello Operativo | **Hub-to-Locker** (1 DronePort + 16 Locker UAV) | Rotte fisse standardizzate; annullamento rischi di impatto privato *porta a porta* |
| **Flotta Operativa** | Dimensionamento UAV | 13 Droni Leggeri (≤5 kg) + 8 Droni Medi (≤25 kg) | Copertura 60% B2C urbano e SLA dedicati per trasporto medicale/B2B pesante |
| **Ingegneria Finanziaria** | CAPEX & Payback | **CAPEX 6.480.000 €** \| **IRR 11,2%** \| **Payback 69 mesi** | Sostenibilità validata tramite **Credito d'Imposta 40% (Transizione 5.0 / PNRR)** |
| **Schedulazione (MS Project)** | Baseline dei Tempi | **22 mesi** (Gennaio 2026 - Novembre 2027) | 10 Milestone, 6 SAL; percorso critico vincolato da autorizzazioni istituzionali |
| **Colli di Bottiglia Normativi** | Permessi & Certificazioni | **M3** (Edilizia comunale) & **M6** (ENAC/EASA BVLOS via SORA) | Tolleranza temporale e accodamento prove fisiche alle approvazioni documentali |
| **Risk Management (EMV)** | Budget Riserve | **404.750 € (Contingency)** + **680.000 € (Management)** | Calcolo probabilistico del valore monetario atteso; polizze RC Droni e Cyber-Risk |
| **Change Management** | CR_01: Paracaduti Balistici | **APPROVATA** (+42.000 € assorbiti da riserve) | Requisito vincolante ENAC classe SAIL IV per spezzare l'impatto al suolo (<69 J) |
| **Change Management** | CR_02: Consegna a Domicilio | **RESPINTA** (Blocco *Scope Creep*) | Rifiuto consegna su tetti/balconi per preservare profilo di sicurezza e scadenze |

---

## 📁 Struttura del Repository

```text
MSc-Engineering-Portfolio/
│
├── 01_Business_Intelligence_FC24/
│   ├── dashboards/
│   │   └── ProgettoFifa.pbix                  # Modello semantico e cruscotti Power BI Desktop
│   ├── data/                                  # Dataset estratti da Kaggle (EA Sports FC 24)
│   │   ├── male_coaches.csv                   # Anagrafica e dettagli tecnici allenatori
│   │   ├── male_players.csv                   # Dataset 96MB: anagrafica, statistiche fisiche e ingaggi
│   │   └── male_teams.csv                     # Record società, campionati e budget
│   ├── docs/
│   │   └── FC24_Business Intelligence_2025_2026.pdf # Relazione accademica completa (76 pagine)
│   └── README.md                              # Documentazione di dettaglio del modulo BI & ML
│
├── 02_Project_Management_Cicogna_Delivery/
│   ├── docs/
│   │   └── Drone Delivery - Project Management 2025-2026.pdf # Project Management Plan integrale (355 pagine)
│   ├── images/
│   │   └── .gitkeep                           # Directory per esportazioni grafiche WBS e Gantt
│   ├── ms_project/
│   │   └── Progetto Definitivo (1).mpp        # Modello di schedulazione Microsoft Project
│   └── README.md                              # Documentazione di dettaglio del modulo PM & Governance
│
├── .gitignore                                 # Esclusioni file temporanei, lock Office e cache Python
└── README.md                                  # Vetrina tecnica e panoramica dei progetti
```

---

## 👥 Crediti Accademici
* **Studenti:** Andrea Altieri, Andrea Flaiani, Andrea Contursi, Luca Belardinelli
* **Corso di Laurea:** Ingegneria Informatica e dell'Automazione (Laurea Magistrale)
* **Ateneo:** Università Politecnica delle Marche (UNIVPM)
