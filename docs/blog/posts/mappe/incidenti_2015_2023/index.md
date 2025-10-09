---
title: Incidenti Stradali - Palermo 2015-2023
description: Dashboard Interattiva
draft: false
date: 2025-10-09T12:00:00
authors:
  - gbvitrano
categories:
  - Mappe
tags:
  - PalermoHub
  - Incidenti
  - Palermo
  - Mappe
social_image: https://palermohub.opendatasicilia.it/legend/clip_index/palermo_incidenti_2015-2023.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
</style>
[![PalermoHub](https://palermohub.opendatasicilia.it/legend/clip_index/palermo_incidenti_2015-2023.jpg "Incidenti Stradali - Palermo 2015-2023 • Dashboard Interattiva" ){class="crop gray off" align=left}](index.md)

# "Ecco la mappa": …..(spoiler: la mappa non c'è)

*Quante volte vi è capitato? Scrollate distrattamente il feed, inciampate in un titolo allettante – "Ecco la mappa del degrado urbano", "Ecco la mappa dei cantieri estivi" – e pensate: "Finalmente qualcosa di chiaro e immediato". Click. E invece no.*

*Vi ritrovate catapultati in un fiume di parole degno del peggior tema scolastico,<!-- more -->  paragrafi su paragrafi che tentano disperatamente di spiegarvi coordinate, numeri e localizzazioni che una mappa  – quella promessa e mai arrivata – vi avrebbe comunicato in tre secondi netti. Della mappa? Nemmeno l'ombra. Nel migliore dei casi, se siete fortunati, vi imbattete in un'immagine sgranata stile anni Ottanta o in un PDF illeggibile che sembra scansionato col fax.*

*Eppure esistono. Software gratuiti, opensource, alla portata di chiunque abbia un minimo di buona volontà. Strumenti che permettono di creare mappe dignitose e grafici comprensibili anche a chi non ha una laurea in cartografia.*

*Quindi, cari giornali nazionali, locali e siti istituzionali vari: o inserite davvero la benedetta mappa, oppure risparmiateci il clickbait e scrivete onestamente "Ecco un lungo articolo senza mappa". Almeno saremo avvisati.*

*"**Ecco la mappa**" è una rubrica nata da un'idea di [@aborruso](https://www.linkedin.com/in/andreaborruso/) per documentare (con ironia e un filo di disperazione) il fenomeno delle mappe promesse e mai consegnate.*

---

## Una Piattaforma Open Data per la sicurezza urbana

Analizzare i dati degli incidenti stradali non è solo una questione statistica: è un'opportunità per comprendere meglio i rischi della mobilità urbana e orientare politiche di prevenzione efficaci. La **Dashboard Interattiva degli Incidenti Stradali di Palermo** rappresenta un passo importante in questa direzione, trasformando oltre 28.000 eventi registrati dalla **[Polizia Municipale](https://www.comune.palermo.it/servizio/polizia-municipale/)** del Comune di Palermo tra il 2015 e il 2023 in uno strumento di analisi accessibile, visuale e interattivo.

### Cos'è e cosa fa

La dashboard è una **web application completamente client-side** che permette di esplorare, filtrare e visualizzare i dati sugli incidenti stradali avvenuti a Palermo negli ultimi nove anni. Non si tratta di una semplice mappa o di un report statico: è un vero e proprio **sistema di analisi territoriale e temporale** che consente a chiunque – amministratori pubblici, ricercatori, giornalisti o semplici cittadini – di interrogare i dati da molteplici prospettive.

Le funzionalità principali includono:

- **Mappa interattiva** con localizzazione geografica precisa degli incidenti
- **Filtri avanzati** per analizzare i dati per anno, mese, giorno, tipologia, zona, condizioni meteo e fascia oraria
- **Visualizzazioni grafiche dinamiche** (barre, linee, radar, heatmap calendari) che si aggiornano in tempo reale
- **Modalità di clustering geografico** per identificare le zone più critiche
- **Calendario personalizzato** per selezionare periodi specifici con estrema precisione
- **Export dei dati filtrati** in formato CSV e JSON

<iframe 
  src="https://palermohub.opendatasicilia.it/palermo_incidenti.html" 
  width="100%" 
  height="800" 
  frameborder="0" 
  style="border:0;" 
  allowfullscreen>
</iframe>

[Dashboard interattiva - visualizza a schermo intero](https://palermohub.opendatasicilia.it/palermo_incidenti.html)

### Tecnologie utilizzate

La web app è stata realizzata utilizzando tecnologie moderne e completamente open source. Per maggiori dettagli tecnici sull'architettura, le librerie utilizzate (MapLibre GL JS, Chart.js, PapaParse) e le scelte progettuali, è possibile consultare direttamente la sezione dedicata nell'applicazione: [**Tecnologie utilizzate**](https://palermohub.opendatasicilia.it/palermo_incidenti.html#tab-tecnologie). *(pulsante arancio in basso al centro)*

---

## I Dati: Un patrimonio di informazioni

### Panoramica del Dataset

Tra il 2015 e il 2023, sulle strade di Palermo la **[Polizia Municipale](https://www.comune.palermo.it/servizio/polizia-municipale/)** ha registrato **28.239 incidenti stradali**. Un numero che, tradotto in media, significa **oltre 8,6 incidenti al giorno** per nove anni consecutivi.

| **Indicatore** | **Valore** |
|---|---|
| Periodo coperto | 2015 – 2023 |
| Totale incidenti | 28.239 |
| Incidenti mappati | 23.487 (83,2%) |
| Ultimo aggiornamento | Dicembre 2023 |

### Qualità e copertura dei dati

Non tutti gli incidenti sono mappabili con la stessa precisione:

- **23.487 incidenti (83,2%)** hanno coordinate geografiche precise e sono visualizzabili sulla mappa
- **3.192 incidenti del 2019 (11,3%)** sono privi di geolocalizzazione, rendendo quell'anno problematico per analisi territoriali
- **1.560 incidenti (5,5%)** presentano coordinate esterne ai confini comunali. Si tratta di errori che potrebbero essere corretti tramite geocoding, qualora si disponesse di tempo sufficiente. Tuttavia, data la necessità di procedere speditamente in questa fase dell'analisi, si è scelto di escluderli dai vari dataset.

### Le quattro categorie di gravità

Gli incidenti sono classificati secondo quattro tipologie:

- **M – Mortali**: incidenti con esito fatale
- **R – Riserva**: incidenti con prognosi riservata, situazioni critiche
- **F – Feriti**: incidenti con feriti di varia gravità
- **C – Cose**: incidenti con soli danni materiali

La dashboard utilizza un sistema di colori per evidenziare immediatamente questa classificazione: rosso per i mortali, viola per le riserve, arancione per i feriti, verde per i danni alle cose.

### Focus 2023: La "Nuova Normalità"

Il 2023, ultimo anno disponibile, viene impostato come **anno di default** nella dashboard. Questo perché rappresenta un periodo post-pandemico in cui la circolazione è tornata ai livelli pre-Covid, rendendo i dati più rappresentativi per valutare l'attuale stato della sicurezza stradale palermitana.

---

## Funzionalità di analisi

### 1. Analisi territoriale multilivello

Il dataset include una stratificazione geografica articolata che permette di "zoomare" progressivamente sulle zone più critiche:

- **Circoscrizioni**: prima suddivisione amministrativa
- **Quartieri**: livello intermedio di dettaglio
- **UPL (Unità di Primo Livello)**: granularità massima

Filtrando una circoscrizione, si vedono automaticamente solo i quartieri inclusi; filtrando un quartiere, solo le relative UPL. Questo sistema a cascata facilita analisi mirate e progressive.

### 2. La Geografia del rischio

La funzionalità **"Top 25 Strade"** identifica le vie con il maggior numero di incidenti, mostrando per ciascuna:

- Indirizzo esatto dell'area critica
- Totale incidenti nella localizzazione
- Distribuzione per gravità (mortali, riserva, feriti, cose)
- Coordinate geografiche per la localizzazione sulla mappa

![strade](incidenti_04.jpg "Top 25 strade con più incidenti" ){class="centro}

Il **sistema di clustering geografico** evidenzia come gli incidenti tendano a concentrarsi in specifici punti critici: grandi incroci, rotonde complesse, arterie di scorrimento veloce.

![cluster](incidenti_05.jpg "Mappa clustering" ){class="centro}

### 3. Analisi temporale avanzata

#### Stagionalità

Il dataset classifica gli incidenti per **stagione**, permettendo di identificare se estate o inverno, primavera o autunno presentino rischi differenti – legati a condizioni meteo, flussi turistici, abitudini di mobilità.

#### Distribuzione settimanale

La suddivisione per **giorno della settimana** rivela pattern comportamentali: i weekend potrebbero mostrare dinamiche diverse (velocità più elevate, guida in stato di ebbrezza) rispetto ai giorni feriali (traffico pendolare, ore di punta).

Il filtro **Feriale/Weekend** sintetizza questa distinzione, evidenziando come il rischio cambi tra giorni lavorativi e di riposo.

#### Fasce orarie critiche

![fasce](incidenti_02.jpg "Fasce orarie critiche" ){class="centro}

La dashboard offre due livelli di granularità temporale:

- **Fascia oraria (4 fasce)**: divisione grossolana della giornata
- **Fascia oraria dettagliata (6 fasce)**: Alba, Mattina, Pranzo, Pomeriggio, Sera, Notte

A questo si aggiunge il filtro **"Ora di punta"** che identifica specificamente i momenti di maggiore congestione – tipicamente le ore 7-9 del mattino e 17-20 del pomeriggio.

### 4. Giorno vs Notte: Il Fattore visibilità

L'analisi comparativa **Giorno/Notte** include contatori in tempo reale che mostrano:

- Numero di incidenti diurni
- Numero di incidenti notturni
- Possibilità di filtrare l'uno o l'altro per analisi mirate

Il parametro **"Condizioni luce"** va oltre la semplice dicotomia temporale considerando: luce naturale piena, crepuscolo, buio con illuminazione artificiale funzionante o insufficiente, condizioni meteo che riducono la visibilità.

### 5. Strumenti di visualizzazione

#### Modalità mappa

- **Visualizzazione a punti**: ogni incidente come punto colorato per gravità
- **Clustering geografico**: aggregazione automatica delle zone ad alta densità
- **Heatmap**: visualizzazione della densità spaziale degli incidenti

#### Grafici analitici

- Trend annuale: evoluzione degli incidenti 2015-2023
- Distribuzione mensile: grafico radar dei mesi più rischiosi
- Analisi oraria: grafici per le fasce della giornata
- Confronti stagionali: bar chart per le quattro stagioni

#### Calendario interattivo

Una funzionalità innovativa che permette di:

- Selezionare un anno specifico
- Navigare per mesi
- Visualizzare giorni specifici con evidenza di quelli con incidenti
- Filtrare per giorno della settimana

---

## **La Grande novità: Chart builder**

### Crea il Tuo DatViz personalizzato

Una delle funzionalità più innovative della dashboard è il **Chart builder**, un potente strumento interattivo che permette di creare visualizzazioni personalizzate dei dati. Con pochi clic è possibile generare grafici professionali scegliendo tra:

- **8 tipologie di grafico**: barre, linea, torta, ciambella, radar, polare, scatter e bubble
- **13 dimensioni di analisi**: dalle dimensioni temporali (anno, mese, stagione) a quelle territoriali (circoscrizione, quartiere, UPL) e orarie (fasce della giornata, condizioni di luce)
- **Personalizzazione completa**: colori (automatici, singoli o sfumati), stili (4 preset rapidi o controlli avanzati), orientamento e animazioni
- **Export professionale**: ogni grafico può essere scaricato come immagine PNG ad alta risoluzione (800×600px) completa di titolo, filtri applicati, fonte dati e crediti

### Casi d'uso pratici

Il Chart Builder applica automaticamente tutti i filtri attivi nella dashboard e consente di creare visualizzazioni perfette per report istituzionali, presentazioni, studi accademici o infografiche per social media.

Per una guida completa al funzionamento, esempi pratici, casi d'uso e suggerimenti per creare grafici efficaci, consultare la documentazione dettagliata disponibile nell'applicazione: [**Crea il tuo DataViz**](https://palermohub.opendatasicilia.it/palermo_incidenti.html#tab-chart-builder). *(pulsante arancio in basso al centro)*

![Chart builder](incidenti_03.jpg "Chart builder" ){class="centro}
---

## Contesto demografico e impatto

Palermo conta circa **650.000 abitanti** nell'area comunale. Con quasi 30.000 incidenti in 9 anni, statisticamente:

- **Ogni 23 palermitani, uno è stato coinvolto in un incidente** nel periodo considerato
- Considerando che non tutti i palermitani guidano (escludendo minori, anziani non automuniti, etc.), la proporzione reale tra conducenti/passeggeri coinvolti è ancora più alta

## Limiti e criticità

È importante evidenziare alcune criticità del dataset:

1. **Il buco nero del 2019**: 3.192 incidenti senza coordinate rendono parziale qualsiasi analisi di quell'anno
2. **Sottoregistrazione possibile**: alcuni incidenti minori potrebbero non essere rilevati
3. **Mancanza di dati su vittime**: il dataset classifica per gravità ma non specifica il numero esatto di morti e feriti per incidente
4. **Assenza di informazioni su cause**: non sappiamo se gli incidenti siano dovuti a velocità, alcol, distrazione o condizioni stradali

---

## Ringraziamenti

Si ringrazia il **[Comune di Palermo](https://www.comune.palermo.it/)** e la **[Polizia Municipale](https://www.comune.palermo.it/servizio/polizia-municipale/)** per la pubblicazione dei dati in formato aperto, rendendo possibile questa analisi e sensibilizzazione.

Un grazie speciale a **[Andrea Borruso](https://www.linkedin.com/in/andreaborruso/)** e **[Totò Fiandaca](https://www.linkedin.com/in/salvatore-fiandaca-23a1a250/)** per il prezioso supporto tecnico, per la loro disponibilità e per aver condiviso con generosità competenze ed esperienza.

---

## Responsabilità e Disclaimer

**I dati sono forniti "as is".**

L'utente accetta i dati nella loro condizione attuale e si assume la responsabilità del loro utilizzo.

**Cosa significa "as is"?**

I dati sono forniti nello stato in cui si trovano, **senza garanzie di alcun tipo** (esplicite o implicite) riguardo:

- Completezza delle informazioni
- Accuratezza o precisione dei dati
- Idoneità per uno scopo specifico
- Assenza di errori o omissioni

**L'elaborazione è a scopo informativo e di sensibilizzazione.**

Per informazioni ufficiali contattare la [Polizia Municipale di Palermo](https://www.comune.palermo.it/servizio/polizia-municipale/).

---

## Link utili

- **Dashboard**: [Incidenti Stradali – Palermo 2015-2023 • Dashboard Interattiva](https://palermohub.opendatasicilia.it/palermo_incidenti.html)
- **Fonte Dati**: [dati.gov.it](https://www.dati.gov.it/view-dataset?Cerca=incidenti+palermo)


<hr>
**Disclaimer:** Le informazioni visibili e condivise non comportano la visualizzazione di dati sensibili. Data la natura esclusivamente informativa degli elaborati grafici e dei testi riportati, questi non costituiscono atti ufficiali. Per accedere agli atti ufficiali si rinvia agli elaborati definitivi allegati alle specifiche deliberazioni.