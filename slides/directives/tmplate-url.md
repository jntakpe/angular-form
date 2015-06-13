## Créer ses directives -
## templateUrl

Il est également possible de passer :

    <myDir>This text will be removed</myDir>

    app.directive('myDir', function() {
           return {
             templateUrl: 'directives/mydir.html'
           };
    });
