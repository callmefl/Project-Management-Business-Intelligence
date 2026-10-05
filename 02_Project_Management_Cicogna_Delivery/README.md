# 🚁 Progetto Cicogna: Sistemi di Logistica Aerea Urbana (Ancona 2025-2026)

Questo modulo documenta il piano di **Project Management** strutturato secondo lo standard **PMI (Project Management Institute) / PMBOK**, sviluppato all'interno del Corso di Laurea Magistrale in Ingegneria Informatica e dell'Automazione (UNIVPM).

* **Codice Iniziativa:** `PGCG` (Progetto Cicogna)
* **Oggetto:** Rete logistica urbana autonoma basata su flotta di droni (UAV) per il comune di Ancona.
* **Deliverable Primario:** Project Management Plan (PMP) integrale di **355 pagine** corredato dal piano di schedulazione in **Microsoft Project (`.mpp`)**.

---

## 🎯 Executive Summary & Business Case

Il Progetto Cicogna nasce per rivoluzionare l'ultimo miglio logistico (*Last-Mile Delivery*) nel capoluogo dorico, decongestionando il traffico veicolare su gomma, azzerando le emissioni dirette di CO2 e garantendo tempi di recapito garantiti.

```text
               ┌────────────────────────────────────────────────────────┐
               │              DronePort Centrale (Hub Porto)            │
               │         Centrale operativa, manutenzione e ricarica    │
               └──────────────────────────┬─────────────────────────────┘
                                          │
                            Rotte Aeree BVLOS (U-Space)
                                          │
                  ┌───────────────────────┼────────────────────────┐
                  ▼                       ▼                        ▼
       ┌─────────────────────┐ ┌────────────────────┐ ┌────────────────────────┐
       │   Locker UAV #01    │ │   Locker UAV #02   │ │     Locker UAV #16     │
       │ (Zona Ospedaliera)  │ │   (Piazza Cavour)  │ │      (Polo Q3/Q4)      │
       └─────────────────────┘ └────────────────────┘ └────────────────────────┘
```

### 1. Architettura Logistica "Hub-to-Locker"
A differenza di modelli sperimentali di consegna porta-a-porta (cortili privati o balconi), il progetto adotta rigidamente il paradigma **Hub-to-Locker**:
* I droni decollano unicamente da un **DronePort centrale** (in area portuale) e atterrano su **16 Locker intelligenti automatizzati** distribuiti nei nodi nevralgici della città.
* **Perché questa scelta?** Azzeramento del rischio di collisione con ostacoli aerei urbani (fili, alberi, persone), abbattimento dell'inquinamento acustico residenziale e rotte fisse rigidamente controllabili dall'ENAV.

### 2. Flotta Operativa Differenziata
* **13 Droni Leggeri (Payload fino a 5 kg):** Dedicati al segmento B2C (e-commerce e pacchi rapidi), responsabili del 60% dei volumi giornalieri.
* **8 Droni Medi (Payload fino a 25 kg con verricello integrato):** Dedicati al segmento B2B e trasporti sanitari/diagnostici ad alto valore aggiunto con accordi SLA garantiti.

### 3. Sostenibilità e Ingegneria Finanziaria
* **CAPEX (Investimento Iniziale):** ~6.480.000 €
* **IRR (Tasso Interno di Rendimento):** 11,2%
* **Periodo di Payback:** 69 mesi (circa 5,7 anni)
* **Leva Fiscale PNRR / Transizione 5.0:** La progettazione 100% elettrica e l'autosufficienza energetica degli Hub fino al 60% (fotovoltaico e micro-eolico) abilita l'accesso prioritario al **Credito d'Imposta statale del 40%**, garantendo la sostenibilità dell'opera.

---

## 🏗️ WBS (Work Breakdown Structure)

La pianificazione delle attività isola gli stream operativi in pacchetti di lavoro modulari:
* **WP 1 - Project Management & Governance:** Coordinamento, monitoraggio SAL, gestione contratti e contabilità.
* **WP 2 & WP 7 - Dominio Software & UTM:** Integrazione API con la piattaforma ENAV per il coordinamento del traffico nello spazio aereo *U-Space* (<1.5s di latenza telemetrica) e sviluppo delle App front-end per cittadini ed operatori.
* **WP 3 - Ingegneria Aeronautica & Flotta:** Acquisizione UAV, collaudi statici, simulazioni in Digital Twin e integrazione meccanica dei verricelli di rilascio.
* **WP 4 & WP 6 - Opere Edili & Infrastrutture di Terra:** Cantierizzazione, scavi, allacciamenti alla rete elettrica e installazione dei 16 Locker e della base DronePort.
* **WP 5 - Logistica & Supply Chain:** Approvvigionamento ricambi e gestione dei vettori di supporto.

---

## ⏱️ Schedulazione & Percorso Critico (Microsoft Project)

Il piano temporale si sviluppa su un orizzonte di **22 mesi** (Gennaio 2026 - Novembre 2027), articolato su 10 Milestone e 6 SAL:
* **M3 - Approvazione Permessi Edilizi:** Vincolo critico per la cantierizzazione contemporanea dei 16 Locker nei siti comunali.
* **M6 - Certificazione ENAC/EASA BVLOS:** Validazione del rischio operativo tramite metodologia **SORA** (*Specific Operations Risk Assessment*) per il volo *Beyond Visual Line of Sight*. Rappresenta il principale collo di bottiglia del **Percorso Critico** (*Critical Path*).
* **M8 - Go-Live Operativo:** Apertura al pubblico del servizio e rilascio delle applicazioni mobile per il ritiro nei locker.

---

## 🛡️ Gestione dei Rischi & Change Management

### Analisi Quantitativa EMV (Expected Monetary Value)
Il modello matematico del rischio non si basa su stime arbitrarie, ma quantifica:
* **Riserva di Contingenza (Contingency Reserve):** **404.750 €**, allocata per gestire i rischi identificati e formalizzati nel registro dei rischi.
* **Riserva di Management (Management Reserve):** **680.000 €**, a copertura di imprevisti sistemici o ritardi autorizzativi istituzionali.
* **Strategia di Trasferimento:** Copertura dei rischi catastrofali (caduta velivolo, violazione cyber GPS) tramite stipula di massimali assicurativi RC e Cyber-Risk dedicati.

### Registro delle Modifiche (Change Control)
* **CR_01 (Adozione Paracaduti Balistici FTS) -> APPROVATA:** Modifica introdotta a fronte dei requisiti di sicurezza ENAC per la classe di rischio SAIL IV (+42.000 € assorbiti dalle riserve di gestione). Senza di essa il progetto non avrebbe ottenuto il permesso di sorvolo urbano.
* **CR_02 (Consegna a Domicilio "Door-to-Door") -> RESPINTA:** Richiesta avanzata dallo Sponsor commerciale per competere coi corrieri tradizionali. Respinta dal Project Manager per evitare un grave fenomeno di **Scope Creep** che avrebbe compromesso la sicurezza e allungato i tempi autorizzativi di oltre 18 mesi.

---

## 📂 Contenuto della Cartella

```text
02_Project_Management_Cicogna_Delivery/
├── README.md                              <-- Questo documento
├── ms_project/
│   └── Progetto Definitivo (1).mpp        # File nativo di schedulazione Microsoft Project
├── docs/
│   └── Drone Delivery - Project Management 2025-2026.pdf # Project Management Plan completo (355 pagine)
└── images/                                # Schemi, WBS e diagrammi esplicativi
```

---

## 🚀 Come Consultare il Progetto

1. **Project Management Plan (Documento Master):**
   La pianificazione dettagliata (comprensiva di Matrice Stakeholder, Piano di Comunicazione, Baseline dei Costi e WBS Dictionary) è consultabile nel file PDF in [`docs/Drone Delivery - Project Management 2025-2026.pdf`](./docs/Drone%20Delivery%20-%20Project%20Management%202025-2026.pdf).
2. **Schedulazione e Gantt (Microsoft Project):**
   * Il file [`ms_project/Progetto Definitivo (1).mpp`](./ms_project/Progetto%20Definitivo%20(1).mpp) può essere aperto con **Microsoft Project 2019/2021/365** o con visualizzatori compatibili (es. ProjectLibre, GanttProject).
   * Al suo interno è possibile analizzare la catena delle relazioni di precedenza (FS, SS), i carichi di lavoro delle risorse umane/strumentali e il tracciamento dello scostamento rispetto alla Baseline.
