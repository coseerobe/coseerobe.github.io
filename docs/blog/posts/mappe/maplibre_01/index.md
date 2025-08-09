---
title: DEMO - Palermo 3D pmtiles
description: DEMO - Palermo 3D pmtiles - Rielaborazione dati OpenDataSicilia
draft: false
date: 2024-12-30T12:00:00
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
social_image: https://palermohub.opendatasicilia.it/pmtiles/social_card.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
.iframe-container {width: 100%;  height:auto;}
.full-space-iframe { width: 100%;  height: 650px;  border: none;   display: block;}
</style>
# Esplorare Palermo in 3D con PMTiles e MapLibre

[![3D](maplibre.jpg "DEMO - Palermo 3D pmtiles - Rielaborazione dati OpenDataSicilia" ){class="crop gra" align=left}](index.md)

## Una Mappa 3D Innovativa

La web app disponibile all'[indirizzo](https://palermohub.opendatasicilia.it/pmtiles/index_pntiles_pa.html) rappresenta un esempio eccellente di come le moderne tecnologie web possano trasformare i dati geografici aperti in esperienze interattive coinvolgenti.  Questa applicazione utilizza una combinazione di tecnologie all'avanguardia per offrire una visualizzazione tridimensionale del territorio palermitano.<!-- more --> 

## Le Tecnologie alla Base

### MapLibre GL JS
MapLibre GL JS è una libreria TypeScript che utilizza WebGL per renderizzare mappe interattive da tiles vettoriali in un browser. Questa libreria open-source è il motore che alimenta la visualizzazione della mappa, garantendo performance elevate e rendering fluido anche con geometrie complesse.

### PMTiles: Il Formato del Futuro
PMTiles è progettato per essere visualizzato direttamente nei browser web in congiunzione con una libreria JavaScript per il rendering delle mappe, inclusa MapLibre GL JS - la libreria raccomandata per costruire esperienze fluide e personalizzazioni di stile.

PMTiles è progettato per dati tiled. Cioè, dati dove un file interno rappresenta un piccolo quadrato da qualche parte su una mappa, di solito rappresentando la griglia Web Mercator. Questo formato innovativo permette di caricare solo le porzioni di dati (tiles) necessarie per visualizzare l'area attualmente visibile sullo schermo, riducendo il tempo di caricamento e il consumo di risorse.

## Caratteristiche Tecniche della Mappa 3D

### Rappresentazione del Territorio
La web app sfrutta le capacità 3D di MapLibre per rappresentare:

1. **Modello Digitale di Elevazione (DEM)**: Il terreno viene renderizzato in tre dimensioni utilizzando dati altimetrici, creando un paesaggio realistico che mostra le colline e le valli caratteristiche del territorio palermitano.

2. **Edificato Tridimensionale**: Gli edifici vengono estrusi in base ai loro attributi geometrici, creando un skyline urbano fedele alla realtà. MapLibre GL JS supporta nativamente la visualizzazione di edifici in 3D, permettendo rappresentazioni accurate dell'ambiente costruito.

### Vantaggi Tecnologici

- **Performance Ottimizzate**: Grazie al formato PMTiles e alle capacità di WebGL, la mappa carica rapidamente solo i dati necessari per l'area visualizzata
- **Interattività Fluida**: La navigazione 3D è responsiva e intuitiva, permettendo rotazione, zoom e pan senza interruzioni
- **Efficienza di Banda**: Il caricamento progressivo delle tiles riduce significativamente il consumo di dati

## Un Esempio di Civic Technology

Questo progetto rappresenta un eccellente esempio di come i civic hacker e i cittadini attivi possano valorizzare gli open data pubblici. L'Atlante delle Carte Tecniche storiche di Palermo, la Variante Generale (2004) vigente di Palermo, la Cartografia con Ortofoto sono tra le mappe più richieste, dimostrando l'importanza di rendere accessibili questi dati in formati moderni e interattivi.

La combinazione di PMTiles con MapLibre GL JS e le funzionalità 3D rappresenta lo stato dell'arte nella visualizzazione web di dati geospaziali, offrendo un'esperienza utente ricca e performante senza richiedere plugin o software aggiuntivi.

## Riferimenti
[MapLibre](https://maplibre.org/)<br>
[MapLibre GL JS](https://maplibre.org/maplibre-gl-js/docs/guides/leaflet-migration-guide/)<br>
[leafmap](https://leafmap.org/)<br>
[bert](https://bertt.wordpress.com/)<br>


---
<br>

<div style="position: relative; width: 100%; height: 600px; border: 1px solid #ccc; border-radius: 8px; overflow: hidden;">
    <iframe 
        src="https://palermohub.opendatasicilia.it/pmtiles/index_pntiles_pa.html" 
        width="100%" 
        height="100%" 
        frameborder="0" 
        allowfullscreen
        title="Mappa 3D di Palermo - PalermoHub">
    </iframe>
    
    <!-- Pulsante per aprire in nuova pagina -->
    <a href="https://palermohub.opendatasicilia.it/pmtiles/index_pntiles_pa.html" 
       target="_blank" 
       rel="noopener noreferrer"
       style="position: absolute; 
              top: 10px; 
              right: 10px; 
              background: rgba(0,0,0,0.8); 
              color: white; 
              padding: 8px 12px; 
              text-decoration: none; 
              border-radius: 4px; 
              font-size: 12px; 
              font-family: Arial, sans-serif;
              z-index: 1000;
              transition: background 0.3s ease;"
       onmouseover="this.style.background='rgba(0,0,0,0.9)'"
       onmouseout="this.style.background='rgba(0,0,0,0.8)'">
        🔗 Apri a schermo intero
    </a>
</div>

--- 

**Disclaimer:** Le informazioni visibili e condivise non comportano la visualizzazione di dati sensibili. Data la natura esclusivamente informativa degli elaborati grafici e dei testi riportati, questi non costituiscono atti ufficiali. Per accedere agli atti ufficiali si rinvia agli elaborati definitivi allegati alle specifiche deliberazioni.