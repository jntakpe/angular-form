## Promise $http

Le service $http renvoie une promise avec en supplément deux méthodes success et error.

    $http.get('/some/uri').then(
        function(data) {
            //promise resolved
        }, function (error) {
            //promise rejected
        }
    );
