# Template Projet Symfony

Ceci est un template tout prêt de projet Symfony - Docker

## Pré-requis

### Docker

Vous aurez besoin de :

* Docker Desktop (Pour windows)
* Docker Compose

### Application

* PHP 8.2
* Symfony CLI
* NodeJS

## Installation

Tout d'abord dans un terminal:

Démarrez les conteneurs docker avec la commande suivante :

```bash
docker-compose up -d
```

Installez les dépendances requises :

```bash
composer install # Permet d'installer les dépendances de composer
npm install # Permet d'installer les dépendances de nodejs
```

Ensuite, lancez le serveur web de symfony avec cette commande :

```bash
symfony serve -d
```

Il faudra pas oublier de changer dans les .env le serveur de la base de données et
mettre votre adresse ip :

`DATABASE_URL="mysql://!DB_USER!:!DB_PASSWORD!@!IP_ADRESS!:3306/!DB_NAME!?serverVersion=10.11.2-MariaDB&charset=utf8mb4"`

Vous pouvez vous rendre sur votre application en [cliquant ici](https://localhost:8000).

Et vous rendre sur PhpMyAdmin en [cliquant ici](http://localhost:8080).

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.