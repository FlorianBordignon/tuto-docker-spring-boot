# French (English below)
# Docker Spring Boot and MySQL base project

## Lancer les services première fois (build app jamais fait)

Exécutez la commande suivante (l'opération est longue.) :

```bash

docker-compose up

```

Docker va télécharger les images de MySql et PhpMyAdmin et va télécharger toutes les dépendances de votre projet (pom.xml) puis va build le projet.

Vous pouvez exécuter le service en arrière-plan :

```bash

docker-compose up -d

```

Pour avoir les logs si vous exécutez en arrière-plan

Faites la commande suivante :

```bash

docker logs <nom_service>

```

Pour lancer qu'un service :

```bash

docker-compose up (-d) <nom_du_service>

```

### Après le premier lancement voir la partie mise à jour

## Arrêter le system

Arrêt de tous les services :

```bash

docker-compose down

```

Arrêter un service en particulier :

```bash

docker-compose rm -s -v <nom_service>

```

## Mise à jour du service App (après le premier lancement)

Pour mettre à jour le service sans supprimer les images manuellement

Faire la commande suivante :

```bash

docker-compose up --build -d <nom_service>

```

# English
# Docker Spring Boot and MySQL base project

## Run the services the first time (build app never done)

Run the following command (it takes a long time):

```bash

docker-compose up

```

Docker will download the images of MySql and PhpMyAdmin and will download all the dependencies of your project (pom.xml) then will build the project.

You can run the service in the background:

```bash

docker-compose up -d

```

To get the logs if you run in background

Do the following command:

```bash

docker logs <service_name>

```

To start only one service:

```bash

docker-compose up (-d) <service_name>

```

### After the first launch see the update part

## Stop the system

Stop all services :

```bash

docker-compose down

```

Stop a particular service:

```bash

docker-compose rm -s -v <service_name>

```

## Updating the App service (after the first launch)

To update the service without deleting the images manually

Do the following command:

```bash

docker-compose up --build -d <service_name>

```







