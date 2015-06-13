## Créer ses directives -
## transclude

Permet de garder le contenu d'un élément

    <myDir>This text wont be removed</myDir>

    app.directive('myDir', function() {
           return {
             transclude: true,
             template: '<h1><div ng-transclude></div> Some title</h1>'
           };
    });

donnera

    <h1><div>This text will not be removed</div> Some title</h1>


