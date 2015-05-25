## Déclaration de modules


        var accountModule = angular.module('myapp-account', []);
        accountModule.controller('accountCtrl', function () {});
        accountModule.service('accountService', function () {});
        var myapp = angular.module('myapp', ['myapp-account']);
