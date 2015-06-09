## Directive de template -
## switch

Permet de remplacer un élément selon la valeur d'une expression :

    <div ng-switch="user.role">
        <span ng-switch-when="ADMIN">Administrateur</span>
        <span ng-switch-when="USER">Utilisateur</span>
        <span ng-switch-default>Anonyme</span>
    </div>
