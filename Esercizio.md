
## Biblioteca 

### Libri

| Caratteristiche       | dato java | dato db | spiegazione                                                                                        |
| --------------------- | --------- | ------- | -------------------------------------------------------------------------------------------------- |
| Titolo                | string    | varchar | testo                                                                                              |
| Autore                | string    | varchar | testo                                                                                              |
| Categoria             | string    | varchar | testo                                                                                              |
| Anno di pubblicazione | string    | date    | per essere in grado poi di classificarli in ordine di uscita                                       |
| Casa Editrice         | string    | varchar | testo                                                                                              |
| ISBN                  | string    | varchar | non serve un dato numerico perché l'ISBN è di identificazione e non serve calcolare niente         |
| Scaffale              | string    | varchar | se la biblioteca tiene conto di dove è conservato un libro, potrebbe usare un sistema alfanumerico |
| Disponibilità         | boolean   | boolean | è disponibile, o no?                                                                               |

### Membri

| Caratteristiche       | dato java | dato db | spiegazione                                                                                             |
| --------------------- | --------- | ------- | ------------------------------------------------------------------------------------------------------- |
| Nome                  | string    | varchar | testo                                                                                                   |
| Cognome               |           |         |                                                                                                         |
| Numero di tessera     | string    | varchar | numero di identificazione                                                                               |
| Data di nascita       | string    | date    | data                                                                                                    |
| Email                 | string    | date    | testo                                                                                                   |
| Numero di telefono    | string    | date    | anche questo, essendo un numero con cui non andrò a fare calcoli, non serve classificarlo numericamente |
| Indirizzo             | string    | varchar | testo                                                                                                   |
| Data di registrazione | string    | date    | data                                                                                                    |

### Prestiti

| Caratteristiche   | dato java | dato db | spiegazione |
| ----------------- | --------- | ------- | ----------- |
| Membro            | string    | varchar | testo       |
| Libro             | string    | varchar | testo       |
| Data del prestito | string    | date    | data        |
| Data consegna     | string    | date    | data        |



## Catalogo ristorante

### Piatti

| Caratteristiche               | dato java | dato db | spiegazione                                                                                           |
| ----------------------------- | --------- | ------- | ----------------------------------------------------------------------------------------------------- |
| Nome                          | string    | varchar | testo                                                                                                 |
| Ingredienti                   | string    | varchar | testo                                                                                                 |
| Categoria (primo, dolce, ecc) | string    | varchar | testo                                                                                                 |
| Descrizione                   | string    | varchar | testo                                                                                                 |
| Prezzo                        | double    | decimal | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario |

### Ingredienti

| Caratteristiche               | dato java | dato db | spiegazione                                                                                           |
| ----------------------------- | --------- | ------- | ----------------------------------------------------------------------------------------------------- |
| Nome                          | string    | varchar | testo                                                                                                 |
| Tipo (pasta, proteine, ecc)   | string    | varchar | testo                                                                                                 |
| Fornitore                     | string    | varchar | testo                                                                                                 |
| Data di acquisto/preparazione | string    | date    | data                                                                                                  |
| Data di scadenza              | string    | date    | data                                                                                                  |
| Costo                         | float     | decimal | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario |
### Clienti

| Caratteristiche    | dato java | dato db | spiegazione               |
| ------------------ | --------- | ------- | ------------------------- |
| Nome               | string    | varchar | testo                     |
| Cognome            | string    | varchar | testo                     |
| Tessera fedeltà    | string    | varchar | numero di identificazione |
| Data di nascita    | string    | date    | data                      |
| Numero di telefono | string    | date    | numero di tel             |


## Negozio di fiori

### Fiori

| Caratteristiche      | dato java | dato db  | spiegazione                                                                                           |
| -------------------- | --------- | -------- | ----------------------------------------------------------------------------------------------------- |
| Nome                 | string    | varchar  | testo                                                                                                 |
| Colore               | string    | varchar  | testo                                                                                                 |
| Prezzo               | float     | decimal  | un numero a virgola mobile che è un prezzo, massimo 2 cifre dopo la virgola, e un calcolo finanziario |
| Quantità disponibile | short     | smallint | numero con cui farò dei calcoli                                                                       |
### Fornitori

| Caratteristiche    | dato java | dato db | spiegazione   |
| ------------------ | --------- | ------- | ------------- |
| Nome/azienda       | string    | varchar | testo         |
| Fornitore          | string    | varchar | testo         |
| Indirizzo          | string    | varchar | testo         |
| Email              | string    | varchar | testo         |
| Numero di telefono | string    | varchar | numero di tel |

### Clienti

| Caratteristiche    | dato java | dato db | spiegazione               |
| ------------------ | --------- | ------- | ------------------------- |
| Nome               | string    | varchar | testo                     |
| Cognome            | string    | varchar | testo                     |
| Tessera fedeltà    | string    | varchar | numero di identificazione |
| Data di nascita    | string    | date    | data                      |
| Numero di telefono | string    | date    | numero di tel             |