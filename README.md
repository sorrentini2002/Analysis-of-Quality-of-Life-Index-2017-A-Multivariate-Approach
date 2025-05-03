# Progetto di Statistica Multivariata - Quality of Life Index 2017

Questo progetto analizza il "Quality of Life Index 2017 Mid-Year", focalizzandosi su un campione di 60 città estratte casualmente da un totale di 201. L'obiettivo principale è esplorare le relazioni tra variabili come sicurezza, costo della vita, potere d'acquisto, inquinamento e altre metriche socio-economiche utilizzando tecniche avanzate di statistica multivariata, tra cui **Cluster Analysis**, **PCA** (Principal Component Analysis) e **Analisi Fattoriale**.

## Obiettivi del Progetto

Il progetto ha come obiettivo l'analisi approfondita delle città in base al loro indice di qualità della vita, con i seguenti obiettivi specifici:

1. **Analizzare** le distribuzioni di **Safety Index** e **Cost of Living Index**.
2. **Studiare** le correlazioni tra le principali variabili socio-economiche.
3. **Classificare** le città in gruppi distinti usando la **K-means clustering** e metodi gerarchici.
4. **Ridurre la dimensionalità** dei dati attraverso tecniche di **PCA** e **Analisi Fattoriale**.
5. **Identificare** le relazioni tra fattori come inquinamento, traffico e qualità della vita.

## Dati Utilizzati

- **Dataset**: "Quality of Life Index 2017 Mid-Year" (comprendente 201 città, 9 variabili quantitative).
- **Campione**: 60 città selezionate casualmente.
- **Variabili Chiave**:
  - **Safety Index**
  - **Cost of Living Index**
  - **Purchasing Power Index**
  - **Pollution Index**
  - **Traffic Commute Time Index**
  - Altri indicatori: **Health Care**, **Climate**, **Property Price to Income Ratio**.

## Metodologie Applicate

Il progetto utilizza un insieme di tecniche statistiche avanzate per analizzare i dati:

1. **Ricodifica in Classi**: 
   - Suddivisione di "Safety Index" in 5 classi e "Cost of Living Index" in 4 classi, utilizzando percentili.
   
2. **Statistiche Descrittive**: 
   - Calcolo di medie condizionate, matrici di covarianza e correlazione per analizzare la distribuzione dei dati.
   
3. **Cluster Analysis**:
   - Applicazione della **K-means clustering** con ottimizzazione tramite il **Pseudo F di Fisher** per determinare il numero ottimale di cluster (K=2).
   - Metodi gerarchici (linkage singolo, completo, medio, Ward) per ottenere una visione più dettagliata della segmentazione.

4. **Analisi delle Componenti Principali (PCA)**:
   - Utilizzo del **criterio di Kaiser** per selezionare le 5 componenti principali.
   - **Rotazione Varimax** per facilitare l'interpretazione delle componenti principali.

5. **Analisi Fattoriale**:
   - Applicazione della **rotazione Promax** per fattori non ortogonali.
   - Identificazione di 3 fattori chiave che spiegano la maggior parte della varianza.

## Risultati Principali

- **Cluster a Due Gruppi**:
  - **Cluster 1**: Città con bassa qualità della vita, alto inquinamento, bassa sicurezza.
  - **Cluster 2**: Città con alto costo della vita, elevata sicurezza, migliori servizi sanitari.

- **Correlazioni Significative**:
  - Positiva tra **Purchasing Power Index** e **Cost of Living Index**.
  - Negativa tra **Cost of Living Index** e **Pollution Index**.
  
- **PCA**: Le prime 5 componenti principali spiegano il **72% della varianza totale** dei dati, indicando una buona rappresentazione delle principali dimensioni del Quality of Life.

## Come Eseguire il Codice

Per eseguire le analisi, segui i passaggi indicati di seguito:

### Prerequisiti

- **Software**: MATLAB (versione 2021a o successiva).
- **Toolbox**: Assicurati di avere il **Statistics and Machine Learning Toolbox** installato.
- **Funzioni Personalizzate**: Le funzioni necessarie sono incluse nella cartella `scripts/funzioni/`.

### Passaggi

1. **Carica il dataset originale** nel formato `.mat` nella cartella `data/`.
2. **Esegui il codice**:
   - Avvia lo script principale `WB2023.m` in MATLAB.
   - Questo genererà tutte le analisi, inclusi i grafici e le tabelle, che saranno salvati nella cartella `results/`.
3. **Visualizza i risultati**:
   - I risultati saranno disponibili come grafici (PNG/PDF) nella cartella `results/figures/` e come tabelle nei file di output in `results/tables/`.

## Conclusioni

Il progetto evidenzia una chiara divisione tra città con alta e bassa qualità della vita, determinata da vari fattori come la sicurezza, l'inquinamento e la disponibilità di servizi sanitari. Le tecniche di **cluster analysis** e **PCA** hanno permesso di individuare pattern significativi e di ridurre la complessità dei dati, fornendo spunti per politiche urbane mirate.

## Contatti

- **Autore**: Matteo Sorrentini
- **Matricola**: 2023085
- **Email**: [sorrentini.2023085@studenti.uniroma1.it]

