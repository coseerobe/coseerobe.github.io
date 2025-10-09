---
title: PalermoHub 2.0
description: PalermoHub
draft: false
date: 2025-09-15T12:00:00
authors:
  - gbvitrano
categories:
  - Mappe
tags:
  - PalermoHub
  - Opendata
  - Palermo
  - Mappe
social_image: assets/img/social/social_card_ph.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
</style>
[![PalermoHub](social_card_ph.jpg "PalermoHub" ){class="crop gray off" align=right}](index.md)


## È arrivato un momento speciale per PalermoHub!

Dopo quasi 8 anni di vita intensa (dal 2017), con decine di mappe realizzate su temi diversi e migliaia di visualizzazioni che hanno accompagnato la scoperta della nostra bella città, abbiamo mandato in pensione la prima versione.
### Il momento del cambiamento <!-- more --> 
Il cuore della prima versione di **PalermoHub** si basa su **Simile Exhibit**, un'applicazione che ai suoi tempi era davvero innovativa, ma che purtroppo non viene più sviluppata da anni. Come spesso accade nel mondo digitale, anche le tecnologie più brillanti invecchiano e oggi il nostro fedele compagno mostra inevitabilmente il peso del tempo. Era arrivato il momento di fare il grande salto!
La sfida non era da poco: dovevo riprogettare completamente il sistema preservando l'anima di **PalermoHub** - quella veste grafica pulita e funzionale che tutti conoscete. Le mappe sono sempre state il nostro punto di forza, ma proprio questa caratteristica di "contenitore universale" ha reso piuttosto complesso adattare il nuovo template a tutte le pagine esistenti.

[![PalermoHub](pa_hub_new.png "PalermoHub" ){class="centro nobox" }](https://PalermoHub.opendatasicilia.it/)

### L'avventura della riprogettazione
La parte più affascinante? Il dialogo con [Claude AI (Anthropic)](https://claude.ai/)! Ho semplicemente descritto a parole quello che avevo in mente, i problemi da risolvere e gli obiettivi da raggiungere. Insieme abbiamo analizzato diverse strade, valutando pro e contro di ogni approccio tecnologico. Alla fine, la scelta è caduta sul [JavaScript Client-Side](https://www.perplexity.ai/search/in-cosa-consisste-la-tecnica-j-Bd04pV_3QbSE_iSR9XFQuQ) - una soluzione elegante che ci permette di:

-    Mantenere tutti i link che utilizzate abitualmente (nessun collegamento rotto!)

-    Preservare la SEO faticosamente costruita in questi anni

-    Garantire prestazioni migliori e una navigazione più fluida

-    Aprire le porte a nuove funzionalità che avevo sempre sognato di implementare

### Il nuovo **PalermoHub** è realtà
E così, dopo settimane di progettazione, coding e test, è nato il nuovo **PalermoHub**! Stesso spirito, stessa passione per la nostra città, ma con un motore completamente rinnovato sotto il cofano. Non vedo l'ora di condividere con voi tutte le novità e di continuare questo viaggio alla scoperta di Palermo insieme.
<br>
Il sito, in particolare la homepage con il sistema di ricerca, filtri e impaginazione, è stato sviluppato attraverso una collaborazione human-[Claude AI (Anthropic)](https://claude.ai/), che ha supportato la progettazione dell’architettura modulare, l’ottimizzazione del codice e l’implementazione di funzionalità avanzate di visualizzazione.

[![**PalermoHub**](social_card_ph.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)


## Una storia che non ci aspettavamo
Quando abbiamo iniziato non immaginavamo che **PalermoHub** potesse diventare un punto di riferimento per studenti, docenti tecnici, amministratori e semplici cittadini curiosi. È nato con l'intento molto più modesto di mettere ordine alle mappe che ODS realizzava pian piano, quasi per necessità interna.
Oggi guardiamo indietro e ci sono quasi **200 mappe!** Un numero che ci sorprende ogni volta che lo pronunciamo. Tutte elaborate partendo da open data e realizzate dalla passione dei civic hacker, rappresentano un esempio virtuoso di come si possano trasformare dati pubblici - spesso aridi e difficili da interpretare - in veri e propri strumenti di conoscenza del territorio. Mappe accessibili e comprensibili per cittadini, amministratori e ricercatori.
**PalermoHub** è diventato, senza che ce ne accorgessimo completamente, un **laboratorio di democrazia digitale** che dimostra ogni giorno le incredibili potenzialità degli open data quando vengono valorizzati e resi vivi dalla comunità. Una dimostrazione pratica che i dati aperti non sono solo numeri in tabelle, ma possono diventare strumenti di partecipazione e conoscenza collettiva.

*Ecco perché questo rilancio non è solo un aggiornamento tecnico, ma il riconoscimento di una responsabilità: continuare a essere quel ponte tra istituzioni, dati e cittadinanza che tanto serve alla nostra città.*

---

## Come Funziona la nuova piattaforma - Guida utente
## Che cos'è PalermoHub

PalermoHub è come una grande biblioteca digitale piena di mappe interattive di Palermo e della Sicilia. Invece di libri sugli scaffali, qui trovi centinaia di mappe che mostrano tutto quello che può interessarti della città: dal traffico ai monumenti, dalla geologia alle piste ciclabili.

Il bello è che tutte queste mappe sono create con "dati aperti" - informazioni che il Comune, la Regione e altri enti pubblici mettono a disposizione di tutti gratuitamente. È come se la città aprisse i suoi archivi e dicesse: "Ecco tutto quello che sappiamo, usate pure questi dati per creare qualcosa di utile".

## Il primo incontro: Cosa succede quando arrivi sul sito

### Il caricamento intelligente

Quando apri PalermoHub per la prima volta, succede qualcosa di interessante dietro le quinte. Il sito scarica un file che contiene tutte le informazioni sulle mappe disponibili - un po' come scaricare l'indice di una biblioteca. 

Ma ecco la parte intelligente: una volta scaricato, questo "indice" viene conservato nella memoria del tuo browser per 30 minuti. È come se il bibliotecario ti desse una copia dell'elenco dei libri da tenere con te, così la prossima volta non deve rifarlo da capo. Risultato? Il sito si carica molto più velocemente nei tuoi prossimi accessi.

### Lo slider delle mappe in evidenza

In cima alla pagina trovi uno slider che mostra a rotazione 5 mappe interessanti, di solito le più recenti. Funziona come una vetrina di un negozio: ti fa vedere subito cosa c'è di nuovo e interessante. Puoi cliccare sulle frecce per navigare manualmente, o lasciare che scorra da solo ogni 5 secondi.

[![PalermoHub](funz_01.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)

-    1 Statistiche;
-    2 Selettori filtri, per Categoria, Territorio, Fonte dati, anno, tag e autore/i delle mappe;
-    3 Ricerca intelligente (Smart search)trova le mappe specifiche attraverso parole chiave
-    4 Interfaccia che mostra il numero di risultati trovati con indicazioni chiave;
-    5 Strumenti per la visualizzazione e la navigazione nell’elenco delle mappe:
-    6 Indicazione dell’ultimo aggiornamento

## Come cercare quello che ti interessa

### La ricerca intelligente

La barra di ricerca di PalermoHub non è una ricerca normale. È più come avere un assistente che capisce quello che vuoi anche se non lo dici perfettamente.

**Come funziona in pratica:**

- **Tollera gli errori**: Se scrivi "traffico" invece di "traffico", ti trova comunque quello che cerchi
- **Capisce i sinonimi**: Se cerchi "biciclette" ti trova anche le mappe delle "bici" e delle "piste ciclabili"  
- **Suggerisce mentre scrivi**: Dopo che hai digitato almeno 2 lettere, inizia a mostrarti i risultati più probabili

**Il sistema di punteggio**: Ogni mappa riceve un "voto" basato su quanto corrisponde alla tua ricerca:
- Se la parola è nel titolo → voto alto
- Se è nella descrizione → voto medio  
- Se è nei tag o nelle informazioni aggiuntive → voto più basso

I risultati vengono ordinati dal voto più alto al più basso, così trovi subito quello che cerchi.

[![PalermoHub](funz_02.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)

### I filtri: come un sistema di classificazione

Oltre alla ricerca, puoi usare i filtri per restringere i risultati. È come in una biblioteca dove puoi cercare per argomento, autore, anno di pubblicazione:

- **Categoria**: Trasporti, Ambiente, Cultura, ecc.
- **Territorio**: Palermo Centro, Periferie, Provincia, Sicilia
- **Anno**: Quando è stata creata la mappa
- **Autore**: Chi l'ha realizzata
- **Fonte dati**: Da dove vengono i dati (Comune, Regione, ecc.)
- **Tag**: Parole chiave associate

**La magia dei filtri interconnessi**: Quando selezioni un filtro, gli altri si aggiornano automaticamente. Se scegli "Trasporti" come categoria, il filtro "Territorio" ti mostrerà solo le zone per cui esistono mappe sui trasporti. È come se il sistema eliminasse automaticamente le combinazioni che non portano a nessun risultato.

### Le statistiche in tempo reale

In alto vedi sempre quante mappe ci sono in totale, quante categorie, quanti autori e - soprattutto - quanti risultati corrispondono ai tuoi filtri attuali. È un modo per capire subito se stai restringendo troppo la ricerca o se hai ancora molte opzioni tra cui scegliere.

## Come navigare tra le mappe

### Due modi di vedere i risultati

PalermoHub ti offre due modi per esplorare le mappe:

**Vista a Griglia** (predefinita): Le mappe sono mostrate come delle "carte" con immagine, titolo e informazioni principali. È più visuale e ti permette di vedere subito di cosa si tratta.

[![PalermoHub](funz_03.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)

**Vista Lista**: Informazioni più dettagliate disposte in righe, utile quando vuoi confrontare rapidamente molte mappe.

[![PalermoHub](funz_04.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)

### Paginazione vs scorrimento infinito

Puoi scegliere come navigare tra i risultati:

**Paginazione** (predefinita): I risultati sono divisi in pagine da 12, 24, 36 o 48 mappe ciascuna. È come sfogliare un catalogo: vedi chiaramente dove sei (pagina 3 di 15) e puoi saltare direttamente a una pagina specifica.

**Scorrimento infinito**: Tutte le mappe si caricano in una lunga lista che puoi scorrere all'infinito. Comodo per esplorare senza pensare alle pagine.

### Come arire le mappe

Ogni mappa può essere aperta in diversi modi:

- **Click normale**: Si apre nella stessa finestra
- **Ctrl+Click** (o Cmd+Click su Mac): Si apre in una nuova finestra
- **Click con rotella del mouse**: Si apre in una nuova scheda

È lo stesso comportamento che conosci dai link normali del web.

## Le Funzionalità intelligenti

### I breadcrumbs 

In cima alla pagina, quando hai dei filtri attivi, appaiono delle "etichette" che mostrano il percorso che hai seguito. È come le briciole di pane di Hansel e Gretel: ti permettono di vedere dove sei e di tornare indietro facilmente.

Per esempio, se hai filtrato per "Categoria: Trasporti" e "Anno: 2024", vedrai due etichette cliccabili. Puoi cliccare sulla X di una di esse per rimuovere solo quel filtro, mantenendo gli altri.

[![PalermoHub](funz_05.jpg "PalermoHub" ){class="centro}](https://PalermoHub.opendatasicilia.it/)

### La sincronizzazione tra componenti

Se usi la ricerca nella barra principale e poi scorri in fondo alla pagina, troverai che anche la barra di ricerca nel footer si è aggiornata automaticamente con lo stesso termine. È un dettaglio piccolo, ma rende l'esperienza più fluida.

### L'ordinamento intelligente

Le mappe sono ordinate per data, con le più recenti in cima. Ma puoi invertire l'ordine con un click sul pulsante "Data". È utile per vedere l'evoluzione storica dei dati o per trovare informazioni di un periodo specifico.

## Come il sito si adatta a te

### Modalità scura/chiara

PalermoHub rileva automaticamente se preferisci la modalità scura o chiara dal tuo sistema operativo. Ma puoi anche cambiarla manualmente con l'interruttore nel menu. La preferenza viene ricordata per le prossime visite.

### Responsive design: dallo schermo grande al telefono

Il sito si adatta automaticamente al dispositivo che stai usando:

**Su computer**: Layout a più colonne, tutti i controlli visibili, menu orizzontale

**Su tablet**: Layout ottimizzato per il touch, dimensioni più grandi per i pulsanti

**Su smartphone**: 
- Menu a hamburger (le tre lineette)
- Ricerca e filtri ripiegabili
- Layout a colonna singola
- Controlli ottimizzati per il dito

### Accessibilità

PalermoHub è progettato per essere usabile da tutti:

- **Navigazione da tastiera**: Puoi usare Tab, Enter, spazio e le frecce per navigare
- **Screen reader**: Le informazioni sono organizzate per essere lette correttamente dai software per non vedenti
- **Contrasti**: I colori rispettano gli standard di accessibilità per chi ha difficoltà visive

## La tecnica... Spiegata in modo semplice

### Come vengono gestiti i dati

Tutte le informazioni sulle mappe sono contenute in un file CSV (come un foglio di calcolo) che viene aggiornato regolarmente. Quando apri il sito:

1. Il browser controlla se ha già una copia recente dei dati
2. Se sì, li usa immediatamente (velocità massima)
3. Se no, scarica la versione aggiornata
4. I dati vengono "processati" per creare gli indici di ricerca

### Il sistema di ricerca

Quando digiti nella barra di ricerca, succede questo:

1. Il sistema aspetta 300 millisecondi dopo che hai smesso di scrivere (così non fa troppe ricerche mentre stai ancora digitando)
2. Divide la tua query in parole e le "pulisce" (rimuove articoli come "il", "la", ecc.)
3. Cerca queste parole in tutti i campi di tutte le mappe
4. Calcola un punteggio per ogni risultato
5. Ordina i risultati per punteggio e te li mostra

### La gestione degli errori

Il sito è progettato per funzionare anche quando qualcosa va storto:

- **Connessione lenta**: Mostra indicatori di caricamento
- **Immagini mancanti**: Genera automaticamente un'immagine placeholder
- **Dati corrotti**: Salta gli elementi problematici e continua
- **Cache danneggiata**: Si ripulisce automaticamente e ricarica i dati

### Privacy e Cookie

Il sito rispetta rigorosamente la privacy:

- **Cookie necessari**: Solo quelli indispensabili per il funzionamento (preferenze tema, cache)
- **Cookie analitici**: Solo se dai il consenso, per capire come migliorare il sito  
- **Controllo granulare**: Puoi scegliere esattamente quali cookie accettare
- **Modifiche**: Puoi cambiare idea in qualsiasi momento dal link nel footer

## Perché é importante PalermoHub

### Trasparenza dei Dati Pubblici

PalermoHub rende visibili e accessibili dati che spesso sono sepolti in documenti tecnici o siti istituzionali difficili da navigare. È un po' come tradurre il "burocratese" in linguaggio normale e presentarlo in modo visivamente comprensibile.

### Citizen Science

Molte delle mappe sono create da cittadini volontari che prendono i dati grezzi e li trasformano in qualcosa di utile per la comunità. È un esempio di come la tecnologia possa democratizzare l'accesso alle informazioni.

### Riutilizzo Creativo

Ogni mappa presente su PalermoHub può ispirare altri progetti. Un giornalista potrebbe usare una mappa del traffico per un articolo, uno studente per una tesi, un'associazione per una campagna di sensibilizzazione.

## L'Esperienza utente in sintesi

PalermoHub è progettato attorno a un principio semplice: rendere facile trovare quello che cerchi, anche se non sai esattamente cosa stai cercando. 

È come avere un bibliotecario digitale molto paziente che:
- Capisce quello che dici anche se non lo dici perfettamente
- Ricorda le tue preferenze
- Ti suggerisce cose correlate che potrebbero interessarti
- Si adatta al dispositivo che stai usando
- Rispetta la tua privacy

Il risultato è una piattaforma che invita all'esplorazione e rende i dati pubblici veramente pubblici - cioè accessibili a tutti, non solo agli addetti ai lavori.
<br><br>
Spero di essere stato chiaro e di aver coperto tutti gli aspetti essenziali... Buona esplorazione &#128512;
<br><br>
*Grazie OpenDataSicilia* ❤️

### Parlano di noi... [Open Data, AI e trasparenza: PalermoHub e l’innovazione che nasce dal basso](https://innovationisland.it/open-data-ai-trasparenza-palermohub-innovazione/) – [innovationisland.it](https://innovationisland.it/open-data-ai-trasparenza-palermohub-innovazione/)

<hr>
**Disclaimer:** Le informazioni visibili e condivise non comportano la visualizzazione di dati sensibili. Data la natura esclusivamente informativa degli elaborati grafici e dei testi riportati, questi non costituiscono atti ufficiali. Per accedere agli atti ufficiali si rinvia agli elaborati definitivi allegati alle specifiche deliberazioni.