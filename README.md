# microbash
Lo scopo di questo laboratorio e' implementare, testandola adeguatamente, una piccola shell che chiameremo µbash, per prendere familiarit`a con le system call POSIX di base per la gestione dei processi.
## Pacchetti da installare
+ libreadline-dev
## Comandi da fare
+ [x] cd
+ [x] variabili d'ambiente (non possiamo crearle ma possiamo leggerle)
+ [x] standard input
+ [x] standard output
+ [x] ls
+ [x] cat
## Gestione della memoria
+ address sanitizer
+ valgrind
## Comando di DEBUG
gcc -fsanitize=address -std=gnu11 -ggdb microbash.c -o microbash
