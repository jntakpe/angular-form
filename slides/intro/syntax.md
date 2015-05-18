## Syntaxe

Déclarative (HTML) pour la construction de l'interface

    <table ng-controller="StatsController">
        <tr ng-repeat="stat in stats">
            <td>{{stat.class}}</td>
        </tr>
    </table>

Impérative (JS) pour la logique de l'application

    myApp.controller('StatsController', function ($scope, application, StatsService) {
        StatsService.findAll(application.id)
        .success(function (data) { $scope.stats = data; })
        .error(function(data, status) { //Some error handling code });
    });
