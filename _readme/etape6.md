# Révision Les généraux de la TIM

## `Étape 6` - Si on ne sélectionne rien?

Il est toujours judicieux de gérer tous les cas possible, on appelle ça la programmation défensive.
On veut éviter que quelqu'un qui clique sur « Valider » ait l'impression que ça bogue.

Voici ce qu'on va faire :

- On veut créer un élément de liste qui contient un message générique et l'ajouter dans la liste pour avertir l'usager
- Comme on va créer un élément de liste pour une 2e fois, on va créer une méthode qu'on pourra appeller des 2 endroits où le code ne sera utilisé qu'une fois.

Sous la méthode setSelection :

- Créez une méthode `createListItem`
  - Cette méthode prendra 2 paramètres
    1. `parent` qui nous servira à passer la variable `list` (le ul)
    2. `name` qui nous servira à passer ce qu'on veut dans le li
  - Emmenez-y tout ce qui se trouve à l'intérieur de la condition `perso.isActive` SAUF le console.log()
    - la ligne qui créé un élément de liste reste intact
    - le contenu HTML de l'item de liste devra être égal au paramètre `name`
    - Au lieu d'ajouter un enfant dans `list`, utilisez plutôt le paramètre `parent` qui contient maintenant la référence à cette liste
  - Finalement, à l'intérieur de la boucle de `setSelection`, après le console.log()
    - Appellez la méthode createListItem en lui passant
      1. La référence à la `liste`
      2. Le `name` provenant de l'instance de `perso`
  - Testez avec des généraux sélectionnés afin de voir que votre liste est toujours fonctionnelle

Maintenant, on va utiliser cette nouvelle méthode pour indiquer l'absence de sélection :

- Juste avant la boucle dans `setSelection`
  - créez une variable modifiable `hasPerso` avec la valeur false
- À l'intérieur de la condition `perso.isActive`, redéfinissez `hasPerso` à true
- Sous la boucle :
  - Si `hasPerso` n'est pas vrai (!)
    - Appellez la méthode createListItem comme au point précédent en changent le 2e paramètre pour un message indiquant qu'il n'y a pas de sélection
- Testez! Votre message devrait apparaître sans sélection

<br><br><hr>

[Passer à l'étape 7 ▶](etape7.md)

<hr><br>

[◀ Retourner à l'étape 5](etape5.md)
