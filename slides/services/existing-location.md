## Services disponibles -
##$location

Permet de maninupuler l'url de la page.

Une url AngularJS est constituée de 6 parties, par exemple pour 'http://localhost:8080/docs/training?subject=angular#service' :

* protocol = http
* host = localhost
* port = 8080
* path = /docs/training
* search = subject=angular
* hash = service

Par exemple, on peut modifier le path en écrivant:

        $location.path('/docs/exercise')
