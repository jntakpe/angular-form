## Resolve

Permet de résoudre des dépendances et de les injecter dans un contrôleur. Si resolve est une promesse, elle sera
résolue avant l'appel du contrôleur.

    $stateProvider.state('contact', {
        resolve: {
            username: function($http) {
                return $http.get('/current/user');
            },
            simple: function() {
                return 'coucou';
            }
        },
        controller: function ($scope, username, simple) {
            $scope.currentUser = username;
            $scope.msg = simple;
        }
    });
