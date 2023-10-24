# Projet Docker Stack : Strapi, MongoDB et MongoExpress

Ce référentiel GitHub contient les fichiers Docker Compose nécessaires pour déployer un environnement de développement complet basé sur Docker, comprenant Strapi, MongoDB et MongoExpress.

#### Prérequis :

- Docker doit être installé sur votre système.
- Docker Compose doit également être installé.

### Configuration

Clonez ce référentiel sur votre machine locale.

```bash
git clone https://github.com/winvdaking/stack-docker.git
```

Accédez au répertoire du projet.

```bash
cd stack-docker
```

Créez un fichier .env à partir du modèle fourni (env.example) et configurez les variables d'environnement selon vos besoins.

```bash
cp env.example .env
```

Mettez à jour les valeurs dans le fichier .env pour correspondre à votre configuration.

### Utilisation

Démarrez le stack Docker en utilisant Docker Compose.

```bash
docker-compose up -d
```

Une fois que les conteneurs sont en cours d'exécution, vous pouvez accéder aux services suivants depuis votre navigateur :
- Strapi: http://localhost:1337
- MongoDB (utilisé par Strapi) : mongodb://localhost:27017
- MongoExpress: http://localhost:8082

### Maintenance

Pour arrêter le stack Docker, utilisez la commande suivante :

```bash
docker-compose down
```

Pour afficher les journaux des conteneurs, utilisez la commande suivante :


```bash
docker-compose logs
```
### Personnalisation

Ce projet est livré avec une configuration par défaut. Vous pouvez personnaliser davantage le fichier docker-compose.yml et le fichier .env en fonction de vos besoins spécifiques.
Licence

Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus d'informations.

---
[@Dorian](https://www.github.com/winvdaking)
