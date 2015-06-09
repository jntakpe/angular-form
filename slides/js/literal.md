# Literal

Pour créer un objet en JavaScript :

    var emptyObj = {};
    var user = {
        name: 'joss',
        age: 28,
        adress: {
            street: 'Jean Jaurès',
            city: 'Toulouse'
        }
    };

Pour modifier une propriété :

    user.name = 'Jocelyn';
    user['age'] = 29;

Pour supprimer une propriété :

    delete user.name;
