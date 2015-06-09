## Directives du framework - ngStrictDi

Depuis la version 1.3, il possible de démarrer l'application en mode injection de dépendance stricte cad avec la
syntaxe :

    app.controller('MyCtrl', ["$scope", "$http", function($scope, $http) {
        // handle minification
    }]);

Si un développeur ne respecte pas cette syntaxe, le message d'erreur suivant sera affiché :

MyCtrl is not using explicit annotation and cannot be invoked in strict mode

Il est possible d'utiliser strictDI avec les plugins ng-min ou ng-annotate basés sur $inject.
