## Configuration des services

Un service peut posséder un bloc config et run.

Le bloc config est exécuter pendant la phase d'enregistrement du service et peut agir sur le provider correspondant.

    angular.module('mod').config(function ($interpolateProvider) {
        $interpolateProvider.startSymbol = '[[';
        $interpolateProvider.endSymbol = ']]';
    });

Le bloc run permet d'agir sur le service une fois le provider enregistré et configuré.

    angular.module('mod').run(function($http) {
        $http.defaults.headers.common.Authorization = 'Basic YmVlcDpib29w'
    });
