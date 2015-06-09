## Directive de template -
## ngModel

Indique à AngularJS que toute modification de ce champ doit être répercutée sur le modèle.

Le travail est fait par un contrôleur lié à la directive (ngModelController). Ce contrôleur gérera la validatation du
champ et expose les méthodes :

* $pristine : permet de savoir si le champ n'a pas été touché
* $dirty : inverse de $pristine
* $valid : savoir si le champ est valide
* $invalid : savoir si le champ est invalide
* $error : map contenant les erreurs
* $untouched : si le champ n'a pas perdu le focus
* $touched : si le champ a perdu le focus
