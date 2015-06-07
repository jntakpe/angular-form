## Créer ses promesses

    angular.module('app').factory('promiseService', function ($q, $timeout) {
            return {
                roll: function () {
                    var deferred = $q.defer();
                    $timeout(function () {
                        var value = Math.floor(Math.random() * 7) + 1;
                        if (value < 7) {
                            deferred.resolve(value);
                        } else {
                            deferred.reject('The dice fell off the table');
                        }
                    }, 2000);
                    return deferred.promise;

                }
            }});
