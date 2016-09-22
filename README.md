# express-ng2-webpack #

## composition de la stack ##

Stack basé sur : 

- Angular 2;
- ExpressJS;
- Typescript; 
- Webpack.

## Éléments réalisés ##

- Partir du `Quick start` d'Angular 2 (en version 2.0.0) ;
- Remplacer systemJS par webpack ;
- Ré-écrire les scripts NPM ;
- Gérer la génération de bundle uglifié ;
- Utiliser webpack-dev-server pour le livereload ; 

## Choses à faire ##

- Ouvrir la page servi au démarrage de la commande `npm run serve` ;
- Remplacer le CSS par du Sass (intégrer le loader webpack) ;
- Ajouter ExpressJS pour le back-end (*en court*) ;
- Refactorer les sources pour séparer client et server proprement ;
- Éviter de laisser des sources à la racine du projet (tout mettre dans src) ;
- Compléter la base Angular avec le tutorial de [angular.io](angular.io) ;
- Remplacer le mock du tutoriel par un service REST servi par ExpressJS ;
- Intégrer des testes unitaires (d'abord en tant que commande indépendante puis les lancé avant le démarrage de l'application) ;
- Ajouter ESLint ;

## Problème courrant

### Proxy

1. Lorsque l'on est derrière un proxy, il faut penser à mettre à jour son utilitaire git et npm
2. ajouter le fichier .typingsrc avec la definition du proxy `proxy="http://nomDomaine:port` ou `proxy="http://login:mdp@nomDomaine:port`