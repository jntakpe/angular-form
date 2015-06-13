## Créer ses directives -
## Restrict

Par défault la directive est restreinte à l'élément.

Il est possible de modifier ce comportement en utilisant :

* A pour attribut
* E pour élément
* C pour classe
* M pour élément

        <div myDir>This text will be removed</div>

        app.directive('myDir', function() {
           return {
             restrict: 'A',
             templateUrl: 'dirs/mydir.html'
           };
        });
