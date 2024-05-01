<img src="img/480px-Crystal_button_cancel.png" style="width:64px;height:64px;">

# ARRESTO DEL PROCESSO DI OSMAND
<p><i><b>Se torno alla schermata Home del mio dispositivo, OsmAnd smette di funzionare?</i></b>


**Dipende** da “come” si esce dall'app e dal suo stato di funzionamento quando ciò
avviene:
* Se si preme il pulsante “Home”, oppure si richiama l'elenco delle app 
recenti col pulsante “Menu/Recenti” l'applicazione viene messa in secondo
piano e continua a funzionare in background: in seguito, il Sistema Operativo
potrebbe metterla in stato di “stand-by”, allo scopo di ridurre il consumo di
energia del dispositivo.
* Se invece si preme il pulsante “Indietro” fino a tornare alla schermata Home, 
OsmAnd si arresta se si trova in stato di riposo; se però sta navigando verso una
destinazione o registrando un tracciato gpx, l'app dovrebbe proseguire nel suo
funzionamento: ciò è indicato anche dalla persistenza di un'icona nella barra di
notifica del dispositivo (ad esempio: “Registrazione traccia in corso”).
</p>

<BR>
<BR>

***Mi hanno suggerito di “arrestare completamente OsmAnd”. Non basta premere il tasto “Indietro” del mio dispositivo?***

**Non sempre.** Se si sta navigando verso la destinazione o registrando il viaggio in un file gpx, uscire dall'app con il tasto Indietro non fa necessariamente cessare l'esecuzione di tutti i processi associati ad OsmAnd.

Il modo corretto per arrestare del tutto OsmAnd (vale per tutte le app di Android, in realtà) sarebbe quello di utilizzare l'apposito pulsante nel menu di sistema ***Impostazioni → Applicazioni → OsmAnd***
***→ Arresto forzato.***

Esiste però un metodo molto più immediato, che consiste nel richiamare l'elenco delle app recenti con l'apposito pulsante del dispositivo, sfogliare la lista fino a trovare quella che si desidera e “terminarla” facendone scorrere la relativa finestra di anteprima verso l'alto (o di lato, a seconda della versione di Android): questo farà interrompere tutti i processi collegati all'app, anche quelli eventualmente “dormienti”.

Si consiglia pertanto di seguire quest'ultima procedura, quando si vuol essere sicuri che
l'app non sia effettivamente più attiva nel sistema.

<BR>
<BR>
<BR>

<img src="img/Gnome-colors-view-refresh.png" style="width:64px;height:64px;">

# REINSTALLAZIONE DI OSMAND
***Avevo un problema con OsmAnd: ho provato a reinstallare l'app ma il comportamento è rimasto il medesimo di prima. Cosa posso fare?***

A volte i comportamenti anomali di OsmAnd non dipendono da errori nel programma, ma da alcuni parametri di configurazione, memorizzati su file nella cartella di salvataggio dati.

Quelle informazioni non vengono sempre eliminate con una semplice disinstallazione tramite i comandi standard dell'interfaccia utente (tocco lungo sull'icona, *Disinstalla*): se per caso un file di configurazione contiene dati corrotti o inconsistenti, OsmAnd li userà di nuovo esattamente come sono, introducendo di nuovo il comportamento indesiderato.

A volte, quindi, bisogna procedere manualmente in modo più mirato.

<br>


## Pulizia della cache
Il Sistema Operativo riserva ad ogni app una *cache*, ovvero uno spazio di memorizzazione in cui salvare informazioni temporanee, come ad esempio stati di funzionamento del programma, identificativi di sessione, ecc.

La cache di OsmAnd viene ripulita alla chiusura ddel programma: può però capitare che ciò non avvenga, ad esempio se si verifica un errore interno e l'app si chiude.

In Android è possibile compiere manualmente quest'operazione: basta aprire il menu di sistema **Impostazioni → Applicazioni → OsmAnd → Memoria archiviazione → Svuota cache.**

Si raccomanda di arrestare completamente OsmAnd (vedi paragrafo precedente) prima di compiere quest'operazione e quindi riavviare l'app una volta ripulita la cache.

<BR>
<BR>

## Reinstallazione “da zero” (“Fresh install”)
Quando si vuole ottenere una pulizia più approfondita dei dati di OsmAnd, ad esempio perchè si comporta in maniera inconsistente, invece di limitarsi a disinstallarlo con la procedura standard si può procedere come segue:

### Backup
* Avviare OsmAnd (se possibile) ed aprire il menu <i><b>/// → Impostazioni → Impostazioni OsmAnd → Cartella salvataggio dei dati</i></b>; Prendere nota del percorso selezionato, ad esempio: <b><i>/storage/emulated/0/Android/data/net.osmand.plus/files</b></i>

* Arrestare OsmAnd premendo alcune volte il tasto “Indietro” del dispositivo;

* Con un File Manager (quello di sistema, oppure un' app Free come Total Commander o Ghost Commander), raggiungere la directory di salvataggio dati; Se si dispone dell'abbonamento al servizio Pro, tutto il materiale qui elencato si può caricare su un server nel Cloud (servizio OsmAnd Cloud).

* (Facoltativo) Fare una copia di backup di tutto il materiale che si desidera conservare, ad esempio le mappe (file .obf), preferiti (cartella favorites), e tracce registrate/pianificate (cartella tracks).  
Si raccomanda di evitare qualsiasi altro tipo di file: se si esegue un backup di un file di configurazione corrotto e poi lo si ripristina, l'intera procedura sarà vanificata.

* La procedura di backup potrebbe durare da pochi secondi a molti minuti: Assicurarsi di mantenere il dispositivo collegato all'alimentazione esterna per evitare che il dispositivo possa interrompere le operazioni per l'intervento del rispsrmio energetico.

* Al termine delle operazioni di backup, chiudere il File Manager.

### Disinstallazione completa
* Disinstallare OsmAnd con la procedura standard (tocco lungo sull'icona, Disinstalla): se il Sistema Operativo chiede se si desidera mantenere i dati dell'app, rispondere NO

* Da File Manager, tornare alla cartella di memorizzazione dati: se esiste ancora, eliminare tutto il suo contenuto.
* Reinstallare OsmAnd normalmente;


### Ripristino dei dati
* (Facoltativo) Ripristinare il materiale salvato (mappe, tracce, ecc.) nella stessa posizione in cui si trovava prima, cosicché OsmAnd, all'avvio, possa già trovare tutti i dati ed indicizzarli correttamente.
Se si è abbonati al servizio Pro, si potranno ripristinare mappe, tracciati ecc. semplicemente scaricandoli dal server attravarso la funzione di sincronizzazione del proprio account OsmAnd Cloud.

* Avviare OsmAnd e procedere all'inizializzazione del programma.

<br>
<br>

<img src="img/attenzione.png" style="width:48px;height:48px;" align="left" hspace=10 vspace=20>

## ATTENZIONE
<br>
Se i dati di OsmAnd si trovavano su una scheda di espansione (SD/MicroSD) esterna e quest'ultima viene sostituita, prima di procedere al ripristino sarà necessario tornare al menu <i><b>/// → Impostazioni → Impostazioni OsmAnd → Cartella salvataggio dei dati</b></i> e ribadire l'impostazione:

* Assicurarsi che sia selezionata la memorizzazione su memoria interna; Se non lo è, selezionarla e riavviare OsmAnd

* Selezionare la memoria esterna desiderata (di solito la MicroSD esterna corrisponde alla "*Memoria esterna 2*")

* Ripristinare i dati dalla copia di backup, ricopiandoli a destinazione.

* Riavviare OsmAnd.
