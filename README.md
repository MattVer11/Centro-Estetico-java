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


