# `Étape 7` - On veut tout effacer

## Ce qu'on veut faire :

- Au clic sur le bouton « Je n'aime pas la guerre » :
  - On veut effacer le contenu de la liste
  - On veut appeller chaque instance de nos personnages et s'assurer qu'ils ne soient plus actifs
  - On veut minimiser chaque carte des généraux

## Classe Army

1. Dans init, sous `btnValidate` :

   - Créez une variable `btnClear` qui sélectionne l'élément avec `.js-clear`
   - Ajouter un `click` sur la variable précédente qui appelle la méthode clearSelection();
   - _N'oubliez pas le bind_

Nous avons besoin d'effacer le contenu de la liste (ul) qui pourrait contenir des généraux. Comme nous devons accéder au `ul` dans une autre méthode que celle où elle a été créé en local, nous allons la passer en globale, dans le constructeur.

2. Dans la méthode `clearSelection` que vous allez créer :

   - ajoutez un console log `#5 - clearSelection`
   - Prenez la ligne où la variable `list` est créée dans `setSelection`, déplacez la dans le constructeur avant le `this.init` et transformez la en global.
   - Dans la méthode `setSelection`, ajoutez le `this.` devant tous les endroits où vous utilisez la variable (indice:  3 endroits)
   - Assurez-vous que le contenu HTML de cette liste soit vide (Pensez string vide)
   - Testez. La liste devrait se vider et vous devez voir le console.log passer

1. Toujours dans `clearSelection`, on veut désélectionner les cartes et enlever la classe css `is-active` pour tout minimiser.

   - Faire une boucle dans tous les éléments de la variable globale `army`
   - Créer une variable `perso` qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i._
   - Appeller la méthode `closePerso()` qu'on va aller créer dans la classe `Perso`

### Classe Perso

1. Sous `selectPerso`, créez la méthode `closePerso`
   - Ajoutez le console.log `'#6 - Yé 6h on fârme!'`
   - Redéfinissez la valeur de `isActive` comme étant fausse
   - Sur l'`élément` :
     - Retirer la classe `is-active`
1. Testez et allez écrire au tableau le nombre de console suivi de vos initiales.

# Bravo! Vous avez complétez le lab ! 💪

### Défi supplémentaire de réusinage de code
1. Dans `Army`, on créé à deux reprises des éléments de liste afin d'y ajouter des valeurs. 3 lignes de code sont répétées à deux reprises. Vous devez créer une méthode avec paramètres, qui effectuera le même travail.



<br><br><hr>

[◀ Retourner au début](../readme.md)

<hr><br>

[◀ Retourner à l'étape précédente](f.md)
