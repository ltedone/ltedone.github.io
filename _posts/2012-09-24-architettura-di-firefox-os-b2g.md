---
id: 12
title: Architettura di Firefox OS (B2G)
date: 2012-09-24T08:25:21+00:00
author: Luigi Tedone
layout: post
guid: http://firefoxositalia.altervista.org/blog/?p=12
permalink: /architettura-di-firefox-os-b2g/
avopt_banners_inside_post:
  - 'true'
av_words_number:
  - 'a:3:{s:10:"word_count";i:355;s:7:"min_pos";i:1413;s:8:"offset_n";i:1;}'
categories:
  - Firefox OS
---
L&#8217;architettura di Firefox OS è formata da 3 livelli chiamati Gonk, Gecko e Gaia; vediamoli adesso in dettaglio:

Gaia: Costituisce l&#8217;interfaccia utente di Firefox OS (B2G). Qualsiasi cosa sia mostrata sullo schermo dopo l&#8217;avvio del sistema operativo fa parte di Gaia. Gaia implementa la lock screen, la schermata principale, l&#8217;applicazione per telefonare, quella per inviare gli SMS, la fotocamera, ecc. Gaia è realizzata interamente in HTML, CSS e JavaScript. La sua sola interfaccia con il sistema operativo sottostante è l&#8217;insieme delle Open Web APIs, che sono implementate all&#8217;interno di Gecko. Gaia funziona perfettamente quando viene eseguito su B2G, ma è possibile utilizzarlo anche su altri sistemi operativi e su altri browser (sebbene con funzionalità ridotte) grazie all&#8217;utilizzo di web APIs standard. E&#8217; possibile installare applicazioni di terze parti (ossia sviluppate dagli utenti) su Gaia.

Gecko: Costituisce l&#8217;ambiente di esecuzione di B2G. Gecko implementa ad alto livello gli standard operti per l&#8217;HTML, CSS e JS e permette a queste interfacce di funzionare correttamente su tutti gli OS supportati da Gecko. Questo significa che Gecko è costituito, insieme ad altre componenti, di un livello che gestisce la rete, uno che gestisce la grafica, un motore che realizza il layout del contenuto, una macchina virtuale per l&#8217;esecuzione di codice JavaScript e livelli per la portabilità.

Gonk: E&#8217; il livello più basso che comunica con l&#8217;hardware e costituisce il sistema operativo di B2G. Gonk è formato da un kernel Linux e un livello di astrazione hardware (HAL). Il kernel e molte librerie sono progetti open source molto conosciuti: linux, libusb, bluez, ecc. Altre parti dell&#8217;HAL sono in comune con il progetto Android, come il GPS, Fotocamera e altri. Si può affermare che Gonk è una distribuzione Linux molto semplice. Gonk costituisce la &#8220;piattaforma&#8221; di Gecko, così come ci sono dei porting di Gecko per OS X, Android, Windows e altri. Dato che il progetto B2G ha il controllo completo su Gonk, è possibile accedere ad interfacce che non sono normalmente esposte da altri OS. Per esempio Gecko ha un accesso diretto all&#8217;intero stack telefonico su Gonk, ma non su altri sistemi operativi.

Se avete bisogno di ulteriori chiarimenti fatemelo sapere attraverso i commenti 😉