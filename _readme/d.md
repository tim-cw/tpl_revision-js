# `Étape 4` - Travaillons sur la classe Perso

Il faut maintenant gérer l'ouverture et la fermeture de la carte, ainsi que sa sélection / déselection.

## Classe Perso

1. Élément a créer dans le constructeur:
   - une variable globale `element` qui contient l'élément HTML en paramètre du constructeur
   - une variable globale `name` qui correspond au `inner text` de l'élément avec la classe css `js-name` (Attention, vous ne devez pas utiliser document. ...)   
   - Au début du constructeur, ajoutez `console.log('#2 - new Perso')` qui devrait apparaître 9 fois.
1. La classe doit avoir une méthode `init`
   - Ajouter un `click` sur _l'élément HTML_ qui représente votre instance. Ce click appellera une méthode `togglePerso`
   - _N'oubliez pas l'exception du contexte pour un événement click_

### `Méthode togglePerso`

1. Déplacez la méthode `togglePerso` commentée de la classe `Army` sous la méthode init de votre classe `Perso`.

   - Décommentez la méthode
   - Remplacez le bout `event.currentTarget` afin d'utiliser la variable globale `element` que vous aviez déjà créé dans votre constructeur
   - Changez le texte dans le console pour `#3 - openPerso`
   - Testez!

<br>

Nous aimerions maintenant avoir accès à l'état du perso dans notre Javascript. Pour l'instant, nous ajoutons ou retirons une classe css lors du click. La seule manière de savoir l'état est de faire la requête dans le HTML à chaque fois, ce qui n'est pas l'idéale. Donc, nous allons créer une variable qui contiendra également l'état (actif / inactif)

2. Dans le constructeur, créer la variable globale `isActive` avec la valeur assignée à faux
3. De retour dans la méthode `togglePerso`, inversez la valeur de la variable globale `isActive`. L'aide-mémoire des Google Slide pourrait vous aider.

### `Avant de passer à l'étape suivante`

Voici où vous devez en être :

- On clique sur le titre pour agrandir / minifier une carte
- L'état `isActive` se met à jour lorsque je clique sur une carte et je l'ai vérifié avec un `console.log`

<br><br><hr>

[Passer à l'étape suivante ▶](e.md)

<hr><br>

[◀ Retourner à l'étape précédente](c.md)
