# ML-for-Predictive-Maintenance
Progetto di tesi presso l'Università degli Studi dell'Insubria che si occupa della realizzazione di un modello di machine learning  con l'obiettivo di ottenere un  sistema di manutenzione predittiva in un ambiente industriale da poter integrare all’interno del progetto di tesi magistrale di Andrea Chiericati in collaborazione con il Dottor Gianfranco Modoni, operativo presso il Consiglio Nazionale delle Ricerche (CNR) di Bari. La soluzione proposta si basa sulla realizzazione e il confronto di molteplici modelli di machine learning basati su due algoritmi: il Support Vector Machine e il Random Forest.
Tutto il progetto è stato sviluppato su Ubuntu 20.04.

## Set-up dell'ambiente di sviluppo
Prima di installare PySpark bisogna verificare di soddisfare il seguente prerequisito. Spark è scritto in Scala Programming Language e funziona in ambiente Java Virtual Machine (JVM). Ecco perché bisogna verificare di aver installato un Java Development Kit (JDK). E' importante avere una versione 8 o superiore, in questo progetto si è utilizzata la versione 11.0.11.
Inoltre, è necessario aver precedentemente installato Python, in questo progetto si è utilizzato Python v. 3.8.8. Consiglio di installare Python con il package manager Anaconda (qui le istruzioni per installare Anaconda: https://docs.anaconda.com/anaconda/install/linux/).
### Installazione PySpark
E' possibile installare PySpark con l'aiuto di `pip`:
```bash
$ pip install pyspark
```
**Nota**: potrebbe impiegarci un po' di tempo.
Assicurati di decomprimere la directory che appare nella cartella `Download`. Si può fare automaticamente, facendo doppio clic sull'archivio `spark-2.2.0-bin-hadoop2.7.tgz` o aprendo il terminale ed eseguendo il seguente comando:
```bash
$ tar xvf spark-2.2.0-bin-hadoop2.7.tgz
```
Spostare la cartella decompressa in `/usr/local/spark` eseguendo la seguente riga:
```bash
$ mv spark-2.1.0-bin-hadoop2.7 /usr/local/spark
```
**Nota**: che se ricevi un errore che dice che l'autorizzazione è negata per spostare questa cartella nella nuova posizione, bisogna aggiungere `sudo` davanti a questo comando.

### Installazione Jupyter
Per installare Jupyter Notebook eseguire il seguente comando sul terminale:
```bash
$ pip install jupyter
```
## JupyterLab
Prima di tutto aprire l'ambiente di sviluppo JupyterLab con il seguente comando:
```bash
$ jupyter-lab
```
**Nota**: se da un errore del tipo "L'accesso al file è stato negato", copiare e incollare nel browser il secondo link che appare nel terminale dopo l'esecuzione del comando.
A questo punto è possibile scaricare i due file `.ipynb` presenti in questa repo e fare l'upload nel JupyterLab. Prima di poter eseguire i notebook è necessario effettuare il download del dataset (https://archive.ics.uci.edu/ml/machine-learning-databases/00601/) e installare le seguenti librerie.

## Installazione librerie necessarie
* **Pandas**: `pip install pandas`
* **Seaborn**: `pip install seaborn`
* **Matplotlib**: `pip install matplotlib`
* **Scikit-learn**: `pip install -U scikit-learn`
* **Imblearn**: `pip install -U imbalanced-learn`
* **Handy spark**: `pip install handyspark`
