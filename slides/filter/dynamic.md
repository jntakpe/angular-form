## Filtrage dynamique

* Agit sur un tableau pour en retourner un sous-ensemble
* Retient tout élément du tableau ayant une propriété contenant la chaîne de caractères recherchée

        <input type="text" ng-model="mysearch"/>
        <tr ng-repeat="person in persons | filter:mysearch">

Ou sur un propriété spécifique :

        <input type="text" ng-model="mysearch.name"/>
        <tr ng-repeat="person in persons | filter:mysearch">
