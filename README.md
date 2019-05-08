# Black Widow
![image](https://www.relativeuniverse.net/black-widow.jpeg)

## CTF Tool (Language: [python3.7](https://www.python.org/downloads/))

#### Dipendenze:
 - [pyshark](https://pypi.org/project/pyshark/): `pip3 install pyshark`
 - [PyQt5](https://pypi.org/project/PyQt5/): `pip3 install PyQt5`

#### Funzionalità:
 - Sniffing (anche con regex sul contenuto delle richieste/risposte) per rubare flag catturate da altri;
 - Invio automatico di flag al gaming server;
 - Invio stessa richiesta a terminali multipli (per sfruttare contemporaneamente le stesse vulnerabilità di più server);
 - Storico mappa {server -> vulnerabilità} sfruttate (condiviso) per evitare ripetizione attacchi già andati a buon fine;
 - Cluster per evitare di effettuare stessi attacchi contemporaneamente;
 - Il tool di ogni macchina comunicherà in modo criptato e autenticato (RSA) con gli altri tool nella rete;

Suggerite voi altre funzionalità (comunque ci verranno in mente con l'esperienza sulle CTF).

#### Directories:
```
  /app      # Package principale dell'applicazione
    |
    |-- /attack/        # Package per modalità di attacco
    |-- /defense/       # Package per modalità di difesa
    |
    |-- /utils/
    |      |
    |      |-- /cluster/        # Package che fornisce metodi per condividere e ricevere info
    |      |-- /encryption/     # Package per criptare/decriptare stringhe/files
    |      |-- /exceptions/     # Contine eventuali eccezioni personalizzate
    |      |-- /helpers/        # Package contenente helpers generici usati in più parti del programma
    |      |-- /history/        # Package che fornisce classi e funzioni per salvare cronologie di vario tipo
    |      |-- /requests/       # Package che fornisce metodi per effettuare richieste (anche multiple)
    |      |-- /settings/       # Package dedito al settaggio di parametri globali (es. IP gaming server, ...)
    |      |-- /sniffing/       # Package che fornisce metodi per sniffing in una rete
    |      |-- /sql/            # Package che fornisce metodi per sql injection
    |
```


<hr/>

### [CyberChallenge.it 2019](https://www.cyberchallenge.it)
#### [© Link Campus University](https://www.unilink.it)
