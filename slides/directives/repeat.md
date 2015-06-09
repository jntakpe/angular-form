## Directives de template -
## repeat

Permet de parcourir un tableau

    <li ng-repeat="todo in todos>

Chaque élément aura son propre scope exposant les propriétés :

* $index : position dans l'itérateur
* $first : vrai s'il s'agit du premier élément
* $last : vrai s'il s'agit du dernier
* $middle : s'il s'agit ni du premier ni dernier élément
* $even/$odd : vrai si l'élément est pair/impair

