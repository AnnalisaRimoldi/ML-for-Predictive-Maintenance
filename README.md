# ML-for-Predictive-Maintenance
Progetto di tesi, sviluppato presso l'Università degli Studi dell'Insubria, che si occupa della realizzazione di un modello di machine learning  con l'obiettivo di ottenere un  sistema di manutenzione predittiva in ambiente industriale da poter integrare all’interno del progetto di tesi magistrale di Andrea Chiericati in collaborazione con il Dottor Gianfranco Modoni, operativo presso il Consiglio Nazionale delle Ricerche (CNR) di Bari. La soluzione proposta si basa sulla realizzazione e il confronto di molteplici modelli di machine learning basati su due algoritmi: il Support Vector Machine e il Random Forest.

Tutto il progetto è stato sviluppato con Ubuntu 20.04.

## Set-up dell'ambiente di sviluppo
Prima di installare PySpark bisogna verificare di soddisfare il seguente prerequisito. Spark è scritto in Scala Programming Language e funziona in ambiente Java Virtual Machine (JVM). Ecco perché bisogna verificare di aver installato un Java Development Kit (JDK). E' importante avere una versione 8 o superiore, in questo progetto si è utilizzata la versione 11.0.11.

Inoltre, è necessario aver precedentemente installato Python, in questo progetto si è utilizzato Python v. 3.8.8. 
```bash
sudo apt install -y python3-pip
```
### Installazione PySpark
E' possibile installare PySpark con l'aiuto di `pip`:
```bash
pip3 install pyspark
```
### Installazione Jupyter
Per installare Jupyter Notebook eseguire il seguente comando sul terminale:
```bash
pip3 install jupyterlab
```
## JupyterLab
Prima di tutto aprire l'ambiente di sviluppo JupyterLab con il seguente comando:
```bash
python3 -m jupyterlab
```

A questo punto è possibile scaricare i due file `.ipynb` presenti in questa repo e fare l'upload nel JupyterLab. Prima di poter eseguire i notebook è necessario effettuare il download del dataset (https://archive.ics.uci.edu/ml/machine-learning-databases/00601/) e installare le seguenti librerie.

## Installazione librerie necessarie
* **Pandas**: `pip3 install pandas`
* **Seaborn**: `pip3 install seaborn`
* **Matplotlib**: `pip3 install matplotlib`
* **Scikit-learn**: `pip3 install -U scikit-learn`
* **Imblearn**: `pip3 install -U imbalanced-learn`
* **Handy spark**: `pip3 install handyspark`
