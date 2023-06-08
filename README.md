# spring

## Creazione del progetto
- con il Packaging JAR all'interno del file sarà presente anche una versione embedded del server Tomcat che permette di eseguire l'applicazione senza dover installare alcun server, con il package WAR si può deployare con un server diverso -> si può cambiare dal file pom.xml
- le Dipendenze vengono messe a disposizione da spring, sono dei microframework focalizzati su specifiche features. 
  -  Spring Boot Dev Tools: permette di non dover riavviare l'applicazione ogni qualvolta andiamo ad effetturare una modifica al codice
  -  Spring Web: permette di gestire il pattern MVC e soprattutto permette di creare delle API RESTful
  -  Sono presenti dependencies per la sicurezza o i driver per interfacciarsi con i database, per il testing, per il cloud

Dal sito https://start.spring.io/:

<img width="1382" alt="Screenshot 2023-06-08 alle 09 54 34" src="https://github.com/martasichinolfi/spring/assets/101711376/6d586f5c-7952-4112-a5e6-565672ec9dcf">

Premendo su GENERATE viene creata la cartella con il progetto spring

## Packages e file
- La struttura del progetto è quella di progetto MAVEN:
  - Package __java/com/task6/editor__ che contiene la classe EditorApplication.java. Questa classe è l'entry point dell'applicazione ed è annotata con @SpringBootApplication, questo fa capire a SpringBoot di che tipo di classe si tratta e come deve essere gestita
  - Package __test/java/com/task6/editor__: package dedicato ai test
  - All'interno degli altri sorgenti troviamo il file ##application.properties## (in resources) che verrà  utilizzato per inserire tutte le impostazioni del progetto, come ad esempio la modifica del numero di porta associato all'applicazione a tutte le impostazioni relative alla sicurezza, connessione database, ecc
  - È presente il file __pom.xml__ che ci permette di gestire tutte le versioni delle varie dipendenze, nel nostro caso sono presenti: spring-boot-starter-web, spring-boot-devtools, spring-boot-starter-test, spring-boot-maven-plugin. Esso contiene la versione di SpringBoot utilizzata, i dati relativi al groupId, all'artifact, la versione (che può essere modificata). Questo file pom può essere modificato manualemente se vogliamo aggiungere altre dipendenze o plugin o modificare parametri.

## RUN
Per lanciare il progetto su VSCode, 
- scaricare la seguente estensione: https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-spring-boot-dashboard
- aprire la dashboard dal VSCode e fare run 
<img width="1381" alt="Screenshot 2023-06-08 alle 10 29 01" src="https://github.com/martasichinolfi/spring/assets/101711376/b4d09031-0dec-4aee-b947-62d07d35019b">

A questo punto la 
