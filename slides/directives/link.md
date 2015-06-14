## Créer ses directives -
## link

Permet de manipuler le DOM à la façon de jQuery.

    app.directive('myDir', function() {
           return {
             link: function(scope, element, attributes) {
                scope.turnRed = function (){
                    scope.color = { color: 'red'};
                }
             },
             template: '<h1 ng-click="turnRed({{color}})" ng-class="">Some title</h1>'
           };
    });
