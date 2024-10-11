<img src="img/map-icon-pure.svg" width=64px>


# Usare stili di mappa personalizzati

<p align="justify">
Lo "stile di rendering" è l'insieme di tutte le regole che OsmAnd applica per disegnare gli elementi della mappa sul display: è grazie a queste regole se, esplorando la mappa, possiamo distinguere le autostrade (linee arancioni, tratto continuo e spesso) dalle strade sterrate (linea tratteggiata marrone, piuttosto sottile) e dai sentieri percorribili solo a piedi (puntini rossi, tratto sottile).
</p>

<p align="justify">
Al momento dell'installazione l'app adotta lo stile *"Default"*, che va bene più o meno per tutto: però, volendo, se ne possono impostare diversi, per evidenziare particolari caratteristiche: ad esempio, nello stile *"Offroad"* risaltano molto le strade sterrate, in quello *"Mappa nautica"* si vedono meglio alcuni elementi utili alla navigazione in barca, oppure in quello *"Topo"* sono molto evidenti gli edifici(la mappa somiglia molto alle cartine di tipo militare).
</p>

<p align=justify>

**Scegliere uno stile di mappa** tra quelli predefiniti è facilissimo:

 - Apri il menu ***/// -> Configura la mappa -> Stile della mappa***
 - Seleziona lo stile che preferisci tra quelli disponibili
 - Torna alla schermata principale per vedere applicata la nuova rappresentazione.
</p>

<p align=justify>
Nel tempo, però, la Comunità degli utenti ha prodotto altri stili personalizzati, utili ad esempio per progettare viaggi in treno o in bicicletta, o semplicemente per visualizzare la mappa in colorazioni più vivide: la <a href="https://osmand.net/docs/user/troubleshooting/resources#custom-map-styles" target="_blank">Documentazione Ufficiale</a> riporta un elenco abbastanza completo di siti web dov'è possibile reperire i rispettivi file di definizione.
</p>


## Come installare uno stile di mappa personalizzato:
<p align=justify>
Lo stile della mappa è descritto da un file testuale (in formato *xml*), detto *"di rendering"*: lì viene definito l'aspetto di ogni elemento della mappa in termini di colore, tipo di tratto, spessore della linea, ecc.
</p>

<p align=justify>
OsmAnd conserva i file di configurazione della mappa nella cartella */rendering*, che si trova nella directory utilizzata per la memorizzazione dei dati: se vuoi aggiungere un nuovo stile, basta salvare il corrispondente file *.render.xml* in quella posizione.
</p>


Vediamo quindi come fare: ad aggiungere un nuovo stile di mappa: 
<br><br>

### Metodo "semplice" (semi-automatico, Android e iOS)
<p align=justify>
 - Scarica sul tuo dispositivo un file *.render.xml*; ad esempio, nella sezione *Risorse* di questo sito puoi trovarne uno che si chiama *Highlighted AB & Night View.render.xml* e localizza la posizione in cui lo hai salvato (ad esempio la directory */Downloads*). 

 - Raggiungi la directory in cui si trova il file utilizzando un qualsiasi File Manager (ad esempio, in Android: *Files*, oppure *Archivio*) e raggiungi quella cartella; Se invece hai inviato il file come allegato (ad esempio via e-mail) apri l'app corrispondente;
 
 - "Apri" il file *.render.xml* per "aprirlo", toccando il suo nome e Seleziona OsmAnd o OsmAnd+ come app per gestirlo;
 
 - Attendi qualche secondo: OsmAnd si avvia ed importa automaticamente il nuovo stile di mappa.

 - In OsmAnd, vai al menu ***/// -> Configura la mappa -> Stile della mappa***; il nuovo stile dovrebbe essere elencato tra quelli disponibili; non resta che selezionarlo e tornare alla schermata principale per vederlo applicato (non farebbe male riavviare OsmAnd, però).
</p>


### Metodo un po' più complicato (copia manuale, solo Android)
<p align=justify>

 - Invia il file *.render.xml* al tuo dispositivo (ad esempio via Cavetto USB, Bluetooth, FTP, Cloud storage, ecc.) e salvalo in una directory che sia facilmente raggiungibile (esempio: */Download*)
 
 - Avvia OsmAnd ed apri il menu ***/// -> Impostazioni -> Impostazioni OsmAnd -> Cartella salvataggio dei dati***; prendi nota del percorso che corrisponde alla memoria selezionata (ad esempio per la memoria "Esterna 1" potrebbe essere */storage/emulated/0/Android/data/net.osmand.plus/files*), facendo bene attenzione alle lettere maiuscole e minuscole. 

 - Con un File Manager avanzato, come *Total Commander*, *Ghost Commander* o *Files (AOSP)*, raggiungi la directory di salvataggio dati ed entra nella subdirectory */rendering* e salva in essa una copia del file *.render.xml*.

 - Chiudi OsmAnd, e ripulisci la lista delle "App Recenti" di Android (tasto *[=] -> Chiudi tutto*)

 - Avvia di nuovo OsmAnd e vai al menu ***/// -> Configura la mappa -> Stile della mappa***; Il nuovo stile dovrebbe essere elencato tra quelli disponibili; selezionalo e torna alla schermata principale per vederlo applicato.
 
</p>