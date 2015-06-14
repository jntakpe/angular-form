## Créer ses directives -
## @ scope

Il est possible de passer des valeurs au scope isolé par chaîne de caractères.

    <myDir color="Red" />

    app.directive('myDir', function() {
       return {
         scope: {
            myColor: '@color'
         },
         template: '<h1>{{myColor}} Will work</h1>'
       };
    });
