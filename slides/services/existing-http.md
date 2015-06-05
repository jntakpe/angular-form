## Services disponibles - $http

Permet de communiquer avec un serveur en abstrayant la plomberie AJAX.

Utilise l'API des promises $q.

L'API permet de déclarer un callback d'erreur et de succès.

        $http.get('monServeur', {params: {key1: value1, key2: value2}})
            .success(function(data, status, header, config) {})
            .error(function(data, status, header, config) {});


        $http.post('monServeur', {login: jOSS, password: nokidding})
                    .success(function(data, status, header, config) {})
                    .error(function(data, status, header, config) {});
