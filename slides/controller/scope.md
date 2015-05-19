## Scope

    <input type="text" ng-model="hello"/>
    <h1>{{ hello }} world !!!</h1>

Comment est évaluée l'expression {{ hello }} ?

AngularJS va chercher un attribut nommé 'hello' dans l'objet scope, si celui-ci est trouvé alors la valeur de l'attribut
 sera affichée sinon une chaîne de caractères vide. <!-- .element: class="fragment" data-fragment-index="1" -->

Le scope est ainsi utilisé pour initialiser des valeurs ou récupérer les valeurs modifiés par un utilisateur (cf
double data binding). <!-- .element: class="fragment" data-fragment-index="2" -->
