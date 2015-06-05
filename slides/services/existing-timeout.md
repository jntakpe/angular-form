## Services disponnibles -
##$timeout et $interval

$timeout permet de différer l'exécution d'une action en respectant le cycle de vie des objets AngularJS.

        var delayed = $timeout(function(){//mon action}, 1OOO);

$interval permet d'exécution toutes les X secondes une action en respectant le cycle de vie des objets AngularJS.

        var interval = $interval(function(){//mon action}, 1000, 0);
