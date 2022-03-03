# Smartbrain

Il progetto Smartbrain consiste nella creazione di un sito web in React con possibilitá di login e registrazione per usufruire di un servizio, offerto dall'API di Clarifai, per il riconoscimento di volti all'interno di immagini inserite dall'utente loggato. 
La pagina iniziale mostra la finestra di login con la possibilitá di selezionare l'opzione di registrazione in caso di nuovo utente. La gestione dell'hashing della password é affidata a bcrypt. 
Una volta verificate le credenziali viene data la possibilitá all'utente di inserire l'url dell'immagine che si vuole analizzare e si mostra il numero di volte che l'utente ha utilizzato il servizio. 
Una volta inviata l'immagine all'API questa viene analizzata e si riceve in risposta tramite stringhe JSON le informazioni relative ai volti trovati dal servizio. I dati ricevuti vengono poi trattati per creare dei riquadri attorno ai volti individuati. 
La parte front-end del sito é realizzata in React, per il lato back-end é stato utilizzato node.js con il framework express.js. 
Il corretto funzionamento del server é stato testato tramite l'utilizzo del software Postman prima di interfacciarlo al front-end. 
Il database di tipo relazionale é stato realizzato tramite la GUI PSequel, programmata con PostgreSQL. 
Il funzionamento del sito si basa sul corretto funzionamento dell'API di Clarifai che tuttavia risulta spesso fuori servizio, sarebbe opportuno trovare una soluzione alternativa per dare maggiore stabilitá all'applicazione.
