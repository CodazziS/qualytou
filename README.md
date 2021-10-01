# Assurance-maladie-digital Qualytou

Fournit des outils d'analyse statique pour PHP utilisé dans les projets de 
la CNAM.

## Démarrage

La manière la plus simple d'utiliser Qualytou est via Composer.

```sh
composer require --dev assurance-maladie/qualytou
```

Une fois Qualytou installé, les fichiers de configurations sont automatiquement 
installés à la racine dans votre projet pour indiquer aux outils comment 
analyser votre code source.  
Une fois configuré, vous pouvez le lancer via `php vendor/bin/grumphp run`.

Qualytou 1 dépend de PHP 7.3+.

## Fonctionnalités

Qualytou est capable d'effectuer les types d'analyse suivants :

* [PHP Coding Standards Fixer (PHP CS Fixer)](https://cs.symfony.com/)
* [PHPMD - PHP Mess Detector](https://phpmd.org/)
* [PHPStan - PHP Static Analysis Tool](https://phpstan.org/)
* [Psalm](https://psalm.dev/)

## Utilisation

Après avoir [installé Qualytou](#demarrage), Qualytou a configuré 
automatiquement les fichiers des outils.  
Il est donc possible de personnaliser chaque fichier de configuration.

Cette commande `php vendor/bin/grumphp run` execute donc tous les outils en 
parallèle, mais uniquement pour les modifications qui seront validées.
