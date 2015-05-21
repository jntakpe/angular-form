## Filtres personnalisés

* Déclaration au niveau du module en utilisant le mot clé 'filter'

* Une fonction de filtrage renvoie une autre fonction qui prend en paramètre l'élément à filtrer

            angular
                    .module('filterapp', [])
                    .controller('FilterCtrl', function ($scope) {
                        $scope.name = "";
                    })
                    .filter('reverse', function () {
                        return function (text) {
                            return text.split("").reverse().join("");
                        };
                    });

