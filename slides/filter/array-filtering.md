## Filtrage de tableaux

* limitTo : permet de filtrer un sous-ensemble

        {{ ['a', 'b', 'c'] | limitTo:2 }} // ['a', 'b']
        {{ ['a', 'b', 'c'] | limitTo:-2 }} // ['b', 'c']

* orderBy : permet de trier les éléments


Par exemple :

        var pierre = {name: 'Pierre', gender: 'male'};
        var paul = {name: 'Paul', gender: 'male'};
        var marie = {name: 'Marie', gender: 'female'};
        var julie = {name: 'Julie', gender: 'female'};
        $scope.persons = [pierre, paul, marie, julie];

Donne :

        {{ persons | orderBy: 'name'}} // Julie, Marie, Paul, Pierre
        {{ persons | orderBy: ['gender', '-name']}} // Marie, Julie, Pierre, Paul
