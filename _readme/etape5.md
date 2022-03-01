# Révision Les généraux de la TIM

## `Étape 5` - Validation des choix

Il faut maintenant générer une liste contenant vos choix (sélections)

### Classe Army

1. Après la boucle :
   - une variable `btnValidate` qui sélectionne l'élément avec `.js-validate`
   - Ajouter un `click` sur la variable précédente qui appelle la méthode setSelection();
     - _N'oubliez pas le bind_
1. Dans la méthode `setSelection` :
   - Créer une variable `list` qui sélectionne la liste du html(ul) qui contient une classe css. Allez voir dans le html pour trouver le nom de la classe.
   - Faire en sorte que le contenu HTML de cette liste soit vide avant de poursuivre (Pensez string vide)
     - Faire une boucle dans tous les éléments de la variable `army`
     - Créer une variable `perso` qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i._

Ici, on ne veut prendre que les persos qui sont sélectionnés (ceux pour lesquels leur propriété `isActive` a été mis à true dans la classe Perso).
On peut appeller une méthode ou obtenir le contenu d'une variable globale d'une instance en utilisant le principe `[instance].[methode/variable]`

1. Si `perso` a sa variable isActive de vraie
   - Créez un console.log qui utilise le _template string_ afin d'obtenir cette structure dans la console :
     - `#4 - [perso.name] est actif`
   - Créez un li avec `createElement` qui sera stocké dans la variable `listItem`
   - Assignez-lui la valeur de la variable `name` qui provient de l'instance `perso`
   - Ajoutez l'élément que vous venez de créer comme un enfant de la `list` créé un peu plus haut

<br><br><hr>

[Passer à l'étape 6 ▶](etape6.md)

<hr><br>

[◀ Retourner à l'étape 4](etape4.md)
