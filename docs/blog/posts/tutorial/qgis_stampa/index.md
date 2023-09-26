---
title: QGIS e la stampa in PDF layered (a strati)
description:  QGIS e la stampa in PDF layered (a strati)
draft: false
date: 2017-01-27
authors:
  - gbvitrano
categories:
  - Tutorial
tags:
  - QGIS
  - pdf
  - Stampa pdf
  - svg
  - Layer
social_image: assets/img/social/corel.jpg
--- 
<style>.md-typeset code { background-color: #fff0;}  </style>
[![QGIS e la stampa in PDF layered (a strati)](pdflayered.webp "QGIS e la stampa in PDF layered (a strati)" ){class="crop gray" align=left}](index.md) 

Come ottenere un file PDF multi livello dal compositore di stampe di QGIS?

Fino ad oggi anche la versione 3.4.4 [QGIS](https://www.qgis.org/it/site/forusers/download.html) non crea livelli nei file pdf che vengono esportati, questo dipende, tra le altre cose, da tutte le proprietà del livello che rendono così grande [QGIS](https://www.qgis.org/it/site/forusers/download.html) per creare mappe e simboli eleganti.Non è semplice trasferire stili e colori trasparenti, nel formato pdf.

Ad oggi un metodo valido (probabilmente l’unico) è quello che [Totò Fiandaca](https://twitter.com/totofiandaca)  spiega nel suo blog [pigrecoinfinito](https://pigrecoinfinito.wordpress.com/2016/10/01/qgis-e-la-stampa-in-pdf-layered-a-strati/), <!-- more -->ideato nel 2015 da_magerlin_ e successivamente discusso [qui](http://gis.stackexchange.com/questions/7078/can-qgis-preserve-layers-when-exporting-to-pdf)gis.stackexchange.com. Vi consiglio di leggerlo per capire in dettaglio la procedura, io mi limiterò semplicemente a riprodurlo ed inserire una semplice variante.

Il metodo è menzionato anche sul blog Svedese [geosupportsystem.se](https://geosupportsystem.se/2018/12/19/pdf-karta-med-lager/?fbclid=IwAR3_VmJ8qPbfdZqlDnfAwVazMVC4wm3YtwFamPEpsubHh-6GKsEHGJ5VzjM) a conferma della bontà della procedura, qualora ce ne fosse bisogno.

La variante è dovuta al fatto che io sono un po distratto…e spesso qualche procedura, selezione o oggetto mi sfugge, soprattutto con layout complessi e ricchi di oggetti. In questi casi  devo fare il lavoro più volte 🙂 per non dimenticare, come dice il buon [Andrea Borruso](https://twitter.com/aborruso) cit. “_Questo post vale come nota personale, da rileggere quando mi servirà nuovamente_“

**Dando per scontato che avete letto il [post](https://pigrecoinfinito.wordpress.com/2016/10/01/qgis-e-la-stampa-in-pdf-layered-a-strati/) di Totò procediamo…**

![QGIS e la stampa in PDF layered (a strati)](screenshot.147_01.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Dopo aver impostato il vostro layout di stampa (dimensione pagina) e utilizzato i vari layer sovrapposti, mappa, legenda, testi, loghi, ecc… esportate il tutto in [SVG

![QGIS e la stampa in PDF layered (a strati)](screenshot.148_03.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Come ci ricorda Totò…è fondamentale selezionare ‘**Esporta layer come gruppi [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)** ‘! nell’esportare il layout di QGIS in [SVG

Dopo questa fase Totò utilizza subito [Scribus](https://www.scribus.net/) un software Open Source che permette di salvare i file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)  in [PDF](https://acrobat.adobe.com/it/it/acrobat/about-adobe-pdf.html) con i diversi livelli definiti.

Io invece faccio un ulteriore passaggio con [InkScape](https://inkscape.org/it/), a causa della mia distrazione, per evitare di complicarmi la vita con le varie selezioni di gruppi e oggetti.

![QGIS e la stampa in PDF layered (a strati)](screenshot.150.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Aprite il file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)  con [InkScape](https://inkscape.org/it/) e salvate una “**copia con nome**…” selezionare l’opzione “**Livelli come SVG separati (. tar)**“, otterrente un file compresso al cui interno ci saranno tanti file SVG quanti sono i livelli del file originale. Il file **.tar** si può decomprimere facilmente con tutte le utility  di compressione ed archiviazione come [WinRAR](https://www.winrar.it/), [7zip](https://www.7-zip.org/) o similari. All’interno del file compresso i file sono nominati con il nome del layer, quindi troveremo, Layer 1.svg, Layer 2.svg, Layer 3.svg, ecc…

**I**l file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) esportato da [QGIS](https://www.qgis.org/it/site/forusers/download.html) può essere aperto con [InkScape](https://inkscape.org/it/) che legge i vari livelli in automatico, però NON supporta la stampa in PDF layered!!! 🙁 al contrario [Scribus](https://www.scribus.net/) supporta la stampa in PDF layered ma NON legge i vari livelli degli SVG!!! (Cit. Totò Fiandaca) Sarebbe tutto troppo facile 🙂

A questo punto dobbiamo decomprimere il file **.tar** e iniziare a lavorare con [Scribus](https://www.scribus.net/). Niente panico [Scribus](https://www.scribus.net/) è semplice ed intuitivo, soprattutto se si ha familiarità con programmi di grafica vettoriale come InkScape, CorelDraW,  Adobe illustrator e Adobe InDesigne ecc…

![QGIS e la stampa in PDF layered (a strati)](screenshot.151.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Installiamo [Scribus](https://www.scribus.net/)**, apriamo un nuovo documento** stando attenti alla dimensione della pagina. Nel mio caso avevo impostato in [QGIS](https://www.qgis.org/it/site/forusers/download.html) un layout di stampa in formato A4 orizzontale, di conseguenza anche in [Scribus](https://www.scribus.net/) devo ricreare le stesse condizioni.

![QGIS e la stampa in PDF layered (a strati)](screenshot.152.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Il prossimo passo è aggiungere tanti nuovi livelli quanti sono i file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) esportati da [InkScape](https://inkscape.org/it/), nel mio caso ho aggiunto 18 nuovi layer.

![QGIS e la stampa in PDF layered (a strati)](screenshot.153.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Adesso diventa tutto semplice, per caricare i vari file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) nei rispettivi layer basta usare il classico **drag-and-drop**, dal pannello **Livelli,** selezioniamo il livello corrispondente al nome del file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) e trasciniamo li il nostro file. Tutti i file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) hanno la dimensione A4 orizzontale (210×297), se non li avete separati e se è necessario, si possono centrare tutti sulla pagina, usando il pannello **Allinea e distribuisci**.

![QGIS e la stampa in PDF layered (a strati)](screenshot.160.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

In alternativa al trascinamento possiamo usare la funzione **Importa** –> **Carica file vettoriale** dal menù **File,** sempre selezionando prima il layer corrispondente.

![QGIS e la stampa in PDF layered (a strati)](screenshot.154a.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Caricati e ordinati tutti i layer, dobbiamo rinominare i layer con i nomi reali dei vari oggetti, dopo averlo fatto siamo pronti per stampare il nostro PDF con livelli.

![QGIS e la stampa in PDF layered (a strati)](screenshot.155a.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Spostiamoci su **File –> Esporta –> Salva come PDF**

![QGIS e la stampa in PDF layered (a strati)](screenshot.157.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }Nelle impostazioni delle opzioni di stampa fate attenzione alla “**Compatibilità”,** selezionate almeno **PDF 1.5** (la versione PDF 1.4 o precendenti non supportano l’opzione livelli) e spuntate **“Include livelli”**, in caso contrario non otterrete il PDF multi livello.

![QGIS e la stampa in PDF layered (a strati)](screenshot.175.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Fatto…ecco il PDF multi layer, fidatevi è molto più semplice di quello che può sembrare 🙂

A questo punto vi state chiedendo perché ho fatto un ulteriore passaggio con [InkScape](https://inkscape.org/it/) e salvato il file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) in  “**Livelli come SVG separati (. tar)**“?

La risposta è semplice, [Scribus](https://www.scribus.net/) quando importa il file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) non mostra l’elenco dei vari gruppi di oggetti nel pannello dei livelli (cosa che per esempio [CorelDraw](https://www.coreldraw.com/it/) fa), quindi quando si sbloccano e si separano i gruppi , diventa molto complicato selezionare gli oggetti da spostare e riordinare. Se invece gruppi e oggetti sono suddivisi in singoli file, diventa molto semplice e immediato riordinare.

“In buona sostanza…”un singolo file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) contiene solo un gruppo di oggetti, basta semplicemente caricarlo nel layer corrispondente.

Si può ottenere un PDF a livelli anche con [CorelDraw](https://www.coreldraw.com/it/), che legge i file [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics) e i relativi livelli nativamente e supporta la stampa PDF layered

![QGIS e la stampa in PDF layered (a strati)](coreldraw.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Vediamo come… Apriamo un **nuovo documento**, settiamo le dimensioni della pagina (in questo caso è sempre un A4 orizzontale) e con il **drag–and–drop** importiamo il file _[SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)_ ottenuto dal compositore di stampe di_[QGIS](https://www.qgis.org/it/site/forusers/download.html)_, dopo qualche secondo di attesa i layers del file _[SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)_ vengono caricati come gruppi di oggetti bloccati, come si vede dall’immagine. Come prima cosa occorre sbloccare i vari gruppi, aggiungere i nuovi livelli, separare i gruppi e spostare i gruppi nei relativi livelli, infine  rinominare i livelli secondo le proprie esigenze.

Riepilogo della procedura con [CorelDraw](https://www.coreldraw.com/it/)

1. Nuovo Documento;
2. Impostare la dimensione della pagina corretta;
3. Importare file _[SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)_;
4. Sbloccare i vari gruppi;
5. Aggiungere i nuovi livelli;
6. Separare i gruppi;
7. Spostare i gruppi nei relativi livelli;
8. Rinominare i livelli;
9. Pubblica PDF.

![QGIS e la stampa in PDF layered (a strati)](corel_02.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

ed infine stampare… **File –> Pubblica PDF** anche in questo caso ricordate di settare nelle preferenze di stampa almeno **PDF 1.5**

![QGIS e la stampa in PDF layered (a strati)](corel_03.webp "QGIS e la stampa in PDF layered (a strati)"){ .off-glb }

Fatto… per motivi di tempo non ho rinominato i layer in [CorelDraw](https://www.coreldraw.com/it/).

Tengo a precisare che [QGIS](https://www.qgis.org/it/site/forusers/download.html), [Scribus](https://www.scribus.net/) e [InkScape](https://inkscape.org/it/) sono software Open Source, e quindi a costo zero, diversamente [CorelDraw](https://www.coreldraw.com/it/) è un software proprietario e quindi a pagamento, ma se siete in possesso di una licenza [CorelDraw](https://www.coreldraw.com/it/) o una copia demo di 30 giorni (come nel mio caso per fare il test) potete usarla per ottenere il PDF layered. Lo stesso metodo può essere applicato con qualsiasi altro software di grafica vettoriale che supporti SVG e stampi in PDF layered. Ricordate che per far tutto questo è fondamentale selezionare ‘**Esporta layer come gruppi [SVG](https://it.wikipedia.org/wiki/Scalable_Vector_Graphics)** ‘ dal compositore di stampa di [QGIS](https://www.qgis.org/it/site/forusers/download.html).

Grazie [Totò Fiandaca](https://twitter.com/totofiandaca) per avermi fatto conoscere la procedura.

I **[PDF](https://acrobat.adobe.com/it/it/acrobat/about-adobe-pdf.html)** layered NON sono supportati da [QGIS](https://www.qgis.org/it/site/forusers/download.html) solo per una questione di tempo e di interesse; se ci fossero molte richieste e qualche contributo, gli sviluppatori di [QGIS](https://www.qgis.org/it/site/forusers/download.html) lo implementerebbero facilmente. [OpenJump](http://openjump.org/) lo supporta. (Cit. Totò Fiandaca)