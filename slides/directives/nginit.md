## Directives framework - ngInit

Cette directive permet d'initialiser une variable dans le scope courant sans utiliser le contrôleur.

    <div ng-init="world = 'world'">Hello {{ world }}!</div>

```Cette pratique n'est pas recommandée, il est préférable d'initialiser les variables dans le contrôleur. ```
