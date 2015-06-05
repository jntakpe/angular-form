## Service

Pour la création de service au sens AngularJS du terme, le constructeur sera appelé :

        angular.module('mod').service('RWService', function ($http) {

            this.read = function readUsers() {
                //Some code
            };

            this.write = function writeUsers() {
                //Some code
            };
        });

        angular.module('mod').controller('MyCtrl', function (RWService) {
            RWService.read();
            RWService.write();
        });
