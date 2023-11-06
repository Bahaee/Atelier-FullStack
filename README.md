# README

## Application Full Stack avec Docker

Ce projet est une application Full Stack qui se compose d'un backend Spring Boot, d'un frontend React, et d'une base de données MySQL, tous conteneurisés à l'aide de Docker.

### Génération des Images Docker

1. **Backend Spring Boot :**
   - Pour générer l'image Docker pour le backend, nous avons utilisé un Dockerfile. Assurez-vous que le Dockerfile est correctement configuré pour votre application Spring Boot.
   - Exécutez la commande suivante dans le répertoire contenant le Dockerfile :
     ```bash
     cd src/main/webapp/reactjs
     docker build -t backend-voiture:1.0 .
     ```

2. **Frontend React :**
   - Pour générer l'image Docker pour le frontend React, assurez-vous que le Dockerfile est correctement configuré pour votre application React.
   - Exécutez la commande suivante dans le répertoire contenant le Dockerfile :
     ```bash
     docker build -t frontend-voiture:1.0 .
     ```

### Pull de la Base de Données MySQL

Nous utilisons une image MySQL provenant de Docker Hub. Vous pouvez la tirer en exécutant la commande suivante :

```bash
docker pull mysql
