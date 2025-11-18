# ISTRUZIONI PER L'INSTALLAZIONE DEL PROGRAMMA <alimenti.py>
~$ cd Scaricati/
~/Scaricati$ file ALIMENTI.tar.gz 
ALIMENTI.tar.gz: gzip compressed data, from Unix, original size modulo 2^32 102400
# ATTENZIONE! La seconda riga riporta l'output del comando
~/Scaricati$ tar -xvzf ALIMENTI.tar.gz 
ALIMENTI/
ALIMENTI/Leguminosa.py
ALIMENTI/Foraggio.py
ALIMENTI/Sottoprodotto.py
ALIMENTI/Farina_di_estrazione.py
ALIMENTI/Fonte_di_fibra.py
ALIMENTI/Cereale.py
ALIMENTI/importa_fieno_prato_stabile_primo_taglio.py
ALIMENTI/alimenti.py
# come sopra: il comando si trova nella prima riga (dopo il simbolo del dollaro, CHE NON DEVE ESSERE INSERITO)
~/Scaricati$ cd ALIMENTI/
~/Scaricati/ALIMENTI$ pwd
/home/piero/Scaricati/ALIMENTI
# l'output del comando <pwd> è il nome della directory in cui ci troviamo
~/Scaricati/ALIMENTI$ python3 alimenti.py
# per eseguire il programma <alimenti.py>




# DAIRY_COWS

BENVENUTO NEL PROGRAMMA PyR!

PyR (Programma Razione Python) è un programma informatico per la formulazione della razione alimentare delle bovine da latte, destinato ai Tecnici Agrari, agli Agronomi ed ai Veterinari che operano nel settore.
Per la sua semplicità d'uso, PyR può rappresentare uno strumento utile per tutti gli allevatori che desiderino assumere il pieno controllo della razione alimentare da somministrare alle proprie bovine, senza doversi avvalere necessariamente della consulenza di un professionista.


DESCRIZIONE

PyR è un software scritto da Piero Rivoira nel linguaggio python3 (https://www.python3.it/). Il calcolo dei fabbisogni nutritivi degli animali si basa sul sistema <_CNCPS_> (Cornell Net Carbohydrate and Protein System), sviluppato dalla Cornell University. Per bilanciare la razione in funzione dei fabbisogni PyR applica un algoritmo molto efficiente (di tipo accetta-rifiuta) il quale, costruendo una catena di Markov (https://it.wikipedia.org/wiki/Catena_di_Markov_Monte_Carlo) che ha come distribuzione stazionaria il vettore dei fabbisogni, calcola la quantità in cui ogni singolo alimento, scelto dall'utente, concorre a formare la razione finale.
Per valorizzare le produzioni aziendali l'utente ha, inoltre, la possibilità di scegliere la quantità di insilato (o di pastone) e/o di granella di mais che desidera inserire nella razione.


REQUISITI DI SISTEMA

GNU/Linux (Ubuntu 22.04 o superiore)

ISTRUZIONI PER L'INSTALLAZIONE

$ cd Scaricati

$ tar -xvzf PYR_LINUX_1.0.tar.gz

$ sudo apt install python3-mysql.connector python3-reportlab python3-tk python3-pil.imagetk python3-matplotlib python3-pandas vlc

PER LANCIARE IL PROGRAMMA

$ cd

$ cp -r Scaricati/PYR ~

$ cd ~/PYR/LINUX

$ python3 programmarazione__ubuntu_23.xx.py
