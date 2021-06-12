---
id: 225
title: Ancora un aggiornamento per i Geeksphone!
date: 2014-04-22T16:25:15+00:00
author: Luigi Tedone
layout: revision
guid: http://blog.luigitedone.it/128-revision-v1/
permalink: /?p=225
---
Poche ore fa è stato rilasciato da Geeksphone un nuovo aggiornamento per i due modelli di smartphone con Firefox OS a bordo, il Keon e il Peak. Questo nuovo aggiornamento allinea la versione corrente del firmware al codice presente nella repository di Mozilla; si tratta pertanto di una versione nightly che potrebbe presentare alcuni bug.

Tra le novità presenti, quella di maggior rilievo è la presenza della lingua italiana (finalmente!) e di una migliore reattività del sistema in generale.

La versione installata dopo l&#8217;aggiornamento sarà la 2.0.0.0-prerelase, basata sulla versione 24.0a1 di Gecko e con Git commit del 30/05/2013.

L&#8217;aggiornamento dovrebbe comparire nella barra delle notifiche; nel caso non sia presente è possibile forzare un controllo manuale recandosi in Settings->Device Information e cliccare sul pulsante Check Now all&#8217;interno della sezione Software updates.

Se anche con il controllo manuale non sono segnalate nuove versioni, è necessario applicare il seguente script per risolvere un bug sugli aggiornamenti FOTA (solo se si ha installata una versione del firmware precedente al 31 maggio 2013):

  1. scaricare il seguente file da Geeksphone <a href="http://downloads.geeksphone.com/drivers/dogfood-setup.sh" target="_blank">http://downloads.geeksphone.com/drivers/dogfood-setup.sh</a>
  2. aprire il terminale, spostarsi all&#8217;interno della cartella dove si è scaricato il file del punto precedente e digitare il seguente comando: 
      1. Per il PEAK ./dogfood-setup.sh <a href="http://gpfosnightly.s3.amazonaws.com/peak_nightly/update.xml" target="_blank">http://gpfosnightly.s3.amazonaws.com/peak_nightly/update.xml</a>
      2. Per il KEON ./dogfood-setup.sh <a href="http://gpfosnightly.s3.amazonaws.com/peak_nightly/update.xml" target="_blank">http://gpfosnightly.s3.amazonaws.com/keon_nightly/update.xml</a>
  3. a questo punto è possibile cercare i nuovi aggiornamenti mediante la procedura manuale sopra esposta, che compariranno nella barra delle notifiche.

Buon aggiornamento! 🙂

&nbsp;