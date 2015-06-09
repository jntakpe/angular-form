## Directives de framework - ngApp

Cette directive permet de déclarer une application AngularJS.

Il ne peut y avoir qu'un ngApp par application. Les ng-app ne peuvent pas s'imbriquer.

Plusieurs syntaxes sont possibles :

* ng-app
* ngApp
* data-ng-app

Il est possible d'avoir plusieurs application sur la même page, dans ce cas il faudra manuellement bootstraper les
autres applications en utilisant : angular.bootstrap()
