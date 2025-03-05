 Documentation du Projet
 
 1. Installer les dépendances
Utilisez Composer pour installer les dépendances du projet :

```bash
composer install
```

2. Configurer la base de données

Dans le fichier `.env`, configurez la variable `DATABASE_URL` comme suit :

```
DATABASE_URL="mysql://root:@127.0.0.1:3306/TodoApp?serverVersion=8.0"
```

3. Créer et configurer la base de données

Exécutez les commandes suivantes pour configurer la base de données :

```bash
php bin/console doctrine:database:create
php bin/console make:migration
php bin/console doctrine:migrations:migrate
```

4. Démarrer le serveur local

Démarrez le serveur local Symfony avec la commande suivante :

```bash
symfony server:start
```






