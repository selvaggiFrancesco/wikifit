**Progetto di piattaforma fitness con Multitenancy**

**Requisiti funzionali:**

- **Registrazione dell'utente:** La piattaforma consente agli utenti di registrarsi fornendo le informazioni necessarie come nome, indirizzo e-mail e password.
  
- **Visualizzazione dei contenuti:** Gli utenti registrati possono accedere a contenuti informativi riguardanti il mondo del fitness, quali articoli, guide, video e programmi di allenamento.
  
- **Coaching online:** La piattaforma offre servizi di coaching online, permettendo agli utenti di prenotare sessioni di allenamento individuali o di gruppo tramite videochiamata.
  
- **Pianificazione e monitoraggio degli allenamenti:** Gli utenti possono creare programmi di allenamento personalizzati e tenere traccia dei propri progressi nel tempo.
  
- **Forum e community:** La piattaforma dispone di un forum o una sezione di community che consente agli utenti di interagire tra loro, condividere esperienze e porre domande agli esperti.

**Requisiti non funzionali:**

- **Scalabilità utenti:** La piattaforma è in grado di gestire un numero crescente di utenti senza influire sulle prestazioni, mantenendo la separazione tra i dati di ogni tenant.
  
- **Sicurezza:** Sono implementate misure di sicurezza per proteggere le informazioni personali degli utenti e impedire accessi non autorizzati, assicurando la privacy dei dati per ogni tenant.
  
- **Esperienza utente:** La piattaforma è intuitiva e facile da navigare, offrendo un'esperienza utente positiva e coinvolgente per ogni tenant.
  
- **Tempi di risposta veloci:** Le pagine del sito caricano rapidamente per evitare tempi di attesa lunghi, assicurando una navigazione fluida per tutti gli utenti.
  
- **Disponibilità:** La piattaforma è sempre accessibile e funzionante, minimizzando il tempo di inattività per ogni tenant.

**Requisiti di dominio:**

- **Conoscenze sul fitness:** Gli sviluppatori hanno una conoscenza approfondita del mondo del fitness per garantire la correttezza e l'affidabilità delle informazioni fornite a tutti i tenant.
  
- **Gestione dei pagamenti:** La piattaforma integra un sistema di pagamento sicuro per le transazioni relative alla vendita di prodotti e ai servizi di coaching online, gestendo in modo separato le transazioni di ogni tenant.

**Requisiti utente:**

- **Login facile:** Gli utenti possono registrarsi facilmente fornendo le informazioni richieste, con un'esperienza di accesso personalizzata per ogni tenant.
  
- **Navigazione:** Gli utenti possono accedere e navigare facilmente tra i contenuti informativi, con una navigazione ottimizzata per ogni tenant.
  
- **Acquisti:** Gli utenti possono effettuare acquisti di prodotti in modo rapido e sicuro, con transazioni gestite in modo separato per ogni tenant.

**Requisiti di sistema:**

- **Pagamento:** Il sistema di pagamento è integrato in modo sicuro per la gestione delle transazioni online, con la possibilità di gestire le transazioni di ogni tenant in modo separato.
  
- **Funzione help:** La piattaforma è supportata da un team di assistenza tecnica in grado di rispondere alle richieste degli utenti e risolvere eventuali problemi tecnici, offrendo supporto personalizzato per ogni tenant.

**Multitenancy:**

La piattaforma è progettata per supportare il multitenancy, consentendo a più entità separate, come palestre, personal trainer o aziende di fitness, di utilizzare la piattaforma contemporaneamente. Ogni tenant ha il proprio spazio personalizzato e gestione degli utenti, con dati e configurazioni separati per garantire l'indipendenza e l'isolamento tra gli utenti. Ciò permette a ogni tenant di offrire i propri servizi ai propri clienti senza interferire con gli altri, con una gestione avanzata delle autorizzazioni e una scalabilità per supportare la crescita degli utenti e dei servizi offerti.
<br>
<br><br><br>

Il sito è formato da tre grandi sezioni: "esplora" è un insieme di informazioni riguardanti gli esercizi e i piani di allenamento, informando l'utente e ampliando la sua conoscenza. "allenati" fornisce un confronto tra personal trainer e clienti, in modo tale da creare piani di allenamento e schede personalizzate alle esigenze di chi si deve allenare (il profilo del personal trainer sarà compilato da lui/lei stesso/a, allegando certificazioni e specializzazioni in modo tale da essere raggiunto da clienti con obiettivi che coincidono con la preparazione e l'esperienza del trainer). "acquista" è come se fosse un negozio online di integratori e accessori per la palestra, è presente una raccolta punti che, in base al punteggio permette di ricevere sconti, avere la consegna gratis e riscuotere prodotti in omaggio.<br>
È inoltre presente un forum per la community che consente agli utenti di mettersi in cotatto tra di loro e conversare discutendo attraverso messaggi scritti, c'è la possibilità di creare un avatar per personalizzare il proprio profilo.<br>
I moderatori e amministratori dispongono della propria etichetta (blu per i moderatori, rossa per gli amministratori) che li contraddistingue dagli ospiti.<br>
I moderatori hanno il compito di gestire quelli che sono i messaggi postati dagli utenti, chiudere discussioni non consone, gestire l'ordine all'interno del forum e rispondere ad eventuali domande.<br>
Gli amministratori possono chiudere il forum, modificarlo, apportare cambiamenti al software, espellere, cancellare o creare utenti.<br><br>

STUDIO DI FATTIBILITA':<br>
i costi saranno principalmente caratterizzati dalla creazione e manutenzione del sito, e della rivendita dei prodotti.<br>
le fonti di guadagno sono caratterizzate da una percentuale dei servizi venduti dai trainer e dalla rivendita dei prodotti, inoltre è presente una funzione che permette ai trainer di aumentare la loro visibilità per un periodo limitato di tempo
all'interno del sito pagando un abbonamento.







[cliente]-(Sign In), [cliente]-(acquisto prodotti), 
[cliente]-(acquisto schede), 
(acquisto prodotti)>(prodotti fitness), 
(acquisto prodotti)>(Checkout), 
[trainer]-(vendita schede), 
(acquisto schede)<(accumulo punti), 
(acquisto prodotti)<(accumulo punti), 
(vendita schede)>(autenticazione trainer),
[moderatore]-(gestire l'ordine nel forum),
(gestire l'ordine nel forum)<(chiudere discussioni),
(gestire l'ordine nel forum)<(rispondere a domande),
[amministratore]-(modifica forum),
(modifica forum)<(apportare cambiamenti),
(modifica forum)<(espellere e creare utenti),
[cliente]-(utilizzo forum),
[amministratore]-(utilizzo forum),
[moderatore]-(utilizzo forum)<br>
<img src="http://yuml.me/diagram/scruffy/usecase/[cliente]-(Sign In), [cliente]-(acquisto prodotti), [cliente]-(acquisto schede), (acquisto prodotti)>(prodotti fitness), (acquisto prodotti)>(Checkout), [trainer]-(vendita schede), (acquisto schede)<(accumulo punti), (acquisto prodotti)<(accumulo punti), (vendita schede)>(autenticazione trainer),[moderatore]-(gestire l'ordine nel forum),(gestire l'ordine nel forum)<(chiudere discussioni),(gestire l'ordine nel forum)<(rispondere a domande),[amministratore]-(modifica forum),(modifica forum)<(apportare cambiamenti),(modifica forum)<(espellere e creare utenti),[cliente]-(utilizzo forum),[amministratore]-(utilizzo forum),[moderatore]-(utilizzo forum)" >


user story:<br><br>
-come personal trainer,<br>
-voglio vendere i miei servizi,<br>
-in modo da avere una fonte di guadagno.<br><br><br>
-come cliente con poche conoscenze,<br>
-voglio informarmi ed essere seguito da un personal trainer,<br>
-in modo che possa migliorare il mio allenamento.<br><br><br>
-come cliente inesperto,<br>
-voglio condividere le mie domande su un forum,<br>
-in modo che altri utenti mi possano rispondere.<br><br><br>
