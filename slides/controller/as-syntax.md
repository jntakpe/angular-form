## Controller as syntax

HTML

        <div ng-controller="CustomerCtrl as customer">
            {{ customer.name }}
        </div>

JS

        function CustomerCtrl() {
            var vm = this;
            vm.name = {};
        }
