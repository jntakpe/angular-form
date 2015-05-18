## Syntaxe

Déclarative (HTML)

    <table ng-controller="StatsController">
        <tr ng-repeat="stat in stats">
            <td>{{stat.class}}</td>
        </tr>
    </table>

Impérative (JS)

    myApp.controller('StatsController', function ($scope, application, StatsService) {
        StatsService.findAll(application.id)
        .success(function (data) { $scope.stats = data; })
        .error(function(data, status) { //Some error handling code });
    });
