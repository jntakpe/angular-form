## Créer ses directives -
## template

Template permet de remplacer la directive par le contenu de la propriété template :

    <myDir>This text will be removed</myDir>

    app.directive('myDir', function() {
           return {
             template: '<h1>Some title</h1>'
           };
    });
