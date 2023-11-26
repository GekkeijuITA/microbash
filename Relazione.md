### Esempi di Linee Corrette:

1. **Cambio della Directory di Lavoro con Padroneggiamento:**
   - **Linea:** `cd /path/valido/foo`
   - **Scopo:** Cambiare la directory di lavoro a una posizione specifica.
   - **Risultato Atteso:** Cambio della directory di lavoro a "/path/valido/foo".

2. **Filtraggio e Redirezione Output con Pipe Multiplo:**
   - **Linea:** `ls -l | grep foo | grep bar > risultato.txt`
   - **Scopo:** Applicare più filtri consecutivi all'elenco dei file e salvare il risultato in un file.
   - **Risultato Atteso:** Creazione di "risultato.txt" contenente il risultato filtrato.

3. **Conteggio delle Righe con `wc` e Redirezione dell'Output:**
   - **Linea:** `ls -l | wc -l > conteggio.txt`
   - **Scopo:** Contare il numero di righe nell'elenco dei file e salvare il risultato in un file.
   - **Risultato Atteso:** Creazione di "conteggio.txt" contenente il numero di righe.

4. **Utilizzo della Variabile d'Ambiente per `echo`:**
   - **Linea:** `echo $HOME > home.txt`
   - **Scopo:** Utilizzare la variabile d'ambiente `$HOME` per scrivere il percorso della home in un file.
   - **Risultato Atteso:** Creazione di "home.txt" contenente il percorso della home dell'utente.

### Esempi di Linee Errate:

1. **Errore nel Numero di Argomenti per `cd`:**
   - **Linea:** `cd /path/valido/foo bar`
   - **Scopo:** Verificare la gestione dell'errore quando il comando `cd` ha più di un argomento.
   - **Risultato Atteso:** Messaggio di errore indicante che il comando `cd` accetta solo un argomento.

2. **Errore di Redirezione in un Comando con Output Multiplo:**
   - **Linea:** `ls -l | grep foo > risultato.txt | wc -l`
   - **Scopo:** Verificare la gestione dell'errore quando si tenta di redirigere l'output di un comando con output multiplo.
   - **Risultato Atteso:** Messaggio di errore indicante che la redirezione deve essere applicata a un comando singolo.

3. **Errore nella Redirezione dell'Input:**
   - **Linea:** `ls < bar -l`
   - **Scopo:** Verificare la gestione dell'errore quando la redirezione dell'input è posizionata in modo non corretto.
   - **Risultato Atteso:** Messaggio di errore indicante che la redirezione dell'input deve seguire il comando.

4. **Errore nel Comando Non Trovato:**
   - **Linea:** `comando_inesistente arg1 arg2`
   - **Scopo:** Verificare la gestione dell'errore quando il comando specificato non esiste.
   - **Risultato Atteso:** Messaggio di errore indicante che il comando non è stato trovato.