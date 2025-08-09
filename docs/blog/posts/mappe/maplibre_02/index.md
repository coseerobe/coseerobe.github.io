---
title: Variante Generale e Particelle catastali - pmtiles
description: Variante Generale e Particelle catastali - pmtiles  - Rielaborazione dati OpenDataSicilia
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
social_image: https://palermohub.opendatasicilia.it/pmtiles/social_card_05.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
.iframe-container {width: 100%;  height:auto;}
.full-space-iframe { width: 100%;  height: 650px;  border: none;   display: block;}
</style>
[![Distretti ](https://palermohub.opendatasicilia.it/pmtiles/social_card_05.jpg "DEMO - Variante Generale e Particelle catastali - pmtiles  - Rielaborazione dati OpenDataSicilia" ){class="crop gray off" align=right}](index.md)

# La Rivoluzione digitale dei dati Urbanistici e Catastali
**Scopri il nuovo strumento interattivo per esplorare il territorio di Palermo con dati aggiornati e funzionalità avanzate**

ZTO e Particelle catastali è una web application innovativa sviluppata da OpenDataSicilia che rappresenta una vera rivoluzione nell'accesso ai dati territoriali del capoluogo siciliano. <!-- more --> Si tratta di mappa interattiva che integra informazioni urbanistiche e catastali in un'unica piattaforma digitale, offrendo agli utenti - professionisti, pubbliche amministrazioni e cittadini - uno strumento potente e gratuito per esplorare il territorio palermitano. 

<!-- Iframe per incorporare Palermo Hub -->
<div style="width: 100%; max-width: 1200px; margin: 0 auto; border: 2px solid #e1e5e9; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
  <div style="background-color: #f8f9fa; padding: 10px 15px; border-bottom: 1px solid #e1e5e9; font-family: Arial, sans-serif; font-size: 14px; color: #495057;">
    <strong>📍 Palermo Hub</strong> - Mappa interattiva dei dati urbanistici e catastali di Palermo
    <a href="https://palermohub.opendatasicilia.it/pmtiles/prg_part_catastali_pdf.html" 
       target="_blank" 
       style="float: right; color: #007bff; text-decoration: none; font-size: 12px;">
      🔗 Apri in nuova finestra
    </a>
  </div>
  <iframe 
    src="https://palermohub.opendatasicilia.it/pmtiles/prg_part_catastali_pdf.html" 
    width="100%" 
    height="600" 
    frameborder="0" 
    scrolling="no"
    style="display: block; border: none;"
    title="Palermo Hub - Mappa interattiva dati urbanistici e catastali"
    loading="lazy">
    <p>Il tuo browser non supporta gli iframe. 
       <a href="https://palermohub.opendatasicilia.it/pmtiles/prg_part_catastali_pdf.html" target="_blank">
         Clicca qui per accedere direttamente alla mappa
       </a>
    </p>
  </iframe>
</div>


## Tecnologia PMTiles: Efficienza e Performance

Il cuore tecnologico dell'applicazione si basa sul formato **PMTiles**, una tecnologia all'avanguardia per la gestione dei dati geospaziali. A differenza dei formati tradizionali che richiedono molteplici file separati, PMTiles utilizza un approccio monolitico che racchiude tutti i dati in un unico file, garantendo:

- **Accesso rapido e selettivo** attraverso la suddivisione in tessere (tiles)
- **Facilità di distribuzione** su server web e CDN
- **Ottimizzazione delle performance** caricando solo le porzioni necessarie per l'area visualizzata
- **Gestione efficiente delle risorse** del dispositivo utilizzato

## Funzionalità Principali

### 1. Ricerca Intelligente
L'applicazione integra un modulo di ricerca avanzato che permette di individuare rapidamente fogli e particelle catastali specifiche. Il sistema richiede che la particella cercata rientri nell'area visualizzata sullo schermo per poter accedere ai dati.

### 2. Tooltip Unificati
Una delle innovazioni più significative riguarda la gestione dei tooltip. Il nuovo sistema genera automaticamente tooltip unificati che integrano in modo ordinato tutte le informazioni degli elementi presenti in un punto specifico, eliminando la confusione precedentemente causata dalla sovrapposizione di più tooltip.

### 3. Vista Satellitare Sincronizzata
È stata implementata una finestra dinamica con mappa satellitare che si sincronizza automaticamente con la mappa principale, attivabile tramite un pulsante nell'angolo inferiore sinistro dell'interfaccia.

### 4. Generazione PDF Automatica
Una volta individuata la particella catastale desiderata, il sistema può generare automaticamente un documento PDF contenente:
- Mappa dettagliata con la particella evidenziata
- Informazioni catastali complete
- Dati urbanistici correlati
- Zonizzazione dell'area secondo il P.R.G.
- Vincoli esistenti

*Nota: La generazione PDF non è disponibile su dispositivi mobili in orientamento verticale.*

## Dati e Fonti

L'applicazione utilizza dati provenienti da fonti ufficiali e aggiornate:

- **Dati catastali**: S.I.T.R. Sicilia (aggiornati a gennaio 2025)
- **Zonizzazione urbanistica**: Comune di Palermo (Variante Generale al P.R.G. - 2003/2004)
- **Piano Particolareggiato Esecutivo** del centro storico (1993)
- **Licenza**: CC-BY 4.0 per tutti i dataset utilizzati

## Novità Legislative 2025

L'applicazione si inserisce nel contesto della recente riforma che, dal 1° gennaio 2025, ha reso gratuito l'accesso telematico alle banche dati ipotecarie e catastali, rappresentando una semplificazione importante per tutti gli operatori del settore.

## Impatto e Utilità

Palermo Hub democratizza l'accesso all'informazione territoriale, offrendo:
- **Trasparenza** nell'accesso ai dati pubblici
- **Efficienza** per professionisti del settore
- **Facilità di consultazione** per i cittadini
- **Strumento di supporto** per le decisioni amministrative

L'applicazione rappresenta un esempio virtuoso di come l'open data possa trasformarsi in servizi concreti per la comunità, facilitando la comprensione del territorio e supportando processi decisionali informati.

## Sviluppo e Riconoscimenti

Il progetto è stato completamente riprogettato e ottimizzato grazie alla collaborazione con DeepSeek AI, mentre un ringraziamento speciale va ad [@aborruso](https://x.com/aborruso) e [@totofiandaca](https://x.com/totofiandaca), per il loro contributo formativo e la condivisione di conoscenze nel campo della cartografia digitale.

---

*Palermo Hub dimostra come l'innovazione tecnologica, unita all'impegno per l'open data, possa creare strumenti concreti al servizio del territorio e della comunità.*

---

 **Disclaimer:** I contenuti presenti in questa sezione, compresi testi ed elementi grafici, hanno carattere puramente informativo e divulgativo.
Non sono presenti dati personali o sensibili. Si precisa che questi materiali non costituiscono documenti ufficiali né hanno alcun valore legale.
Per consultare la documentazione ufficiale e legalmente vincolante, si prega di fare riferimento agli atti definitivi allegati alle relative deliberazioni degli organi competenti.