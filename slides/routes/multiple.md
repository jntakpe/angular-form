## Vues multiples

Plusieurs vues peuvent être activées sur un même template.

    <!-- index.html -->
    <body>
      <div ui-view="filters"></div>
      <div ui-view="tabledata"></div>
      <div ui-view="graph"></div>
    </body>

_

    $stateProvider
      .state('report',{
        views: {
          'filters': {
            templateUrl: 'report-filters.html',
            controller: function($scope){ ... }
          },
          'tabledata': {
            templateUrl: 'report-table.html',
            controller: function($scope){ ... }
          },
          'graph': {
            templateUrl: 'report-graph.html',
            controller: function($scope){ ... }
          }
        }
      })
