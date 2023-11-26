### Esempi di Linee Corrette:

1. **Cambio della Directory di Lavoro con Padroneggiamento:**
   - **Linea:** `cd /path/valido/foo`
   - **Scopo:** Cambiare la directory di lavoro a una posizione specifica.
   - **Risultato Atteso:** Cambio della directory di lavoro a "/path/valido/foo".

2. **Filtraggio e Redirezione Output con Pipe Multiplo:**
   - **Linea:** `ls -l | grep bar >risultato.txt`
   - **Scopo:** Applicare più filtri consecutivi all'elenco dei file e salvare il risultato in un file.
   - **Risultato Atteso:** Creazione di "risultato.txt" contenente il risultato filtrato.

3. **Conteggio delle Righe con `wc` e Redirezione dell'Output:**
   - **Linea:** `ls -l | wc -l >conteggio.txt`
   - **Scopo:** Contare il numero di righe nell'elenco dei file e salvare il risultato in un file.
   - **Risultato Atteso:** Creazione di "conteggio.txt" contenente il numero di righe.

4. **Utilizzo della Variabile d'Ambiente per `echo`:**
   - **Linea:** `echo $HOME >home.txt`
   - **Scopo:** Utilizzare la variabile d'ambiente `$HOME` per scrivere il percorso della home in un file.
   - **Risultato Atteso:** Creazione di "home.txt" contenente il percorso della home dell'utente.

5. **Utilizzo di `echo` per Scrivere un Messaggio:**
   - **Linea:** `echo "Hello World!" >hello.txt`
   - **Scopo:** Utilizzare il comando `echo` per scrivere un messaggio in un file.
   - **Risultato Atteso:** Creazione di "hello.txt" contenente il messaggio "Hello World!".

6. **Utilizzo di `echo` per Scrivere un Messaggio con Variabile d'Ambiente:**
   - **Linea:** `echo "Hello $USER!"`
   - **Scopo:** Utilizzare il comando `echo` per scrivere un messaggio su terminale, utilizzando la variabile d'ambiente `$USER`.
   - **Risultato Atteso:** Messaggio su terminale: "Hello <nome_utente>!".

### Esempi di Linee Errate:

1. **Errore nel Numero di Argomenti per `cd`:**
   - **Linea:** `cd /path/valido/foo bar`
   - **Scopo:** Verificare la gestione dell'errore quando il comando `cd` ha più di un argomento.
   - **Risultato Atteso:** Messaggio di errore indicante che il comando `cd` accetta solo un argomento.

2. **Errore di Redirezione in un Comando con Output Multiplo:**
   - **Linea:** `ls -l | grep foo >risultato.txt | wc -l`
   - **Scopo:** Verificare la gestione dell'errore quando si tenta di redirigere l'output di un comando con output multiplo.
   - **Risultato Atteso:** Messaggio di errore indicante che la redirezione deve essere applicata a un comando singolo (l'ultimo).

3. **Errore nel Comando Non Trovato:**
   - **Linea:** `comando_inesistente arg1 arg2`
   - **Scopo:** Verificare la gestione dell'errore quando il comando specificato non esiste.
   - **Risultato Atteso:** Messaggio di errore indicante che il comando non è stato trovato.

4. **Errore nel Comando con Argomenti Errati:**
   - **Linea:** `ls -l argomento_inesistente`
   - **Scopo:** Verificare la gestione dell'errore quando il comando specificato ha un argomento non valido.
   - **Risultato Atteso:** Messaggio di errore indicante che l'argomento non è valido.

5. **Errore nel Comando con Opzione Errata:**
   - **Linea:** `ls -z`
   - **Scopo:** Verificare la gestione dell'errore quando il comando specificato ha un'opzione non valida.
   - **Risultato Atteso:** Messaggio di errore indicante che l'opzione non è valida.

6. **Errore nel Comando di redirezione con spazio dopo <:**
   - **Linea:** `ls -l > file`
   - **Scopo:** Verificare la gestione dell'errore quando il comando di redirezione ha uno spazio dopo <:.
   - **Risultato Atteso:** Messaggio di errore indicante che il comando di redirezione non è valido.