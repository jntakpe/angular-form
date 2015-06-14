## Créer ses directives -
## function scope

Il est possible de passer des fonctions au scope isolé par référence.

    <myDir turn-color="turnRed()" />

    $scope.turnRed = function() {alert('Red');};

    app.directive('myDir', function() {
       return {
         scope: {
            turnColor: '&'
         },
         template: '<h1 ng-click="turnColor()">Will work</h1>'
       };
    });
