## Array

Pour créer un tableau :

    var tab = ['a', 1, true];
    tab[0]; // 'a'
    tab['2']; // true

``` Les tableaux sont des objets JS ```

La longueur d'un tableau JS est modifiable :

    tab.length; //3
    tab[20] = 'wtf';
    tab.length; //21
    tab.length = 2;
    tab // ['a', 1]
    tab.length = 0;
    tab // []
