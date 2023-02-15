# `Étape 2` - Classe Army

## Classe Army

1. Au début du constructeur, ajoutez `console.log('#1 - new Army')`
1. Éléments à créer dans le constructeur :
   - Une variable globale `element` qui contient l'élément HTML qui devra être passé en paramètre du constructeur. (Indice, vous devrez retourner dans `Main` ajouter quelque chose en paramètre dans votre instanciation)
<br><br>

> **IMPORTANT**  
> Lorsqu'on veut sélectionner un élément HTML qui ne fait PAS parti de l'élément HTML de la classe en cours, on utilise `document.querySelector`.  <br><br>
> Cependant, il arrivera souvent qu'on veuille sélectionner que des éléments HTML qui **sont à l'intérieur** d'une instance en particulier et non pas dans toute la page (ici, la classe `Army`). Dans la structure que nous utilserons pour TimTools cette session, on veut alors **TOUJOURS** utiliser `this.element.querySelector` ou `this.querySelectorAll` pour aller chercher les références.

<br>

3. La classe doit avoir une méthode `init` :
   - Crééz une variable `persos` qui doit contenir tous les éléments HTML avec la classe css `js-perso`. (Indice: Voir la note ci-haut, ici on veut seulement ceux qui sont dans this.element).
   - Faire une boucle dans tous les éléments de la variable `persos`
     - Créer une variable `perso` (singulier de persos) qui contiendra l'élément en cours dans l'itération de la boucle. _Pensez i_
     - Ajouter un `click` sur votre variable `perso` qui appelle la méthode togglePerso() que vous devez aussi créer
     - _N'oubliez pas l'exception du contexte pour votre événement_


2. Dans la méthode `togglePerso` :
     - Ajoutez un console log avec `#2 - togglePerso dans Army`
     - Testez dans le navigateur.
     - Vous devrez récupérer les informations de l'événement avec le paramètre `event` afin de savoir sur quel élément vous avez cliqué.
     

> `event.currentTarget` retourne l'élément HTML sur lequel le click a été enregistré.

3. Lors du click, vous devrez ajouter la classe css d'état `is-active` si elle n'est pas sur l'élément ou l'enlever si elle est déjà présente. Comme un espèce de _toggle_.

[Voir la référence pour vous aider](https://developer.mozilla.org/fr/docs/Web/API/Element/classList)

4. Testez à nouveau, vous devriez voir les cartes s'agrandir.

<br><br><hr>

[Passer à l'étape suivante ▶](c.md)

<hr><br>

[◀ Retourner à l'étape précédente](a.md)
