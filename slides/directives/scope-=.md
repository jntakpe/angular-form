## Créer ses directives -
## = scope

Il est possible de passer des valeurs au scope isolé par référence.

    <myDir color="obj" />

    app.directive('myDir', function() {
       return {
         scope: {
            obj: '=color'
         },
         template: '<h1>{{obj.color}} Will work</h1>'
       };
    });
