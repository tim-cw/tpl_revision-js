# Révision Les généraux de la TIM

## `Étape 3` - Classe Army

### Classe Army

1. Au début du constructeur, ajoutez `console.log('#1 - new Army')`
1. Éléments à créer :
   - une variable globale `element` qui contient l'élément HTML en paramètre du constructeur
1. La classe doit avoir une méthode `init`
   - une variable `persos` qui sélectionne tous les éléments HTML data-army qui ont la valeur `perso`
   - Faire une boucle dans tous les éléments de la variable `persos`
     - Créer une variable `element` qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i_
     - Ajouter un `click` sur votre variable `element` qui appelle la méthode togglePerso();
     - _N'oubliez pas le bind_
     - Ajoutez un console log avec `#2 - togglePerso dans Army` dans cette méthode
     - Testez dans le navigateur
     - Dans cette méthode, utilisez `event.target`, qui permet de savoir sur quel élément on a cliqué, afin de lui ajouter la classe `opened` s'il ne l'a pas, ou de la retirer s'il l'a. (un genre de toggle)
     - Testez à nouveau, vous devriez voir les cartes s'agrandir

<br><br><hr>

[Passer à l'étape 3 ▶](etape3.md)

<hr><br>

[◀ Retourner à l'étape 1](etape1.md)
