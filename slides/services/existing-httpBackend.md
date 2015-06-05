## Services disponibles -
##$httpBackend

Service de bas niveau utilisé par $http et $resource pour faire les requêtes.
Ce service est très rarement utilisé directement par les développeurs excepté pour les tests.


        it('should get 2 users when list is called', function () {
            $httpBackend.exceptGET('http://localhost:8080/myapp/users').respond([joss, sophie]);
            scope.list();
            $httpBackend.flush();
            except(scope.users.length).toBe(2);
        });
