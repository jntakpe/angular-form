## Filtres natifs

* number : permet de préciser le nombre de chiffres après la virgule

        {{ 31.26 | number:1 }} // 31.3
        {{ 31.26 | number:3 }} // 31.260

* currency: permet de préciser la monnaie

        {{ 31.26 | currency:'$' }} // $31.26

* date : permet de formatter la date en passant le pattern en paramètre

        {{ today | date:'dd/MM/yyyy' }} // 21/05/2015

* lowercase/uppercase : convertit en minuscules ou majuscules

        {{ "Jocelyn" | uppercase }} // JOCELYN
        {{ "Jocelyn" | lowercase }} // jocelyn

* json : affiche l'objet au format JSON

        {{ user | json }} // { name: 'Jocelyn', company: 'Sopra Steria' }
