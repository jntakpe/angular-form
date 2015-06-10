## Similitudes

Etat :

    $stateProvider.state('contact.detail', {
        url: '/contacts/:id',
        templateUrl: 'contacts.html',
        controller: 'ContactsCtrl as contacts',
        resolve: {...}
    });


Route :


    $routeProvider.when('/contacts/:id', {
        templateUrl: 'contacts.html',
        controller: 'ContactsCtrl as contacts',
        resolve: {...}
    });
