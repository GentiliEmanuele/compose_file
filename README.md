# compose_file
**Regole per l'esecuzione dell'applicazione**

***Configurazione del service registry***
Per modificare la configurazione del service registry si deve modificare questo file. In particolare, è possibile cambiare il numero di porta su cui esso si mette in ascolto e l'indirizzo IP. Quando si modifica il numero di porta del service registry si deve anche modificare la variabile d'ambiente *REGISTRY* per tutti i server. E' necessario anche cambiare il numero di porta che il container deve esporre nella direttiva ports.
Link alla repository: https://github.com/GentiliEmanuele/service_registry.git

***Configurazione dei server***
E'possibile modificare il numero di porta con considerazioni analoghe a quelle fatte per il service registry. Inoltre, è possibile modificare l'indirizzo IP che viene assegnato a ciascun server. Queste modifiche non richiedono ulteriori aggiornamenti del file di configurazione.
Per aggiungere un server basta utilizzare una struttura analoga a quella degli altri server cambiando solamente la porta dell'host sulla quale viene mappata la porta del container e l'indirizzo IP.
Link alla repository: https://github.com/GentiliEmanuele/server.git

***Configurazione del load balancer***
Anche in questo caso si può modificare l'indirizzo IP e il numero di porta. La variazione richiede anche di aggiornare le righe del file di configurazione relative al client in modo che esso conosca i nuovi indirizzi.
Link alla repository: https://github.com/GentiliEmanuele/load_balancer.git

***Configurazione del client***
Si può modificare l'indirizzo IP e i parametri passati ai servizi che permettono di testare l'applicazione.
Link alla repository: https://github.com/GentiliEmanuele/client.git
