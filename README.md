# **Analisi dei Dati sui Taxi - Marzo 2016**

Questo progetto analizza un dataset relativo ai viaggi in taxi nel mese di marzo 2016, con l'obiettivo di esplorare, pulire e visualizzare i dati per ottenere informazioni utili sulle tendenze dei trasporti.

## **Dati utilizzati**

Il dataset analizzato si chiama **"yellow_tripdata_2016-03.csv"** e contiene informazioni sui viaggi effettuati con i taxi gialli a New York.

### **Principali colonne del dataset**:

- `pickup_datetime`: data e ora di inizio del viaggio
- `dropoff_datetime`: data e ora di fine del viaggio
- `passenger_count`: numero di passeggeri
- `trip_distance`: distanza percorsa in miglia
- `fare_amount`: costo della corsa
- `payment_type`: metodo di pagamento
- `store_and_fwd_flag`: indicatore se i dati sono stati archiviati prima di essere inviati al server

## **Obiettivi del progetto**

1. **Caricamento ed esplorazione dei dati**: verificare la struttura del dataset e individuare eventuali valori mancanti.
2. **Pulizia dei dati**: eliminare colonne non necessarie e gestire i dati nulli.
3. **Analisi statistica**: osservare le principali statistiche descrittive dei dati.
4. **Visualizzazione dei dati**: creare grafici per analizzare distribuzioni e trend dei viaggi in taxi.

## **Tecnologie utilizzate**

- **pandas** per la manipolazione e pulizia dei dati
- **numpy** per le operazioni numeriche
- **matplotlib** e **seaborn** per la visualizzazione grafica dei dati
- **folium** per la creazione di mappe interattive.
- **scikit-learn** per la modellazione e l'analisi predittiva.
- **tensorflow** e **keras** per l'implementazione del modello LSTM e il deep learning.

## **Passaggi principali dell'analisi**

1. **Caricamento dei dati**: lettura del file CSV in un DataFrame Pandas.
2. **Pulizia dei dati**:
   - Rimozione di colonne inutili (`Unnamed: 0`, `store_and_fwd_flag`)
   - Eliminazione di valori nulli
3. **Esplorazione del dataset**:
   - Utilizzo di `df.info()` e `df.describe()` per analizzare la struttura e le statistiche dei dati
4. **Visualizzazione dei dati**:
   - Creazione di grafici per osservare la distribuzione dei passeggeri, la distanza media delle corse e la distribuzione dei costi delle corse.
5. **Modellazione Predittiva:**
   - Implementazione di modelli di **Regressione Lineare** e **Regressione Logistica** per identificare relazioni tra le variabili e prevedere andamenti futuri.
   - Utilizzo di modelli di **Deep Learning** basati su **LSTM** per effettuare previsioni a lungo termine sui trend dei viaggi.
6. **Visualizzazione Geospaziale:**
   - Creazione di mappe interattive con **folium** per rappresentare la distribuzione geografica dei punti di partenza e destinazione dei taxi.

## **Risultati ottenuti**

Dall'analisi dei dati emergono alcune tendenze chiave:

- La maggior parte delle corse coinvolge uno o due passeggeri, suggerendo un utilizzo prevalente da parte di individui o coppie.
- Le distanze percorse mostrano una distribuzione con una forte presenza di viaggi brevi, tipici degli spostamenti urbani.
- Il pagamento con carta di credito è il metodo più utilizzato, suggerendo una crescente digitalizzazione delle transazioni nei servizi di trasporto.

## **Conclusioni**

Questa analisi fornisce una panoramica delle principali caratteristiche dei viaggi in taxi a New York nel marzo 2016. Il dataset è stato ripulito e analizzato, fornendo una visione sulle abitudini dei passeggeri e sulle dinamiche di trasporto urbano.

#### **Fonte Dataset**

https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data

#### **Versione python utilizzata:**

3.11.8
