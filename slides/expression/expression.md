## Expressions

Angular interprète les templates, ce qui permet d'écrire du HTML contenant des expressions dynamiques (!= eval()).

    <h1>{{ 1+1 }}</h1> // 2
    <h1>{{ "Hello " + "world !!!" }}</h1> // Hello world

*Pour respecter la séparation du code entre les vues et les contrôlleurs, il est nécessaire de garder les expressions
 simples.*
