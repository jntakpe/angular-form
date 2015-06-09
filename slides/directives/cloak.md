## Directives de style - cloak

Comme ngBind permet d'éviter le flickering. S'applique sur une balise html qui sera uniquement affichée lorsque que le
template sera compilé.

    <div ng-cloak>Hello {{ world }}</div>
