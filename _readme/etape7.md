# Révision Les généraux de la TIM

## `Étape 7` - On veut tout effacer

### Ce qu'on veut faire :

- Au clic sur le bouton « Je n'aime pas la guerre » :
  - On veut effacer le contenu de la liste
  - On veut appeller chaque instance de nos personnages et s'assurer qu'ils ne soient plus actifs
  - On veut minimiser chaque carte des généraux

### Classe Army

1. Dans init, sous `btnValidate` :

   - Créez une variable `btnClear` qui sélectionne l'élément avec `.js-clear`
   - Ajouter un `click` sur la variable précédente qui appelle la méthode clearSelection();
   - _N'oubliez pas le bind_

1. Dans la méthode `clearSelection` que vous allez créer :

   - ajoutez un console log `#5 - clearSelection`
   - une variable `list` qui sélectionne l'élément de liste qui contient `.js-final-selection` comme tantôt.
   - Assurez-vous que le contenu HTML de cette liste soit vide (Pensez string vide)
   - Testez. La liste devrait se vider et vous devez voir le console.log passer

1. Ensuite, on veut désélectionner les cartes et enlever la classe css `opened` pour tout minimiser

   - Faire une boucle dans tous les éléments de la variable `army`
   - Créer une variable `perso` qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i._
   - Appeller la méthode `closePerso()` qu'on va aller créer dans la classe `Perso`

### Classe Perso

1. Sous `selectPerso`, créez la méthode `closePerso`
   - Ajoutez le console.log `'#6 - Yé 6h on fârme!'`
   - Redéfinissez la valeur de `isActive` comme étant fausse
   - Sur l'`élément` :
     - Retirer la classe `opened`
     - Retirer la classe `selected`
1. Testez et dite à haute voix le nombre de console.log apparaissant

# Bravo! Vous avez complétez le lab ! 💪

<br><br><hr>

[◀ Retourner au début](../readme.md)

<hr><br>

[◀ Retourner à l'étape 6](etape6.md)
