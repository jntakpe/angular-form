# Modules

* AngularJS utilise une logique modulaire pour déclarer les différents composants de l'application

* Le chargement des modules peut être fait dans n'importe quel ordre

* Les librairies externes sont souvent récupérées sous forme de module

* Permet d'avoir des fichiers séparés par responsabilité (un fichier / service, controller, module)


        var myApp = angular.module('myApp', []);

` Même si un module n'a pas de dépendance, il ne faut pas omettre les crochets`
