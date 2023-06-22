# Centro-Estetico-java
Software di un possibile Centro Estetico java
Autori : Vladyslav , Matteo , Mattia , Gregorio , Stefania , Gianni
Librerie: javax.swing , java.awt , java.
Database utilizzato MySql nome database: dbcentroestetico

Tabelle database:
Cliente 
id INT PK AUTO_INCREMENT
nome VARCHAR(50) NOT NULL
cognome VARCHAR(50) NOT NULL
email VARCHAR(50)
telefono VARCHAR(20) NOT NULL
codiceFiscale VARCHAR(16)
indirizzo VARCHAR(100)
preferenzaOperatore VARCHAR(100)
eventualiAllergie VARCHAR(100) NOT NULL

Utente 
id INT PK AUTO_INCREMENT
username VARCHAR(50) NOT NULL
password VARCHAR(50) NOT NULL
ruolo VARCHAR(100) NOT NULL

Operatore 
id INT PK AUTO_INCREMENT
nome VARCHAR(50) NOT NULL
cognome VARCHAR(50) NOT NULL
email VARCHAR(50)
telefono VARCHAR(20) NOT NULL

Appuntamento 
id INT PK AUTO_INCREMENT
data DATE NOT NULL
ora DATETIME NOT NULL
idTrattamento INT
idCliente INT
idOperatore INT

Trattamento 
id INT PK AUTO_INCREMENT
nomeTrattamento VARCHAR(50) NOT NULL
durata DOUBLE
prezzo DOUBLE NOT NULL
idOperatore INT

Pagamento 
id INT PK AUTO_INCREMENT
idCliente INT
idTrattamento INT
idProdotto INT

Stanza 
id INT PK AUTO_INCREMENT
nStanza INT NOT NULL
nomeStanza VARCHAR(50)
idTrattamento INT

Prodotto 
id INT PK AUTO_INCREMENT
nome VARCHAR(50) NOT NULL
prezzo DOUBLE NOT NULL
quantita INT NOT NULL
idTrattamento INT

Macchinario 
id INT PK AUTO_INCREMENT
nMacchinari INT NOT NULL
nomeMacchinario VARCHAR(50)
verificaMacchinario BOOLEAN
idTrattamento INT
idStanza INT

Descrizione ed uso:
Il software è utile nella gestione di un piccolo-medio centro estetico per l'ottimizzazione del tempo e la gestione degli operatori.

Moduli:
Gestione Appuntamento,
Gestione Cliente,
Gestione Macchinario,
Gestione operatore,
Gestione Prodotto,
Gestione Pagamento,
Gestione Stanza,
Gestione Trattamento,
Gestione Utente,
Menu di login

I ruoli esistenti sono 3:
1) administator
2)sectretary
3)operator

Per poter accedere la prima volta al programma è necessario avere un utente amministratore presente nella tabella utente e conoscerne le credenziali d'accesso.






