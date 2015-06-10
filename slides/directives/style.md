## Directives de style -
## style

Permet d'ajouter dynamiquement un style sur un élément sous la forme clé/valeur :

     $scope.style = { color: 'red' };
     <div>{{ style }}</div>
     <label>Style color </label><input type="text" ng-model="style.color"/>
     <div ng-style="style">I've got some style</div>

