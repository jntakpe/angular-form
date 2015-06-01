## Injection de dépendances - fonctionnement

Par exemple pour utiliser le service $http, on peut écrire :

    angular.module('myModule').controller('MyCtrl', function ($scope, $http) {});

Ca marche aussi en inversant l'ordre des paramètres.

Si on change le nom des paramètres, Angular lance une erreur :

    angular.module('myModule').controller('MyCtrl', function ($scope, httpService) {});

Pour créer un contrôleur Angular :

* va reconnaître les paramètres de la fonction (en appelant toString() sur le contrôleur)
* puis récupérer les objets auprès de *providers* (ici $httpProvider)
* ensuite appeler le contrôleur avec les objets récupérés
