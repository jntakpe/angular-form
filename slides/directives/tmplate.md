## Créer ses directives -
## template

Template permet de remplacer la directive par le contenu de la propriété template :

    <div myDir>This text will be removed</div>

    app.directive('myDir', function() {
           return {
             template: '<h1>Some title</h1>'
           };
    });
