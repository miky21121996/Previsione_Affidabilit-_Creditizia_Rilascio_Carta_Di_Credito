# Previsione dell'Affidabilità Creditizia per il Rilascio della Carta di Credito

Realizzare un modello in grado di stimare l'affidabilità creditizia dei clienti. Questo modello aiuterà a comprendere se accettare o meno la richiesta per il rilascio della carta di credito.

## Dati Forniti
A disposizione ci sono i dati anonimizzati di clienti che hanno già ottenuto la carta di credito e ne pagano regolarmente le rate. I dati sono disponibili in un file CSV:

- **File**: `credit_scoring.csv`

Il file contiene le informazioni sui correntisti che hanno richiesto l’apertura di una linea di credito.

### Colonne del Dataset:
- **ID**: numero identificativo del cliente.
- **CODE_GENDER**: sesso del cliente.
- **FLAG_OWN_CAR**: indicatore del possesso di un'automobile.
- **FLAG_OWN_REALTY**: indicatore del possesso di una casa.
- **CNT_CHILDREN**: numero di figli.
- **AMT_INCOME_TOTAL**: reddito annuale.
- **NAME_INCOME_TYPE**: tipo di reddito.
- **NAME_EDUCATION_TYPE**: livello di educazione.
- **NAME_FAMILY_STATUS**: stato civile.
- **NAME_HOUSING_TYPE**: tipo di abitazione.
- **DAYS_BIRTH**: numero di giorni trascorsi dalla nascita.
- **DAYS_EMPLOYED**: numero di giorni trascorsi dalla data di assunzione (se positivo, indica il numero di giorni da quando è disoccupato).
- **FLAG_MOBIL**: indicatore della presenza di un numero di cellulare.
- **FLAG_WORK_PHONE**: indicatore della presenza di un numero di telefono di lavoro.
- **FLAG_PHONE**: indicatore della presenza di un numero di telefono.
- **FLAG_EMAIL**: indicatore della presenza di un indirizzo email.
- **OCCUPATION_TYPE**: tipo di occupazione.
- **CNT_FAM_MEMBERS**: numero di familiari.
- **TARGET**: variabile che vale 1 se il cliente ha un'alta affidabilità creditizia (pagamento costante delle rate), 0 altrimenti.

## Obiettivo
L'obiettivo è costruire un modello che preveda il **target**, ovvero la variabile **TARGET** che indica se il cliente ha una buona affidabilità creditizia.
Se ad un cliente viene negata la carta di credito, il team deve essere in grado di fornirgli una spiegazione. Questo significa che il modello deve essere interpretabile e deve fornire
