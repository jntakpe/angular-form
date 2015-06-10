## AutoBoxing

```Les primitifs sont convertis à la volée si c'est nécessaire```

    var n=5;
    n.toString();

    var s='hello';
    s.length;

``` Evitez de créer (comme en Java) des objets Boolean, Number et String ```

    var a = new String('a');
    a == 'a'; //true
    a === 'a'; //false

```Préférez la comparaison stricte (===) ```
