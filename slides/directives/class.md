## Directives de style -
## class

Permet de modifier dynamiquement les classes CSS.

         .green { color: green;}
         .bold { font-weight: bold;}
         <input type="checkbox" ng-model="greenChecked"/>
         <input type="checkbox" ng-model="boldChecked"/>
         <div ng-class="{green: greenChecked, bold: boldChecked }">I'm classy
         </div>

Il est existe également deux directives ngClassEven et ngClassOdd pour changer de classe dans un repeat.
