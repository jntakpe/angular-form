## Factory

La méthode de création de service la plus fréquemment utilisée.

Une factory doit renvoyer le service à enregistrer, on utilise en général le 'revealing module pattern' :


        angular.module('mod').factory('RWService', function ($http) {
            function readUsers() {
                //Some code
            }
            function writeUsers() {
                //Some code
            }
            return {
                read: readUsers,
                write: writeUsers
            }
        });

        angular.module('mod').controller('MyCtrl', function (RWService) {
            RWService.read();
            RWService.write();
        });
