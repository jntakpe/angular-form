## Directive de template -
## ngMessages

Permet d'afficher des messages en fonction de l'état d'un champ sans avoir à passer par plusieurs ng-if.

    <div ng-if="myForm.myFieldName.$dirty"
    ng-messages="myForm.myFieldName.$error">
        <div ng-message="required">The field name is required</div>
       <div ng-message="minlength">The field name is too short</div>
       <div ng-message="maxlength">The field name is too long</div>
    </div>

Les messages seront affichés par ordre de priorité. Il est également possible d'afficher plusieurs messages en ajoutant
l'attribut 'multiple'.

    <div ng-if="myForm.myFieldName.$dirty"
     ng-messages="myForm.myFieldName.$error" multiple>
