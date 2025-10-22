# Prova Pratica

## Obiettivo:
Realizzare un programma Python che gestisca un archivio di playlist musicali per diversi utenti, impiegando tecniche di programmazione funzionale, decoratori e una buona organizzazione del codice in moduli.
## Specifiche:
1. **Gestione Utenti:**
    - All’avvio del programma, consentire di selezionare un utente esistente o di crearne uno nuovo.
    - Ogni utente possiede un archivio personale di playlist.
2. **Creazione e Gestione di Playlist:**
   Una volta selezionato l’utente, deve essere possibile creare nuove playlist specificando:
    - Titolo della playlist
    - Data di creazione
    - Descrizione (facoltativa)
3. **In ogni playlist è possibile aggiungere brani musicali. Per ogni brano:**
    - Titolo del brano
    - Artista
    - Durata (in secondi o in formato mm:ss)
    - Genere (ad es. “Rock”, “Pop”, “Classica”)
4. **Filtraggio e Funzioni Funzionali:**
    - Fornire funzioni che permettano di filtrare, trasformare e analizzare l’insieme dei brani dell’utente. Ad esempio:
        - Filtrare tutti i brani di un determinato genere
        - Calcolare la durata totale di una playlist utilizzando ```reduce```
        - Estrarre una lista di titoli di canzoni mappando i brani tramite ```map```
    - Permettere di visualizzare playlist o brani filtrati secondo criteri definiti dall’utente.
5. **Decoratori**:
    - Implementare almeno un decoratore personalizzato da applicare su funzioni chiave. Il decoratore potrebbe, ad esempio:
        - Validare i dati inseriti (es. controllare che il titolo di una playlist non sia vuoto, che la durata del brano sia > 0)
        - Effettuare logging su file delle operazioni di creazione/modifica playlist o brani
        - Misurare i tempi di esecuzione di determinate operazioni di filtraggio o esportazione
6. **Backup e Ripristino:**
    - Salvare l’archivio (playlist e brani) di un utente su un file di backup (ad es. in formato pickle).
    - Permettere di ripristinare i dati da tale file di backup.
7. **Esportazione:**
    - Consentire l’esportazione di una playlist (o di un sottoinsieme filtrato dei suoi brani) in un file testuale.
    - L’esportazione deve includere tutte le informazioni: titolo della playlist, data, descrizione, elenco dei brani con i loro dettagli.
8. **Utilizzo da Linea di Comando:**
    - Fornire un modulo eseguibile da linea di comando che:
        - Prenda in input il nome dell’utente
        - Applichi un filtro (ad es. tutte le playlist di genere “Rock” o tutti i brani di un certo artista)
        - Esporti il risultato filtrato in un file testuale passato come parametro
    - Il modulo non deve richiedere input interattivo, tutti i parametri devono essere forniti da riga di comando.

**[Bonus] Test Suite:**
Scrivere almeno una Test Suite con almeno un caso di test per verificare il corretto funzionamento di una o più funzionalità (es. creazione di una playlist, aggiunta di un brano, filtraggio dei brani, validazione dei dati via decoratore).