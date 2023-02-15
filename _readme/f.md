# `Étape 6` - Si on ne sélectionne rien?

Il est toujours judicieux de gérer tous les cas possible, on appelle ça la programmation défensive.
On veut éviter que quelqu'un qui clique sur « Valider » ait l'impression que ça bogue.

1. Juste _avant_ la boucle dans `setSelection` :
    - Créez une variable modifiable `hasPerso` avec la valeur `false`
- À l'intérieur de la condition `perso.isActive`, redéfinissez `hasPerso` à true
- Sous la boucle, à l'extérieur :
  - Si `hasPerso` n'est pas vrai. (Pensez point d'exclamation)
    - Copiez-collez les 3 lignes de création d'un élément de liste afin de créer un élément de liste qui dit : `Vous devez faire un choix.`
- Testez! Votre message devrait apparaître sans sélection

<br><br><hr>

[Passer à l'étape suivante ▶](g.md)

<hr><br>

[◀ Retourner à l'étape précédente](e.md)
