## Directives de template -
## trackBy

``` ngRepeat ne permet pas d'avoir d'éléments dupliqués dans un tableau. ```

AngularJS calcule un hash qu'il insère dans la propriété $$hashkey. Par exemple, dans le cas d'un tableau de noms,
 il est possible qu'il y ait un conflit. Dans ce cas, Angular lancera une erreur ngRepeat:dupes.

Pour éviter cette erreur, il est nécessaire de préciser la manière avec laquelle Angular doit suivre les éléments :

    <div ng-repeat="name in names track by $index">{{ name }}</div>
