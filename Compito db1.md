
## Biblioteca 

### Libri

| Caratteristiche            | dato java        | dato db           | spiegazione                                                                                        |
| -------------------------- | ---------------- | ----------------- | -------------------------------------------------------------------------------------------------- |
| Titolo                     | string           | varchar           | testo                                                                                              |
| Autore                     | string           | varchar           | testo                                                                                              |
| Categoria                  | byte             | tinyint           | testo                                                                                              |
| Anno di pubblicazione==*== | ~~string~~ short | ~~date~~ smallint | per essere in grado poi di classificarli in ordine di uscita                                       |
| Casa Editrice              | string           | varchar           | testo                                                                                              |
| ISBN                       | string           | varchar           | non serve un dato numerico perché l'ISBN è di identificazione e non serve calcolare niente         |
| Scaffale                   | string           | varchar           | se la biblioteca tiene conto di dove è conservato un libro, potrebbe usare un sistema alfanumerico |
| Disponibilità              | boolean          | bit               | è disponibile, sì o no?                                                                            |
| Descrizione                | string           | text              | in text ci stanno più caratteri                                                                    |
==`*`==anno di pubblicazione - l'anno non è una data, ma un numero intero 
### Membro

| Caratteristiche       | dato java                | dato db           | spiegazione                                                                                             |
| --------------------- | ------------------------ | ----------------- | ------------------------------------------------------------------------------------------------------- |
| Nome                  | string                   | varchar           | testo                                                                                                   |
| Cognome               | string                   | varchar           | testo                                                                                                   |
| Data di nascita       | ~~string~~ localDate     | date              | data                                                                                                    |
| Numero di telefono    | string                   | varchar           | anche questo, essendo un numero con cui non andrò a fare calcoli, non serve classificarlo numericamente |
| Indirizzo             | string                   | varchar           | testo                                                                                                   |
| Email                 | string                   | varchar           | testo                                                                                                   |
| Numero di tessera     | string                   | varchar           | numero di identificazione                                                                               |
| Data di registrazione | ~~string~~ localDateTime | ~~date~~ datetime | data, ora e minuti della registrazione                                                                  |

### Prestito

| Caratteristiche   | dato java            | dato db  | spiegazione                       |
| ----------------- | -------------------- | -------- | --------------------------------- |
| Membro            | string               | varchar  | testo                             |
| Libro             | string               | varchar  | testo                             |
| Data del prestito | ~~string~~ localdate | date     | data                              |
| Data consegna     | ~~string~~ localdate | date     | data                              |
| Stato             | short                | smallint | meglio averlo numerico in backend |
| Cauzione          | float                | decimal  |                                   |



## Catalogo ristorante

### Piatto

| Caratteristiche               | dato java       | dato db             | spiegazione                                                                                            |
| ----------------------------- | --------------- | ------------------- | ------------------------------------------------------------------------------------------------------ |
| Nome                          | string          | varchar             | testo                                                                                                  |
| Ingredienti                   | string          | varchar             | testo                                                                                                  |
| Categoria (primo, dolce, ecc) | ~~string~~ byte | ~~varchar~~ tinyint | utilizzare una strategia numerica così è più facile da gestire. traduzioni varie gestite in front end. |
| Descrizione                   | string          | text                | testo                                                                                                  |
| Disponibilità                 | boolean         | bit                 |                                                                                                        |
| Foto                          | string          | text                | rimanda al nome dell'immagine                                                                          |
| Variazioni                    | string          | text                | testo                                                                                                  |
| Allergeni                     | string          | varchar             | testo                                                                                                  |
| Calorie                       | short           | smallint            |                                                                                                        |
| Prezzo                        | double          | decimal             | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario  |

### Ingrediente

| Caratteristiche                  | dato java | dato db | spiegazione                                                                                            |
| -------------------------------- | --------- | ------- | ------------------------------------------------------------------------------------------------------ |
| Nome                             | string    | varchar | testo                                                                                                  |
| Descrizione                      | string    | text    | testo                                                                                                  |
| Foto                             | string    | varchar |                                                                                                        |
| Tipologia (pasta, proteine, ecc) | byte      | tinyint | utilizzare una strategia numerica così è più facile da gestire. traduzioni varie gestite in front end. |
| Fornitore                        | string    | varchar | testo                                                                                                  |
| Disponibilità                    | boolean   | bit     |                                                                                                        |
| Modalità di conservazione        | string    | varchar |                                                                                                        |
| Costo                            | float     | decimal | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario  |
### Clienti

| Caratteristiche    | dato java     | dato db  | spiegazione   |
| ------------------ | ------------- | -------- | ------------- |
| Nome               | string        | varchar  | testo         |
| Cognome            | string        | varchar  | testo         |
| Numero di telefono | string        | varchar  | numero di tel |
| Data di nascita    | localdate     | date     |               |
| data iscrizione    | localDateTime | datetime |               |
| email              | string        | varchar  |               |
| username           | string        | varchar  |               |
| password           | string        | varchar  |               |
| note               | string        | text     |               |


## Negozio di fiori

### Fiore

| Caratteristiche      | dato java | dato db  | spiegazione                                                                                           |
| -------------------- | --------- | -------- | ----------------------------------------------------------------------------------------------------- |
| Nome                 | string    | varchar  | testo                                                                                                 |
| Colore               | string    | varchar  | testo                                                                                                 |
| Prezzo               | float     | decimal  | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario |
| Quantità disponibile | short     | smallint | numero con cui farò dei calcoli                                                                       |
### Fornitore

| Caratteristiche    | dato java | dato db | spiegazione   |
| ------------------ | --------- | ------- | ------------- |
| Nome/azienda       | string    | varchar | testo         |
| Fornitore          | string    | varchar | testo         |
| Indirizzo          | string    | varchar | testo         |
| Email              | string    | varchar | testo         |
| Numero di telefono | string    | varchar | numero di tel |

### Cliente

| Caratteristiche    | dato java | dato db | spiegazione               |
| ------------------ | --------- | ------- | ------------------------- |
| Nome               | string    | varchar | testo                     |
| Cognome            | string    | varchar | testo                     |
| Tessera fedeltà    | string    | varchar | numero di identificazione |
| Data di nascita    | localDate | date    | data                      |
| Numero di telefono | string    | varchar | numero di tel             |
