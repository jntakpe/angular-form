## Directive de template -
## Form

La directive form instancie un contrôleur FormController. Ce contrôleur est un parent des contrôleur ngModelController
 et il est possible d'accéder aux champs en utilisant le nom du champ suivi du nom du contrôleur.

Ce contrôleur expose les méthodes :

* $pristine : si l'utilisateur n'a pas touché le formulaire
* $dirty : si l'utilisateur a touché le formulaire
* $valid : si l'ensemble des champs du formulaire est valide
* $invalid : si un des champs du formulaire est invalide
* $error: représente le dictionnaire des erreurs
* $submitted : indique si le formulaire a été envoyé
