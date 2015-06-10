## Hiérarchie

Permet d'imbriquer les états les uns dans les autres.

    $stateProvider
        .state('home', {...})
        .state('contacts', {...})
        .state('contacts.detail', {...})
        .state('contacts.detail.edit', {...});


Alternative :

    $stateProvider
        .state('home', {...})
        .state('contacts', {...})
        .state('details', {
            parent: 'contacts'
        });

``` Le point dénote sur relation de parent à enfant ``` <!-- .element: class="fragment" data-fragment-index="2" -->


