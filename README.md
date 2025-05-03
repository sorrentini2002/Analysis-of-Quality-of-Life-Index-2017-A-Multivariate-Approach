# Progetto di Statistica Multivariata - Quality of Life Index 2017

## 📝 Sommario

- [Introduzione](#introduzione)
- [Obiettivi del Progetto](#obiettivi-del-progetto)
- [Dataset Utilizzato](#dataset-utilizzato)
- [Metodologie Applicate](#metodologie-applicate)
- [Risultati Principali](#risultati-principali)
- [Requisiti Tecnici](#requisiti-tecnici)
- [Come Eseguire il Codice](#come-eseguire-il-codice)
- [Contributi](#contributi)
- [Licenza](#licenza)
- [Contatti](#contatti)
- [Acknowledgments](#acknowledgments)

---

## 📌 Introduzione

Questo progetto si concentra sull'analisi del **Quality of Life Index 2017 Mid-Year**, focalizzandosi su un campione casuale di **60 città** estratte da un totale di **201**. Lo scopo principale è esplorare le relazioni tra variabili socio-economiche come sicurezza, costo della vita, potere d'acquisto, inquinamento e altre metriche utili per comprendere la qualità della vita nelle città.

L'analisi approfondita dei dati permette di identificare pattern significativi attraverso tecniche avanzate di statistica multivariata, quali **Cluster Analysis**, **PCA (Principal Component Analysis)** e **Analisi Fattoriale**. Il risultato finale è una classificazione delle città in gruppi distinti basati sul loro livello di qualità della vita.

---

## 🎯 Obiettivi del Progetto

- Analizzare le distribuzioni di **Safety Index** e **Cost of Living Index**.
- Studiare le correlazioni tra le principali variabili socio-economiche.
- Classificare le città in gruppi distinti usando la **K-means clustering** e metodi gerarchici.
- Ridurre la dimensionalità dei dati attraverso tecniche di **PCA** e **Analisi Fattoriale**.
- Identificare le relazioni tra inquinamento, traffico e qualità della vita.

---

## 📊 Dataset Utilizzato

- **Fonte**: Quality of Life Index 2017 Mid-Year
- **Numero totale di città**: 201
- **Campione selezionato**: 60 città (scelte casualmente)

**Variabili principali**:
- Safety Index  
- Cost of Living Index  
- Purchasing Power Index  
- Pollution Index  
- Traffic Commute Time Index  

**Altri indicatori**:
- Health Care  
- Climate  
- Property Price to Income Ratio

---

## 🧪 Metodologie Applicate

### 1. Ricodifica in Classi
- **Safety Index**: suddiviso in 5 classi (percentili)
- **Cost of Living Index**: suddiviso in 4 classi (percentili)

### 2. Statistiche Descrittive
- Medie condizionate
- Matrici di covarianza e correlazione

### 3. Cluster Analysis
- **K-means clustering**: selezione ottimale di *K=2* tramite Pseudo F di Fisher
- **Cluster gerarchici**: linkage singolo, completo, medio e Ward

### 4. PCA (Principal Component Analysis)
- Criterio di Kaiser per selezione componenti
- **Rotazione Varimax** per facilitare l’interpretazione

### 5. Analisi Fattoriale
- Rotazione **Promax** per fattori non ortogonali
- Identificazione di **3 fattori chiave**

---

## 📈 Risultati Principali

### 🔹 Cluster a Due Gruppi
- **Cluster 1**: bassa qualità della vita, alto inquinamento, bassa sicurezza
- **Cluster 2**: alto costo della vita, elevata sicurezza, migliori servizi sanitari

### 🔹 Correlazioni Significative
- Positiva: tra **Purchasing Power Index** e **Cost of Living Index**
- Negativa: tra **Cost of Living Index** e **Pollution Index**

### 🔹 PCA
- Le **prime 5 componenti** spiegano il **72%** della varianza totale

### 🔹 Analisi Fattoriale
- **Fattore 1**: Sicurezza e accesso ai servizi
- **Fattore 2**: Costo della vita e potere d'acquisto
- **Fattore 3**: Inquinamento e qualità ambientale

---

## 💻 Requisiti Tecnici

- **Software**: MATLAB (versione 2021a o successiva)
- **Toolbox**: Statistics and Machine Learning Toolbox
- **Funzioni personalizzate**: incluse nella cartella `scripts/funzioni/`

---

## 🤝 Contributi

Puoi contribuire al progetto in diversi modi:

- Segnalare errori nei dati o nell'analisi
- Proporre miglioramenti metodologici
- Aggiungere nuove visualizzazioni o tecniche

> Fai una **pull request** o apri una **issue** per discutere i tuoi suggerimenti!

---

## 📜 Licenza

Questo progetto è distribuito sotto licenza **MIT**. Consulta il file `LICENSE` per maggiori dettagli.

---

## 📬 Contatti

**Matteo Sorrentini**  
Matricola: 2023085  
Email: [sorrentini.2023085@studenti.uniroma1.it](mailto:sorrentini.2023085@studenti.uniroma1.it)

---

## 🙏 Acknowledgments

Grazie all'autore del dataset per aver reso disponibile il *Quality of Life Index 2017 Mid-Year*.  
Questo progetto è stato sviluppato nel contesto dell’esercitazione del **11 dicembre 2023**.
