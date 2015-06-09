## Directives de template - CSS

En plus des attributs spécifiques Angular, les attributs min, max et type email et url sont aussi gérés.

AngularJS ajoute une classe CSS pour décrire les différents état du système.

Par exemple pour un input de type number :

        <input type="number" name="age" ng-model="age" placeholder="012"
        min="18" max="130">

        input.ng-dirty.ng-invalid.ng-invalid-min { border: 6px solid red; }
        input.ng-dirty.ng-invalid.ng-invalid-max { border: 6px solid orange; }
        input.ng-dirty.ng-valid { border: 6px solid green; }
