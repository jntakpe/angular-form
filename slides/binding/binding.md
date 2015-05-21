# Binding

Le double data-binding d'Angular permet de maintenir le modèle en accord avec la vue et vice-versa.

    <input type="text" ng-model="hello"/>
    <h1>{{ hello }} world !!!</h1>

En préférant la 'dot notation' avec l'expression évaluée dans la classe

    <input type="text" ng-model="hello.myclass"/>
    <h1 class="{{ hello.myclass }}">Hello world !!!</h1>
