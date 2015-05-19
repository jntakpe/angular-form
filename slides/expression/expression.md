# Expressions

Angular interprète les templates, ce qui permet d'écrire du HTML contenant des expressions dynamiques (!= eval()).

    <h1>{{ 1+1 }}</h1> // 2
    <h1>{{ "Hello " + "world !!!" }}</h1> // Hello world

`Les expressions pardonnent les null ou undefined (une chaîne de caractères vide sera affichée).`
