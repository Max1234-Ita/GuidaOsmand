<img src="img/OsmAnd V	eloce.png" style="width:64px;height:64px;">

# VELOCIZZARE L'ESECUZIONE DI OSMAND
<p><i><b>Ultimamente OsmAnd è molto lento: la mappa si muove a scatti, la registrazione dei tracciati s'interrompe, la posizione non viene aggiornata e l'app sembra non reagire ai comandi, o lo fa con molto ritardo. Perchè?</i></b>


Diversi fattori possono causare questi fenomeni:

* **Sovraccarico del Sistema**
Quando le risorse di memoria del dispositivo scarseggiano, il sistema cerca di liberarne una parte: ciò può tradursi in un maggiore carico di lavoro per il processore (CPU) e ripercuotersi sulle prestazioni delle applicazioni, che funzionano più lentamente.  
  
  Discorso analogo vale nel caso in cui il processore grafico (GPU) si trovi a dover gestire un numero di elementi troppo elevato rispetto alle sue capacità di elaborazione: in questo caso il display sarà aggiornato con ritardo (tecnicamente chiamato “lag”), da cui la “scattosità” del programma.

* **Surriscaldamento**  
Entrambe le situazioni sopra descritte portano il dispositivo a funzionare al massimo della potenza, aumentando così il consumo di energia e la temperatura di esercizio; quando quest'ultima è troppo elevata e non vi è un efficace raffreddamento, interviene il meccanismo di protezione noto come ***“Thermal throttling”**:* la velocità di funzionamento dei processori si riduce, il che peggiora ulteriormente le prestazioni generali del sistema.  
  
  È quindi bene evitare di far funzionare il dispositivo in un luogo chiuso, poco ventilato e, soprattutto, esposto all'irraggiamento solare diretto, che può far salire rapidamente la temperatura dei componenti elettronici e, soprattutto, della batteria: anche pochi minuti in queste condizioni possono danneggiarlo seriamente.  
    
    Un **accorgimento utilizzabile in auto** è quello di posizionare il dispositivo davanti ad una delle aperture per la ventilazione dell'abitacolo, fissandolo con un apposito supporto reperibile comunemente nei negozi di accessori per la
telefonia mobile; se si viaggia **in moto o in bicicletta**, invece, il semplice flusso dell'aria in movimento potrebbe giovare (anche in questo caso, esistono sostegni che si possono facilmente installare sul manubrio o altra
struttura tubolare del mezzo).

<p align="center"><img src="img/Car Holder.png" style="width:320px;"></p>


* **Impostazioni di risparmio energetico**  
Nei moderni dispositivi è disponibile la modalità “Risparmio energetico”: si può prolungare la durata della batteria tramite particolari opzioni, come ad esempio la disattivazione delle connessioni di rete, la riduzione della luminosità del display o l'uso di sfondi neri per le app (la cosiddetta “Modalità notte” o “Dark mode”, efficace se il display è di tipo *OLED*.    
Queste funzionalità si possono attivare, in Android, dal menu ***Impostazioni →
Assistenza dispositivo e batteria → Batteria → Risparmio energetico***: si ottiene un minore consumo energetico e più risorse libere, al costo però di sacrificare le prestazioni generali del dispositivo e delle applicazioni.<BR>  

Sia Android che iOS sono poi in grado di “mettere in pausa” le applicazioni non
utilizzate e limitare la frequenza operativa del processore; purtroppo, però, a volte può capitare che il sistema consideri come applicazione da mettere in stand-by anche qualche app che in realtà si vuole mantenere sempre attiva. <BR>   
In Android è possibile indicare al Sistema Operativo quali app considerare
“Importanti”: esse non saranno messe in stato di riposo; per fare ciò
basta ricercare, nelle impostazioni del Sistema Operativo, la funzione "App mai
in sospensione".  
  
  Al solito, i nomi e le posizioni di queste voci di menu possono variare a seconda della versione di Sistema Operativo utilizzata.<BR>
<BR>

<p align="center"><img src="img/App mai in sospensione.png" style="width:320px;"></p>

<br>

---

<BR>
<BR>

# Possibili accorgimenti per velocizzare l'esecuzione di OsmAnd

**In Android**

* **Chiudere tutte le applicazioni non utilizzate**, eliminandole anche
dall'elenco delle App recenti; se le app non sono affatto utilizzate, disinstallarle o disabilitarle;

* **Disabilitare il risparmio energetico** (impostare l'opzione su “Disattivato”), quindi disabilitare il limitatore di velocità della CPU (opzione “Limita
velocità CPU al 70%”) e la limitazione delle app (opzione “Limita app e schermata Home”); se lo si desidera, abilitare di nuovo il risparmio
energetico dopo aver fatto queste modfifiche.

<p align="center"><img src="img/Risparmio energia.png" style="width:320px;"></p>

* **Chiudere tutte le notifiche** presenti nella barra di stato del dispositivo: la loro presenza è infatti associata al relativo processo che gira in background: se ve ne sono molte, ciò può avere impatto negativo sulle prestazioni del sistema.    
  
  Non è necessario disabilitare del tutto le notifiche, sarebbe però bene
autorizzare all'emissione soltanto le app essenziali, come ad esempio email,
SMS, messaggi istantanei ed OsmAnd, naturalmente.  

* **Aggiungere OsmAnd all'elenco delle app *“Mai in sospensione”*** per evitare ch possa venire messo in stand-by dalla gestione del risparmio energetico quando si trova in secondo piano.  
La procedura è semplice, purtroppo però, arrivare al menu che permette di controllare quelle impostazioni è poco intuitivo:

  1. Aprire il menu di Android: ***Impostazioni → Assistenza dispositivo e batteria
→ Limiti per l'uso in background → App mai in sospensione***;
  2. Scorrere l'elenco delle app e verificare se OsmAnd sia presente.
  3. Se OsmAnd non è in elenco, toccare il tasto ***“ + “*** nell'angolo superiore destro del display, scorrere l'elenco delle app e selezionare quindi quella che si desidera escludere dalla sospensione, che verrà così aggiunta alla categoria;
  4. Se l'app cercata non è nemmeno nell'ultimo elenco, verificare il menu: ***Impostazioni → Applicazioni → Accesso speciale → [...] → Ottimizza uso batteria***:   
  se qui il relativo selettore è spostato verso sinistra, significa che l'app è esclusa a priori dall'ottimizzazione: il controllo, infatti, agisce a monte della sospensione delle app.

<p align="center"><img src="img/Ottimizza uso batteria.png" style="width:320px;"></p>

<BR>

**Nell'app**

* **Limitare il numero di tracciati GPX** aperti in OsmAnd nello stesso momento;
* **Utilizzare la mappa di OsmAnd in modalità 2D**
* **Nascondere eventuali livelli aggiuntivi**, come ad esempio l'ombreggiatura del terreno e le linee isoipse, per non gravare eccessivamente sulla GPU;

* **Se si utilizza il motore di rendering *v.2*** (OpenGL), passare alla *v.1*, nativa per Android; si perdono alcune funzionalità della mappa (ad esempio le viste 2.5D/3D), ma vengono impegnate meno risorse di sistema;
* Viceversa, **se il dispositivo è molto recente** (Android 14 o superiore) **e si sta utilizzando il rendering *v.1***, provare ad abilitare la *v.2*: la
visualizzazione nativa, infatti, potrebbe non essere ottimizzata per le versioni più recenti del Sistema Operativo, mentre la GPU potrebbe essere in grado di supportare agevolmente la grafica OpenGL.

* **Se le mappe sono memorizzate su una scheda MicroSD esterna, spostarle** nello spazio di memorizzazione integrato nel dispostivo: il sistema accede infatti a quest'ultimo supporto molto più velocemente.
* Se è attivo un abbonamento ai servizi Pro, **disattivare la visualizzazione dei livelli Meteo e/o Rilievo 3D**;
* Se il dispositivo è datato e/o poco performante, installare ed **utilizzare mappe *“solo strade”*** invece di quelle *“standard”*, per ridurre il numero di dettagli grafici che OsmAnd deve gestire.
<BR>
