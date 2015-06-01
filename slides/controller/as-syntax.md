## Controller as syntax

* Plus de proche de la logique objet JavaScript
* Fournit la notation avec un '.' directement
* Permet de nommer explicitement dans les vues le contrôleur contenant une variable ou fonction

`Attention à l'utilisation de this`

HTML

        <div ng-controller="CustomerCtrl as customer">
            {{ customer.name }}
        </div>

JS

        function CustomerCtrl() {
            var vm = this;
            vm.name = {};
        }


