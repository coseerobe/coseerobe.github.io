---
title: Osservare il cambiamento di una città grazie alla cartografia
description: Atlante - Carta Tecnica - Palermo
draft: false
date: 2017-04-05
authors:
  - gbvitrano
categories:
  - Mappe
slug: atlante-storico-palermo   
tags:
  - Cartografia
  - Palermo
  - Atlante
  - Carta Tecnica
social_image: assets/img/social/atlante_storico.jpg
---
<style>
.md-typeset code { background-color: #fff0;}  
.md-typeset pre>code { background-color: #fff0;}  
</style>
[![Atlante](atlante_storico.jpg "Atlante - Carta Tecnica - Palermo" ){class="crop gray off" align=left}](index.md)

## Il caso di Palermo
Dopo aver letto l’articolo di [@napo](https://twitter.com/napo) [mappa di Trento 1915 – da un libro di Cesare Battisti](https://medium.com/@napo/mappa-di-trento-1915-da-un-libro-di-cesare-battisti-84935794b1ed), ne sono rimasto affascinato, sia per il gran lavoro fatto dalla biblioteca comunale di Trento, nel digitalizzare il contenuto del libro e renderlo di dominio pubblico e sia per la parte tecnica e dall’analisi, che si può fare agevolmente, mettendo a confronto una carta storica ed una di oggi.<!-- more -->

Brevemente, con il plugin [leaflet-tileoverlay-mask](https://github.com/frogcat/leaflet-tileoverlay-mask),  si ottiene un effetto “[spot](https://github.com/frogcat/leaflet-tileoverlay-mask)”  sulle cartografie, che ci permette di mettere a confronto, dinamicamente e istantaneamente, una carta storica con lo stato attuale.

La realizzazione tecnica, è più semplice di quello che si pensa

Subito ho pensato come poter usare questa tecnica sulle cartografie storiche e non di Palermo.

Il primo test  l’ho fatto, con la cartografia del  nuovo schema di [massima del PRG](https://www.comune.palermo.it/js/server/uploads/_06102015125400.pdf) di Palermo presentato dal [Comune nel 2015](https://www.comune.palermo.it/noticext.php?id=8088) e [georeferenziata](http://mapwarper.net/maps/19437) da [@cirospat](https://twitter.com/cirospat), con [mapwarper.net](http://mapwarper.net/) constatando, in prima persona, la bontà del lavoro fatto da [@napo](https://twitter.com/napo).

![cambiamenti](cambiamenti.jpg "Cambia-menti"){.off-glb }

In questo caso ho semplicemente sostituito la base cartografica **“L.tileLayer.mask**” di riferimento, nel file di esempio fornito con  plugin [leaflet-tileoverlay-mask](https://github.com/frogcat/leaflet-tileoverlay-mask)”.

Inserendo la nuova mappa tiles e centrando la mappa sulle coordinate di Palermo, il lavoro è fatto.

**Nuova base tiles**

var prg =  L.tileLayer.mask(‘[http://mapwarper.net/maps/tile/19437/{z}/{x}/{y}.png](http://mapwarper.net/maps/tile/19437/%7Bz%7D/%7Bx%7D/%7By%7D.png)‘

**Zoom e coordinate di base**

var map = L.map(‘map’, {attributionControl:true}).setView([38.11127,13.3534422], 14);

Usando la versione originale del plugin [leaflet-tileoverlay-mask](https://github.com/frogcat/leaflet-tileoverlay-mask), ho notato un limite, ovvero, l’impossibilità di utilizzare più basi cartografiche, per fare l’analisi.

Con il contributo fondamentale di [@piersoft](https://twitter.com/Piersoft), sono riuscito a superare l’ostacolo.

Dopo questo piccolo test, mi sono chiesto, come poter sfruttare al meglio la tecnica.

Confrontandomi con _[@aborruso](https://twitter.com/aborruso)_ e _[@cirospat](https://twitter.com/cirospat)_, del gruppo di _[opendatasicilia](http://opendatasicilia.it/)_, sull’uso della _[tileoverlay-mask](https://github.com/frogcat/leaflet-tileoverlay-mask)_ e conoscendo il _[Portale Cartografico](http://geosrv.comune.palermo.it/carto/)_, realizzato dalla _[Sispi](http://www.sispi.it/)_ spa (società in house del comune di Palermo), subito abbiamo pensato di utilizzarla, con le cartografie storiche. Rese disponibili dall’ottimo lavoro di scansione e georeferenziazione del geom. Liborio Plazza, dipendente del Comune di Palermo e  dalla _[Sispi](http://www.sispi.it/)_.

L’obiettivo era chiaro, costruire un atlante, dove poter mettere a confronto, velocemente, le carte storiche con la città dei nostri giorni.

Scaricate e georeferenziate le cartografie storiche, da [@borruso](https://twitter.com/aborruso) e [@cirospat](https://twitter.com/cirospat), a me, non è rimasto altro da fare, che organizzare  il materiale e dargli una veste grafica user friendly. Spero di esserci riuscito!

[Qui larticolo su #opendatasicilia – Osservare il cambiamento di una città grazie alla cartografia: il caso di Palermo](http://opendatasicilia.it/2017/04/06/osservare-il-cambiamento-di-una-citta-grazie-alla-cartografia-il-caso-di-palermo/)

[Qui](https://medium.com/tantotanto/dati-da-un-server-wms-scaricarli-riproiettarli-comprimerli-e-tassellarli-da-riga-di-comando-a34cb6fe13e0) una guida di [@aborruso](https://twitter.com/aborruso)  su come scaricare i dati da un server WMS – [Come faremmo senza GDAL?](https://medium.com/tantotanto/dati-da-un-server-wms-scaricarli-riproiettarli-comprimerli-e-tassellarli-da-riga-di-comando-a34cb6fe13e0)

<hr>

<iframe width="100%" height="600px" frameborder="0" allowfullscreen allow="geolocation" src="https://palermohub.opendatasicilia.it/index_atlante_noheader.html#14/38.1113/13.3534"></iframe>
<p><a href="https://palermohub.opendatasicilia.it/index_atlante.html#14/38.1113/13.3534">Visualizza a schermo intero</a></p>

![atlante_news](atlante_news.jpg "atlante_news"){.off-glb style="display: block; margin: 0 auto" }

<hr>

### Gli strumenti che abbiamo utilizzato per il il progetto dell’atlante sono:

1. [Dati da un server WMS:](https://medium.com/tantotanto/dati-da-un-server-wms-scaricarli-riproiettarli-comprimerli-e-tassellarli-da-riga-di-comando-a34cb6fe13e0) scaricarli, riproiettarli, comprimerli, tassellarli e piramidarli da riga di comando, di [@aborruso](https://twitter.com/aborruso);
2. [Leaflet,](http://leafletjs.com/) per creare l’interfaccia di web mapping;
3. [Leaflet-hash](https://github.com/mlevans/leaflet-hash), per generare URL che contengono livello di zoom e posizione corrente;
4. [Leaflet-tileoverlay-mask](https://github.com/frogcat/leaflet-tileoverlay-mask), per la sovrapposizione delle tile con effetto svg maschera, un effetto “spot“ che ci permette di vedere come era la città al tempo in un particolare punto;
5. [Sidebar-v2](https://github.com/turbo87/sidebar-v2/), per creare sidebar a scomparsa;
6. [Leaflet.MousePosition](https://github.com/ardhi/Leaflet.MousePosition), è un semplice controllo della posizione del mouse. Esso mostra le coordinate geografiche del puntatore del mouse, mentre viene spostato sulla mappa;
7. [Leaflet-graphicscale](https://github.com/nerik/leaflet-graphicscale), è un semplice barra di scala con effetto animato al cambio dello zoom;
8. [Map Warper](http://mapwarper.net/), è uno strumento open source per georeferenziare immagini, nato grazie al [contributo](https://github.com/timwaters/mapwarper) del progetto [spacetime](https://github.com/nypl-spacetime/) della [Biblioteca Comunale di New York](https://github.com/NYPL), sviluppato, ospitato e mantenuto da [Tim Waters](https://twitter.com/tim_waters);
9. [Btns](https://github.com/mrmrs/btns), è un piccolo modulo CSS che permette di inserire pulsanti reattivi.
10. [Leaflet.Basemaps](https://github.com/consbio/Leaflet.Basemaps), consente di creare un controllo dell’interfaccia utente per la scelta della mappa di base utilizzato sulla mappa.

### Il codice script usato per il progetto è  liberamente scaricabile dalla pagine html dell’atlante. Basta sostituire i relativi L.tileLayer.mask e il setView([38.11127,13.3534422] per adattarla alle proprie esigenze.

### Ne parlano…


* [Giornale di Sicilia](http://palermo.gds.it/2017/04/12/un-dipendente-del-comune-ricostruisce-la-mappa-di-palermo-del-1935-1956-e-1987-guarda-le-immagini_652985/?utm_medium=feed&utm_source=facebook.com&utm_campaign=Feed%3A+gds_facebook_feed);
* [Balarm](https://www.balarm.it/articoli/magazine/territorio/palermo-viaggia-nel-tempo-fino-al-1935-grazie-a-una-mappa-da-hacker-18336);
* [palermoalcontrario;](https://palermoalcontrario.com/2017/04/12/mouse-e-carte-storiche-per-un-viaggio-nel-tempo/)
* [ilcantooscuro](https://ilcantooscuro.wordpress.com/2017/04/12/viaggio-nel-tempo/);
* [ilsicilia.it;](http://www.ilsicilia.it/levoluzione-di-palermo-dal-1935-a-oggi-ricostruita-la-mappa-del-sacco-edilizio-naviga-la-mappa/)
* [Il Piccolo.](http://ilpiccolo.gelocal.it/trieste/cronaca/2017/05/19/news/maggiore-efficienza-grazie-ai-dati-aperti-i-segreti-del-successo-lombardo-1.15359875?ref=hfpitsea-1)

Un ringraziamento particolare va a [@napo](https://twitter.com/napo) che con il lavoro, **[mappa di Trento 1915 – da un libro di Cesare Battisti](https://medium.com/@napo/mappa-di-trento-1915-da-un-libro-di-cesare-battisti-84935794b1ed#.w7hqdcsuv)**, ci ha fatto riscoprire la bellezza e l’importanza delle mappa storiche.

Ringrazio anche il mio Capo Area, dell’Area Tecnica della Riqualificazione Urbana e delle Infrastrutture, Arch. Mario Li Castri e tutti i miei colleghi del Comune di Palermo, che con un post pubblico su [facebook](https://www.facebook.com/mario.l.castri/posts/10210864347916224), hanno appezzato questa nostra piccola iniziativa ed omaggio a Palermo, grazie di cuore a tutti, questo è un motivo in più per continuare a lottare contro il cancro e rientrare al più presto in Ufficio.

<hr>
**Disclaimer:** Le informazioni visibili e condivise non comportano la visualizzazione di dati sensibili. Data la natura esclusivamente informativa degli elaborati grafici e dei testi riportati, questi non costituiscono atti ufficiali. Per accedere agli atti ufficiali si rinvia agli elaborati definitivi allegati alle specifiche deliberazioni.