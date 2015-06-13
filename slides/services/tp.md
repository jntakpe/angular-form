## TP services

    git reset --hard HEAD
    git pull
    git checkout start-tp-service
    java -jar target/fra.jar --spring.profiles.active=dev

Sur la vue request :

* Récupérer les données depuis le backend en utilisant un service
* Afficher les données dans la table HTML

Sur la vue endpoints :

* Récupérer les données depuis le backend en utilisant un service
* Afficher les données dans la table HTML
* Créer les liens vers la vue 'endpoints.edit'
* Implémenter la méthode de suppression d'un endpoint
* Facultatif : afficher le JSON 'content' dans une popup en utilisant ui.bootstrap
