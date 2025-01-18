---
title: DEMO - Variante Generale e Particelle catastali - pmtiles
description: DEMO - Variante Generale e Particelle catastali - pmtiles  - Rielaborazione dati OpenDataSicilia
draft: false
date: 2025-01-02T12:00:00
authors:
  - gbvitrano
categories:
  - Mappe
tags:
  - Crisi idrica
  - Sicilia
  - Palermo
  - Amap
  - Distreii
social_image: https://palermohub.opendatasicilia.it/pmtiles/social_card_04.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
.iframe-container {width: 100%;  height:auto;}
.full-space-iframe { width: 100%;  height: 650px;  border: none;   display: block;}
</style>
[![Distretti ](https://palermohub.opendatasicilia.it/pmtiles/social_card_04.jpg "DEMO - Variante Generale e Particelle catastali - pmtiles  - Rielaborazione dati OpenDataSicilia" ){class="crop gray off" align=right}](index.md)


<br><br><br><br><br><br>
Coming soon....<!-- more --> 

# Demo 1

<div class="iframe-container">
<iframe class="full-space-iframe" width="100%" height="650px" frameborder="0" allowfullscreen  src="https://palermohub.opendatasicilia.it/pmtiles/demo_prg_catasto.html#12.3/38.1219/13.36462/-46.4/60"></iframe>
</div>  <br>
<hr>
 <br>
# Nuova mappa con particelle catastali e strumenti urbanistici vigenti di Palermo

La nuova versione è completamente riprogettata e ottimizzata, grazie all'aiuto di [@deepseek_ai](https://x.com/deepseek_ai), per offrire una migliore esperienza utente.

## Principali miglioramenti

### Gestione avanzata dei tooltip
La novità più significativa riguarda la gestione dei tooltip. Nella versione precedente, in presenza di elementi sovrapposti nei livelli PMTiles, i tooltip si sovrapponevano creando confusione. Ora, lo script genera automaticamente un tooltip unificato che integra in modo ordinato le informazioni di tutti gli elementi presenti in un punto specifico.
Inoltre, è stato integrato un pratico modulo di ricerca che permette di individuare rapidamente fogli e particelle specifiche.
Infine è stata implementata una finestra dinamica che visualizza una mappa satellitare, la quale si sincronizza automaticamente con la mappa principale. Questa funzionalità inquadra il centro dell'area visualizzata sul monitor e può essere attivata mediante un pulsante posizionato nell'angolo inferiore sinistro dell'interfaccia.

### Aspetti tecnici

Il codice è stato completamente ristrutturato per garantire:

-    Maggiore stabilità e riduzione dei bug
-    Performance ottimizzate
-    Migliore gestione della visualizzazione dei dati
-    Modulo di ricerca per Foglio e particella catastale
-    Finestra dinamica per visualizzare la mappa satellitare

<div class="iframe-container">
<iframe class="full-space-iframe" width="100%" height="650px" frameborder="0" allowfullscreen  src="https://palermohub.opendatasicilia.it/pmtiles/prg_part_catastali_pdf.html#12/38.14074/13.33225"></iframe> 
</div> <br>
<hr>

## Ricerca geografica dellee particelle catastali

Il layer **Particelle Catastali** viene esposto in formato PMTiles.

Il PMTiles è un formato di file progettato per archiviare e servire dati geospaziali, come mappe vettoriali o raster, in modo efficiente. È un formato basato su tessere (tiles), che permette di suddividere i dati in piccole porzioni (tiles) per un accesso rapido e selettivo.
La particolarità di PMTiles è che è un formato monolitico, cioè tutti i dati sono contenuti in un unico file, a differenza di altri formati che richiedono molteplici file separati. Questo lo rende più semplice da gestire e distribuire, ad esempio su un server web o su un CDN (Content Delivery Network).

### Cerca una Particella
Viste le caratteristiche del PMTiles, Durante la ricerca con PMTiles, è necessario che la particella da visualizzare sia compresa nell'area mostrata sullo schermo del proprio dispositivo (PC desktop o mobile). In caso contrario, poiché il dato non sarà stato caricato, verrà mostrato un messaggio di errore.

### Ricerca con PMTiles
Dato che il formato **PMTiles** è progettato per caricare solo le **porzioni di dati** (tiles) necessarie per visualizzare l'area attualmente visibile sullo schermo (monitor del PC o display del dispositivo), è fondamentale assicurarsi che la particella o l'oggetto geospaziale richiesto rientri nell'area visualizzata.

### Come funziona il processo:
1.    Visualizzazione dell'area: Quando apri una mappa, il software (ad esempio, un'applicazione web basata su MapLibre o Leaflet) carica solo le tiles corrispondenti all'area visibile sullo schermo. Questo riduce il tempo di caricamento e il consumo di risorse.
2.    Ricerca di una particella: Se cerchi una particella o un oggetto specifico, il sistema verifica se i dati relativi a quell'oggetto sono già stati caricati (cioè, se rientrano nelle tiles visualizzate).
3.    Messaggio di errore: Se la particella richiesta non rientra nell'area visualizzata, il sistema non avrà caricato i dati necessari per rispondere alla richiesta. In questo caso, verrà restituito un messaggio di errore, ad esempio:
"Dato non disponibile: la particella richiesta non è visibile nell'area corrente."

### Come evitare l'errore:
-    Zoom o spostamento: Assicurati di zoommare o spostare la mappa in modo che l'area contenente la particella richiesta sia visibile sullo schermo.
-     Ricerca geografica: Se l'applicazione lo supporta, utilizza una funzione di ricerca geografica che carica automaticamente l'area corretta quando cerchi una particella

In sintesi, il formato PMTiles è ottimizzato per l'efficienza, ma richiede che l'area di interesse sia visibile per accedere ai dati corretti. Se non lo è, il sistema non può recuperare le informazioni necessarie, generando un messaggio di errore.


## Stampa pdf

Una volta effettuata la ricerca della particella catastale tramite il pulsante 'Cerca', comparirà una nuova icona sottostante.

Cliccando su questa icona, il sistema genererà automaticamente un documento PDF che include una mappa dettagliata con la particella evidenziata.

Il documento contiene inoltre tutte le informazioni catastali della particella selezionata e i relativi dati urbanistici, compresi la zonizzazione dell'area e gli eventuali vincoli esistenti.

**N.B. Non è possibile generare file pdf quando si usa un device mobile orientato in verticale (Portait)**

Per generare PDF con le informazioni richieste, ruotare il dispositivo in orientamento orizzontale (modalità landscape).

<br>
<hr>

### Ringraziamenti
Un sentito ringraziamento va a [@aborruso](https://x.com/aborruso) e [@totofiandaca](https://x.com/totofiandaca), i cui insegnamenti e la costante condivisione di conoscenze hanno contribuito in modo determinante alla realizzazione di questo progetto. Il loro supporto mi permette di implementare e migliorarmi nel campo della cartografia digitale.
<hr>
 **Disclaimer:** I contenuti presenti in questa sezione, compresi testi ed elementi grafici, hanno carattere puramente informativo e divulgativo.
Non sono presenti dati personali o sensibili. Si precisa che questi materiali non costituiscono documenti ufficiali né hanno alcun valore legale.
Per consultare la documentazione ufficiale e legalmente vincolante, si prega di fare riferimento agli atti definitivi allegati alle relative deliberazioni degli organi competenti.