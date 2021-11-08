# ML-for-Predictive-Maintenance
Progetto di tesi, sviluppato presso l'Università degli Studi dell'Insubria, che si occupa della realizzazione di un modello di machine learning  con l'obiettivo di ottenere un  sistema di manutenzione predittiva in ambiente industriale da poter integrare all’interno del progetto di tesi magistrale di Andrea Chiericati in collaborazione con il Dottor Gianfranco Modoni, operativo presso il Consiglio Nazionale delle Ricerche (CNR) di Bari. La soluzione proposta si basa sulla realizzazione e il confronto di molteplici modelli di machine learning basati su due algoritmi: il Support Vector Machine e il Random Forest.

Tutto il progetto è stato sviluppato con Ubuntu 20.04.

## Set-up dell'ambiente di sviluppo
Prima di installare PySpark bisogna verificare di soddisfare il seguente prerequisito. Spark è scritto in Scala Programming Language e funziona in ambiente Java Virtual Machine (JVM). Ecco perché bisogna verificare di aver installato un Java Development Kit (JDK). E' importante avere una versione 8 o superiore, in questo progetto si è utilizzata la versione 11.0.11.

Procediamo con l'installazione di Python attraveerso il packet manager Anaconda.
1. Scaricare Anaconda dal seguente link: https://www.anaconda.com/products/individual#Downloads
2. Una volta scaricato, aprire il terminale nella cartella in cui è stato scaricato il file e renderlo eseguibile con il seguente comando:
```bash
sudo chmod +x Anaconda3-2021.05-Linux-x86_64.sh
```
3. Installare Anaconda con il comando:
```bash
./Anaconda3-2021.05-Linux-x86_64.sh
```
  E' necessario accettare i termini e condizioni, quindi premere invio fino a che non sarà necessario digitare `yes` nel terminale.
  Verrà chiesto se mantenere o meno il path di salvataggio di default, quindi per accettare premere invio.
  Infine, verrà chiesto “Do you wish the installer to initialize Anaconda3 by running conda init?”, quindi digitare `yes` nel terminale.
4. A questo punto l'installazione è terminata, chiudere il terminale o eseguire il seguente comando:
```bash
source ~/.bashrc
```
5. Verificare se l'installazione è andata a buon fine con il comando:
```bash
conda list
```
6. Effettuare l'aggiornamento di tutti i pacchetti con il comando:
```bash
conda update --prefix /home/annalisa/anaconda3 anaconda
```
## Installazione librerie necessarie
E' necessario installare alcune librerie utilizzate nel progetto. Per farlo scaricare il file `requirements.txt` ed eseguire il seguente comando:
```bash
pip install -r /path/requirements.txt
```

## Eseguire JupyterLab
Per aprire Jupyter Lab è sufficiente eseguire il seguente comando e si aprirà una finestra nel browser predefinito.
```bash
jupyter lab
```

A questo punto è possibile scaricare i due file `.ipynb` presenti in questa repo e fare l'upload nel JupyterLab. Prima di poter eseguire i notebook è necessario effettuare il download del dataset (https://archive.ics.uci.edu/ml/machine-learning-databases/00601/).

**Nota:** E' necessario cambiare il path di locazione del dataset nei file `.ipynb` nella seconda cella!
