# PenguinsDataAnalysis
Prima di iniziare l'analisi importo le librerie che mi serviranno allo scopo.
Inizio la fase EDA:
- Uso il metodo describe() icludendo tutto il DataFrame;
- Controllo da quante righe e quante colonne è composto il DataFrame;
- Controllo se esistono duplicati;

### Descrizione del DataFrame
Il DataFrame penguins è composto da 7 colonne e 344 righe.

Le colonne:

- species è di tipo stringa. Ha solo 3 tipi di valori e contiene la specie di appartenenza del pinguino
- island è di tipo stringa. Ha solo 3 tipi di valori e contiene l'isola in cui vive il pinguino
- bill_length_mm è di tipo numerico e contiene la lunghezza del pinguino espressa in millimetri
- bill_depth_mm è di tipo numerico e contiene la larghezza del pinguino espressa in millimetri
- flipper_length_mm è di tipo  numerico e contiene la lunghezza della pinna del pinguino espressa in millimetri
- body_mass_g è di tipo numerico e contiene il peso del pinguino espresso in grammi
- sex è di tipo stringa. Ha solo 3 valori e contiene il sesso del pinguino.

## Data Cleaning
Ho riscontrato il pattern dove il sesso era uguale ad "." quindi essendo non conforme ai dati prima di creare la copia del dataframe ho eliminato la riga corrispondente andando a filtrare i dati.

Rinomino le colonne del DataFrame:
- species in Specie
- island in Isola
- bill_length_mm in LunghezzaMM
- bill_depth_mm in LarghezzaMM
- flipper_length_mm in LunghezzaPinnaMM
- body_mass_g in PesoGR
- sex in Sesso

Successivamente controllo se ci sono righe con valori nulli e in quali colonne si trovano questi ultimi, e vado ad eliminarli definitivamente in quanto inutili ai fini dell'analisi.

Aggiungo delle colonne nelle quali converto i grammi in Kilogrammi e i millimetri in Centimetri

## Data Manipulation
### Distribuzione della Specie

Vado a calcolare come sono distribuiti i pinguini nelle varie isole, e lo faccio per specie e sesso

Concludo l'analisi inserendo dei grafici per visualizzare la distribuzione del peso tra i pinguini. Nello specifico inserisco Istogramma, Kde e Scatter.



# ENGLISH VERSION

# PenguinsDataAnalysis

Before starting the analysis, I import all the libraries needed for the project.

I begin the EDA phase by:
- Using the `describe()` method on the entire DataFrame  
- Checking the number of rows and columns  
- Verifying the presence of duplicates  

### DataFrame Description
The *penguins* DataFrame consists of **7 columns** and **344 rows**.

The columns:

- **species**: string type. Contains 3 possible values and indicates the penguin species  
- **island**: string type. Contains 3 possible values and indicates the island where the penguin lives  
- **bill_length_mm**: numeric type. Contains the penguin’s bill length in millimeters  
- **bill_depth_mm**: numeric type. Contains the penguin’s bill depth in millimeters  
- **flipper_length_mm**: numeric type. Contains the penguin’s flipper length in millimeters  
- **body_mass_g**: numeric type. Contains the penguin’s body mass in grams  
- **sex**: string type. Contains 3 possible values and indicates the penguin’s sex  

## Data Cleaning
I identified a pattern where the value `"."` appeared in the *sex* column. Since it was not consistent with the dataset, I removed the corresponding row before creating a cleaned copy of the DataFrame.

I then renamed the columns as follows:
- *species* → **Specie**  
- *island* → **Isola**  
- *bill_length_mm* → **LunghezzaMM**  
- *bill_depth_mm* → **LarghezzaMM**  
- *flipper_length_mm* → **LunghezzaPinnaMM**  
- *body_mass_g* → **PesoGR**  
- *sex* → **Sesso**  

After that, I checked for missing values, identified which columns contained them, and removed the corresponding rows since they were not useful for the analysis.

I also added new columns converting grams to kilograms and millimeters to centimeters.

## Data Manipulation
### Species Distribution
I calculated how penguins are distributed across the different islands, grouping the results by species and sex.

I concluded the analysis by creating visualizations to explore the distribution of penguin body mass. Specifically, I included a histogram, KDE plot, and scatter plot.


