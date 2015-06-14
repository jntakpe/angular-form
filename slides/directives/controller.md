## Créer ses directives -
## controller

Il est possible d'extraire le comportement de la function link dans un contrôleur plus facile à tester unitairement.

    app.directive('myDir', function() {
           return {
             controller: myCtrl,
             template: '<h1 ng-click="turnRed({{color}})" ng-class="">Some title</h1>'
           };
    });

    function myCtrl(scope, element, attributes) {
        scope.turnRed = function (){
            scope.color = { color: 'red'};
        }
     }
