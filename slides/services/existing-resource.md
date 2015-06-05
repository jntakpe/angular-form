## Services disponibles -
##$resource


Service possédant un niveau d'abstraction supérieur à $http, permettant de communiquer de manière transparente avec
des ressources REST en fournissant des méthodes query, save, get, remove, delete.

``` $resource provient du module externe ngResource qui doit être importé ```

        var userRes = $resource('/users/:userId', {userId: '@id'});
        userRes.query(); // récupère la liste des utilisateurs
        var firstUser = userRes.get({userId: 1}); // récupère l'utilisateur 1
        firstUser.name = 'toto'; // change le nom de l'utilisateur
        firstUser.$save(); // enregistrement de l'utilisateur
