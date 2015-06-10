## Démarrage

Ajouter le script :

    <script src="angular-ui-router.js"/>


Charger le module en tant que dépendance :

    angular.module('myApp', [’ui.router']);

Déclarer un état :

    angular.module('myApp').config(function($stateProvider) {
        $stateProvider.state('home', {
            url: '/',
            templateUrl: 'home.html'
        });
    });


