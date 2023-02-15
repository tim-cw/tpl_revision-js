# `Étape 5` - Validation des choix

Après avoir choisi les différents guerriers, soit ceux qui possède le classe `is-active`, nous allons générer et afficher une liste qui contient nos choix.

## De retour dans la classe Army

1. Dans init, après la boucle :
   - Créez une variable `btnValidate` qui sélectionne l'élément avec `.js-validate`
   - Ajouter un `click` sur la variable précédente qui appelle la méthode setSelection();
     - _N'oubliez pas le bind_
1. Dans la méthode `setSelection` :
   - Créer une variable `list` qui sélectionne la liste du html (ul) qui contient une classe css. Allez voir dans le html pour trouver le nom de la classe.
   - Faire en sorte que le contenu HTML de cette liste soit vide avant de poursuivre (Pensez string vide)
     - Faire une boucle dans tous les éléments de la variable globale `army`
     - Créer une variable `perso` qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i._

Ici, on ne veut prendre que les persos qui sont sélectionnés (ceux pour lesquels leur _propriété_ `isActive` a été mis à true dans la classe Perso).

On peut appeller une méthode ou obtenir le contenu d'une variable globale d'une instance en utilisant le principe `[instance].[methode/variable]` tant qu'elle est dans le contexte global de cette instance.

### À l'intérieur de la boucle créé précédemment:
1. Si `perso` a sa variable isActive de vraie :
    - Créez un console.log qui utilise le `Template String` afin d'obtenir cette structure dans la console :
      - `#4 - [perso.name] est actif`
   - Créez un li avec `createElement` qui sera stocké dans la variable `listItem`
   - Assignez-lui la valeur de la variable `name` qui provient de l'instance `perso`
   - Ajoutez l'élément que vous venez de créer comme un enfant de la `list` créé un peu plus haut

<br><br><hr>

[Passer à l'étape suivante ▶](f.md)

<hr><br>

[◀ Retourner à l'étape précédente](d.md)
