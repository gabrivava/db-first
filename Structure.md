# Database Auto usate

<!-- Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario. -->

## (table) Cars

- id                  BINGINT PRIMARY KEY AUTOINCREMENT UNIQUE NOTNULL 
- name                VARCHAR(50) NOTNULL
- company             VARCHAR(50) NOTNULL INDEX
- model               VARCHAR(255) NOTNULL INDEX <!-- tipo di modello: utilitaria | monovolume | suv | ecc..  -->
- peso                MEDIUMINT NULL
- prezzo              DECIMAL(8,2)
- cilindrata          MEDIUMINT NULL
- dimensioni          VARCHAR(20) NULL
- porte               TINYINT NULL
- fuel                VARCHAR(40) NOTNULL
- chilometraggio      MEDIUMINT NOTNULL
- anno di uscita      YEAR NOTNULL
- usata               TINYINT NOTNULL <!-- 1 VERO| 0 FALSE -->
- proprietari         TINYINT NOTNULL
- decrizione          TEXT NULL
- max_speed           SMALLINT NULL
- colore_esterno      VARCHART(20) NOTNULL
- interni             VARCHART(40) NULL
- cambio              VARCHART(20) NOTNULL <!-- AUTOMATICO, MARCE -->
- marce               TINYINT NOTNULL
- emissioni(g/km)     SMALLINT NULL <!-- emissioni in g/km(CO2) -->
- classe emissioni    VARCHART(10) NOTNULL   