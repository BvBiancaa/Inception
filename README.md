# 42 Inception

<h3> Italiano 🇮🇹</h3>
Questo progetto ha l'obiettivo di ampliare le competenze nell'amministrazione di sistema attraverso l'utilizzo di Docker.

Inception richiede di creare un'infrastruttura virtuale composta da diversi servizi, ciascuno eseguito all'interno di un container Docker separato.
È vietato utilizzare immagini Docker già pronte o servizi come DockerHub, è quindi necessario costruire le immagini Docker.
Deve essere presente un Makefile che chiama il docker-compose.yml che, a sua volta, fa riferimento e costruisce i Dockerfile di ciascun servizio.

La parte base del progetto comprende la configurazione di tre servizi principali: NGINX con supporto solo a TLSv1.2 o TLSv1.3, WordPress con php-fpm (senza nginx) e MariaDB. 
È inoltre richiesto di creare volumi separati per il database di WordPress e i file del sito web.

La parte bonus offre la possibilità di configurare Redis Cache per il sito web di WordPress, creare un server FTP per accedere ai file del sito, configurare Adminer per la gestione del database e configurare un servizio aggiuntivo, io ho scelto vsftpd e ho settato uno snake sul sito.

Le competenze acquisite una volta completato il progetto includono:

- Conoscenza avanzata di Docker e delle sue funzionalità per la virtualizzazione di immagini e container.
- Capacità di creare immagini personalizzate usando i Dockerfile e di costruirle utilizzando docker-compose.
- Comprensione dei concetti di orchestrazione dei container e creazione di un'infrastruttura di servizi Docker.
- Abilità nell'utilizzo di Docker per creare e gestire container per NGINX, WordPress, php-fpm e MariaDB.
- Esperienza nell'uso di volumi Docker per memorizzare e gestire i dati del database di WordPress e i file del sito web.
- Conoscenza della configurazione di reti Docker per stabilire la connessione tra i container.
- Competenza nella gestione del ripristino automatico dei container in caso di arresto anomalo.
- Abilità nel configurare il server NGINX con supporto per il protocollo TLSv1.2 o TLSv1.3.
- Conoscenza nell'implementazione di un dominio personalizzato per puntare all'indirizzo IP locale.
- Capacità di gestire variabili d'ambiente tramite file .env e l'utilizzo delle stesse all'interno dei Dockerfiles.
- Conoscenza delle pratiche di sicurezza per evitare la presenza di password nei Dockerfiles e proteggere le credenziali sensibili.
- Abilità nel configurare servizi aggiuntivi come Redis, un server FTP, un sito web statico e Adminer (un tool di gestione del database).

-------------------

<h3> English 🇬🇧</h3>
This project aims to broaden your knowledge of system administration by using Docker.

Inception requires creating a virtual infrastructure composed of different services, each running inside a separate Docker container.
Using pre-built Docker images or services like DockerHub is forbidden, so Docker images must be built from scratch.
A Makefile must be present that calls the docker-compose.yml, which in turn references and builds the Dockerfiles for each service.

The mandatory part of the project involves configuring three main services: NGINX with support for only TLSv1.2 or TLSv1.3, WordPress with php-fpm (without nginx), and MariaDB.
Separate volumes need to be created for the WordPress database and website files.

The bonus part offers the opportunity to configure Redis Cache for the WordPress website, create an FTP server to access the site's files, set up Adminer for database management, and configure an additional service. I chose vsftpd and set up a Snake game on the website.

The skills acquired upon completing the project include:

- Advanced knowledge of Docker and its features for image and container virtualization.
- Ability to create custom images using Dockerfiles and build them using docker-compose.
- Understanding of container orchestration concepts and creating a Docker service infrastructure.
- Proficiency in using Docker to create and manage containers for NGINX, WordPress, php-fpm, and MariaDB.
- Experience with Docker volumes to store and manage WordPress database data and website files.
- Knowledge of Docker networking to establish connections between containers.
- Competence in automatically restarting containers in case of abnormal termination.
- Ability to configure the NGINX server with TLSv1.2 or TLSv1.3 protocol support.
- Understanding of implementing a custom domain to point to the local IP address.
- Skill in managing environment variables using .env files and utilizing them within Dockerfiles.
- Knowledge of security practices to avoid storing passwords in Dockerfiles and protect sensitive credentials.
- Proficiency in configuring additional services like Redis, an FTP server, a static website, and Adminer (a database management tool).
