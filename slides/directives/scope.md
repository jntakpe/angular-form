## Créer ses directives -
## scope

Précédemment les directives héritait du scope englobant.

Pour faire des composants réutilisables, il est possible de les isoler du scope.

        app.directive('myDir', function() {
               return {
                 scope: {},
                 template: '<h1>{{color}} Wont work</h1>'
               };
        });
