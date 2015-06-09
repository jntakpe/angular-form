## Promise

Les promesses sont utilisées par AngularJS pour gérer les traitements asynchrones, elles permettent la composition
 contrairement aux callback et ainsi éviter le Callback Hell.

Une promesse peut avoir deux résultats :

* fulfilled en cas d'appel avec succès
* rejected en cas d'erreur

avec deux états :

* pending en attente de résultat
* settled lorsque le résultat a été renvoyé

On dit que les promesses sont des objets 'thenable'
