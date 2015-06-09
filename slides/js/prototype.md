## Prototype

Manière de faire de l'héritage en JS (très puissant mais compliqué).

Pour récupérer une valeur :

* on cherche pas l'objet courant
* puis dans son prototype
* puis dans le prototype du prototype
* ... jusqu'à Object.prototype


``` Pas toujours vrai pour setter une valeur```

Pour créer un objet avec un prototype :

    var obj = Object.prototype(base);
    console.log(this.baseFct()); //execute function called baseFct
