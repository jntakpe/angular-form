## Directives de template - if

ngIf permet de créer un élément du DOM en fonction de la valeur d'un paramètre.

Contraire à ngHide ou ngShow, l'élément sera supprimé ou créé sur le DOM plutôt que juste caché.

    <input type="checkbox" ng-model="isVisible"/><br/>
    <div ng-if="isVisible">I'm gonna disappear</div>
