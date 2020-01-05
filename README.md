# PROMETHEUS PROJECT

![Prometheus](/images/Prometheus_Adam_Louvre_MR1745_edit_atoma.jpg?raw=true "Prometheus from wikipedia") 

English version below

## MOTIVAZIONE

Non vorrei essere pessimista, ma in alcuni degli scenari futuri possibili ci aspetta una brusca riduzione delle risorse.

Mancanza di accesso alla rete o brusca riduzione/controllo di essa, perdita della rete elettrica e conseguente carenza di energia. In questi scenari verrebbe a mancare tutto quello che attualmente viene offerto da internet: repositories, capacita' di calcolo, documentazione, etc... 

In alcuni scenari potrebbe essere necessario trasformare vecchia tecnologia in devices utili a nuovi scopi: cluster di processori per aumentare la capacita' di calcolo, sistemi di sorveglianza a basso costo, modifica di apparecchiature elettroniche ed industriali per nuovi utilizzi. 

Questo progetto si propone di creare un device (*pipboy*) completamente open e off-grid in grado di essere utile in caso di scenari *apocalittici*.

Un device in grado di funzionare scollegato dalla rete e con batterie di fortuna e/o pannelli solari, in grado di "hackare" altri device per trasformarli in qualcosa di utile, in grado di lavorare off-grid in assenza di tutto quello che attualmente viene offerto dalla una connessione ad internet: repositories, capacita' di calcolo, documentazione, etc.

Pipboy deve essere in grado di controllare al meglio il consumo della batteria, riducendo al minimo l'utilizzo dell'interfaccia grafica e l'uso di periferiche non necessarie.

## PIBOY

	 ┌─────────────────────────────────────────────────────┐ 
	 │01010000 01001001 01010000 01000010 01001111 01011001│ 
	 │    _____  _____  _____      ______   _____  __   __ │ 
	 │   |_____]   |   |_____] ___ |_____] |     |   \_/   │ 
	 │   |       __|__ |           |_____] |_____|    |    │ 
	 │                _      __     __     __              │ 
	 │               '  )  /   )  /   )  /   )             │ 
	 │              ,--'  /   /  /   /  /   /              │ 
	 │             /___  (__ /  (__ /  (__ /               │ 
	 │                                                     │ 
	 │01010000 01001001 01010000 01000010 01001111 01011001│ 
	 └─────────────────────────────────────────────────────┘                  

### CARATTERISTICHE

Il device deve contenere

 * documentazione, documentazione, documentazione
 * strumenti per la compilazione e decompilazione
 * drivers per accesso a protocolli di basso livello (UART-I2C-DSI-GPIO-SERIAL)
 * drivers e periferiche per segnale satellitare
 * drivers e periferiche per segnale radio 
 * strumenti per "flashare" e modificare microchip (recupero vecchia tecnologia)
 * strumenti per root access in iOS e Android
 * strumenti per convertire device con architetture diverse in un cluster con capacita' di calcolo
 * strumenti per convertire device Android e iOS in sistemi di sorverglianza a basso costo

Altro:

 * Android SDK per compilare software android
 * software e repository di progetti stampa 3D
 * manuali di sopravvivenza
 
### SOFTWARE

 * uno script  **boostrap** in grado di preparare una immmagine disco per il device, un disco per i repositories offline, etc...
 * uno script **install** che crea un nuovo user, rende sicuro un device, installa i software necessari e prepare il device
 * uno script **update** che aggiorna un device esistente
 * uno strumento **test** che prova periferiche e devices
 * uno script **freeze** che prepara un immagine disco post-install o update

### DEV NOTES
 
 * scripting con **bash** per la gestione del device (install, update, etc).
 * strumenti vari scritti in **go**

## PIPBOY HARDWARE

Attualmente il mio pipboy e' composta da:

 * Rasperry PI 4 B
 * 7" Touch screen
 * Periboard keyboard
