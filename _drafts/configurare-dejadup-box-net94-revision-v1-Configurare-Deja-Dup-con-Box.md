---
id: 101
title: Configurare Déjà Dup con Box
date: 2014-04-10T14:37:58+00:00
author: Luigi Tedone
layout: revision
guid: http://blog.luigitedone.it/94-revision-v1/
permalink: /?p=101
---
[<img loading="lazy" class="aligncenter size-full wp-image-98" alt="dejadupplusbox" src="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?resize=647%2C297" width="647" height="297" srcset="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?w=647 647w, https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?resize=300%2C137 300w" sizes="(max-width: 647px) 100vw, 647px" data-recalc-dims="1" />](https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png)

Con la recente notizia della chiusura di [Ubuntu One](https://one.ubuntu.com/) mi sono trovato nella necessità di dover pensare ad una soluzione alternativa per il backup dei miei dati. Ubuntu One era perfetto perché era strettamente integrato con Déjà Dup, il tool presente di default all’interno di Ubuntu che consente di eseguire il backup dei propri dati in maniera criptata, veloce ed automatica. Per fortuna Déjà Dup è un tool abbastanza flessibile che può essere configurato per l’utilizzo con vari servizi di storage; può salvare i backup in una cartella locale, su uno spazio FTP, ecc.

Nel mio caso, trovandomi 50 GB su Box praticamente inutilizzati, ho deciso di utilizzarli per effettuare il backup di tutti i miei dati. Box.net, configurato opportunamente, supporta l’accesso con WebDAV; tale protocollo è implementato in Déjà Dup.

Vediamo come procedere per la configurazione:

  * Andare nella scheda Archiviazione
  * Posizione di backup: WebDAV
  * Server: dav.box.com
  * Spuntare la casella Usa connessione sicura (HTTPS)
  * Porta: 443
  * Cartella: inserire il percorsa della cartella nella quale si vogliono memorizzare i file di backup. Tale cartella deve per forza iniziare con il percorso /dav/; io per comodità ho creato all&#8217;interno di Box una cartella chiamata BackupDuplicity e quindi nel mio caso il percorso della cartella sarà /dav/BackupDuplicity/
  * Nome utente: inserire il nome utente con il quale ci si è registrati a Box (corrisponde all&#8217;indirizzo email)

Il risultato sarà molto simile a quello mostrato nell&#8217;immagine seguente:

[<img loading="lazy" class="aligncenter size-full wp-image-96" alt="dejadup" src="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?resize=750%2C426" width="750" height="426" srcset="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?w=851 851w, https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?resize=300%2C170 300w" sizes="(max-width: 750px) 100vw, 750px" data-recalc-dims="1" />](https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png)

A questo punto sarà tutto configurato e sarà possibile utilizzare lo spazio su Box per i propri backup!