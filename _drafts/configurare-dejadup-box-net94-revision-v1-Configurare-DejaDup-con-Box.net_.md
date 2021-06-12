---
id: 99
title: Configurare DejaDup con Box.net
date: 2014-04-10T14:23:57+00:00
author: Luigi Tedone
layout: revision
guid: http://blog.luigitedone.it/94-revision-v1/
permalink: /?p=99
---
[<img loading="lazy" class="aligncenter size-full wp-image-98" alt="dejadupplusbox" src="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?resize=647%2C297" width="647" height="297" srcset="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?w=647 647w, https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png?resize=300%2C137 300w" sizes="(max-width: 647px) 100vw, 647px" data-recalc-dims="1" />](https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadupplusbox.png)

Con la recente notizia della chiusura di [Ubuntu One](https://one.ubuntu.com/) mi sono trovato nella necessità di dover pensare ad una soluzione alternativa per il backup dei miei dati. Ubuntu One era perfetto perché era strettamente integrato con DejaDup, il tool presente di default all’interno di Ubuntu che consente di eseguire il backup dei propri dati in maniera criptata, veloce ed automatica. Per fortuna DejaDup è un tool abbastanza flessibile che può essere configurato per l’utilizzo con vari servizi di storage; può salvare i backup in una cartella locale, su uno spazio FTP, ecc.

Nel mio caso, trovandomi 50 GB su Box.net praticamente inutilizzati, ho deciso di utilizzarli per effettuare il backup di tutti i miei dati. Box.net, configurato opportunamente, supporta l’accesso con WebDAV; tale protocollo è implementato in DejaDup.

Vediamo come procedere per la configurazione:

[<img loading="lazy" class="aligncenter size-full wp-image-96" alt="dejadup" src="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?resize=750%2C426" width="750" height="426" srcset="https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?w=851 851w, https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png?resize=300%2C170 300w" sizes="(max-width: 750px) 100vw, 750px" data-recalc-dims="1" />](https://i1.wp.com/blog.luigitedone.it/wp-content/uploads/2014/04/dejadup.png)