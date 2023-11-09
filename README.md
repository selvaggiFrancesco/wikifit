Requisiti funzionali:

-Registrazione dell'utente: Il sito deve consentire agli utenti di registrarsi fornendo le informazioni necessarie come nome, indirizzo e-mail e password<br>
-Visualizzazione dei contenuti: Gli utenti registrati devono poter accedere a contenuti informativi riguardanti il mondo del fitness come articoli, guide, video e programmi di allenamento<br>
-Coaching online: Il sito deve fornire servizi di coaching online, consentendo agli utenti di prenotare sessioni di allenamento individuali o di gruppo tramite videochiamata<br>
-Vendita di prodotti: Devono essere disponibili prodotti fitness come attrezzature, integratori alimentari da acquistare tramite il sito<br>
-Pianificazione e monitoraggio degli allenamenti: Gli utenti devono poter creare programmi di allenamento personalizzati e tenere traccia dei propri progressi nel tempo<br>
-Forum e community: Il sito deve avere un forum o una sezione di community che permetta agli utenti di interagire tra loro, condividere esperienze e porre domande agli esperti<br>


Requisiti non funzionali:

-Scalabilità utenti: Il sito deve essere in grado di gestire un numero crescente di utenti senza influire sulle prestazioni<br>
-Sicurezza: Devono essere implementate misure di sicurezza per proteggere le informazioni personali degli utenti e impedire accessi non autorizzati<br>
-Esperienza utente: Il sito deve essere intuitivo e facile da navigare, offrendo un'esperienza utente positiva e coinvolgente<br>
-Tempi di risposta veloci: Le pagine del sito devono caricarsi rapidamente per evitare tempi di attesa lunghi<br>
-Disponibilità: Il sito deve essere sempre accessibile e funzionante, minimizzando il tempo di inattività<br>


Requisiti di dominio:

-Conoscenze sul fitness: Gli sviluppatori devono avere una conoscenza approfondita del mondo del fitness per garantire la correttezza e l'affidabilità delle informazioni fornite<br>
-Gestione dei pagamenti: Il sito deve integrare un sistema di pagamento sicuro per le transazioni relative alla vendita di prodotti e ai servizi di coaching online<br>


Requisiti utente:

-login facile: gli utenti devono essere in grado di registrarsi facilmente fornendo le informazioni richieste<br>
-navigazione: gli utenti devono poter accedere e navigare facilmente tra i contenuti informativi<br>
-acquisti: gli utenti devono poter effettuare acquisti di prodotti in modo rapido e sicuro<br>


Requisiti di sistema:

-pagamento: il sistema di pagamento deve essere integrato in modo sicuro per la gestione delle transazioni online<br>
-funzione help: il sito deve essere supportato da un team di assistenza tecnica in grado di rispondere alle richieste degli utenti e risolvere eventuali problemi tecnici<br>
<br><br><br>

il sito è formato da tre grandi sezioni: "esplora" è un insieme di informazioni riguardanti gli esercizi e i piani di allenamento, informando l'utente e ampliando la sua conoscenza. "allenati" fornisce un confronto tra personal trainer e clienti, in modo tale da creare piani di allenamento e schede personalizzate alle esigenze di chi si deve allenare (il profilo del personal trainer sarà compilato da lui/lei stesso/a, allegando certificazioni e specializzazioni in modo tale da essere raggiunto da clienti con obiettivi che coincidono con la preparazione e l'esperienza del trainer). "acquista" è come se fosse un negozio online di integratori e accessori per la palestra, è presente una raccolta punti che, in base al punteggio permette di ricevere sconti, avere la consegna gratis e riscuotere prodotti in omaggio.<br><br>

STUDIO DI FATTIBILITA':<br>
i costi saranno principalmente caratterizzati dalla creazione e manutenzione del sito, e della rivendita dei prodotti.<br>
le fonti di guadagno sono caratterizzate da una percentuale dei servizi venduti dai trainer e dalla rivendita dei prodotti, inoltre è presente una funzione che permette ai trainer di aumentare la loro visibilità per un periodo limitato di tempo
all'interno del sito pagando un abbonamento.







[cliente]-(Sign In),
[cliente]-(acquisto prodotti),
[cliente]-(acquisto schede),
(acquisto prodotti)>(prodotti fitness),
(acquisto prodotti)>(Checkout),
[trainer]-(vendita schede),
(acquisto schede)<(accumulo punti),
(acquisto prodotti)<(accumulo punti),
(vendita schede)>(autenticazione trainer)<br>
<img src="http://yuml.me/diagram/scruffy/usecase/[cliente]-(Sign In),[cliente]-(acquisto prodotti),[cliente]-(acquisto schede),(acquisto prodotti)>(prodotti fitness),(acquisto prodotti)>(Checkout),[trainer]-(vendita schede),(acquisto schede)<(accumulo punti),(acquisto prodotti)<(accumulo punti),(vendita schede)>(autenticazione trainer)" >
