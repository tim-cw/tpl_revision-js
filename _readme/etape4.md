# Révision Les généraux de la TIM

## `Étape 4` - On complète la classe Perso

Il faut maintenant gérer l'ouverture et la fermeture de la carte, ainsi que sa sélection / déselection.

### Classe Perso

1. La classe doit contenir le minimum pour être une classe
1. Élément a créer dans le constructeur:
   - une variable globale `element` qui contient l'élément HTML en paramètre du constructeur
   - une variable globale `name` qui correspond au texte du h2 de l'élément
   - une variable globale `isActive` avec la valeur à faux
   - une variable globale `btnSelect` qui contient l'élément titre des cartes qui a la classe css `js-select`
   - une variable globale `btnAdd` qui contient le bouton de sélection des cartes qui a la classe css `js-add`
   - Au début du constructeur, ajoutez `console.log('#2 - new Perso')` qui devrait apparaître 9 fois
1. La classe doit avoir une méthode `init`
   - Ajouter un `click` sur votre variable `btnSelect` qui appelle la méthode togglePerso();
   - Ajouter un `click` sur votre variable `btnAdd` qui appelle la méthode selectPerso();
   - _N'oubliez pas le bind pour les 2 points précédents_

#### `Méthode togglePerso`

1. Déplacez la méthode `togglePerso` commentée de la classe `Army` sous la méthode init.

   - Décommentez la méthode
   - Changez `event.currentTarget` afin d'utiliser la variable globale `element`
   - Changez le texte dans le console pour `#3 - openPerso`
   - Testez!

#### `Méthode selectPerso`

1. Inverser la valeur de votre variable globale `isActive`
1. Alterner la classe css `opened` en utilisant une méthode de classList sur votre variable `element`

Au fait, avez-vous vu un bouton lorsque vous avez agrandit une carte? Ce dernier est fait à l'aide de 2 icônes qui s'affichent un à la fois selon l'état.

1. Trouvez pourquoi les icônes n'apparaissent pas et réglez le problème.

#### `Avant de passer à l'étape suivante`

Voici où vous devez en être :

- On clique sur le titre pour agrandir / minifier une carte
- On clique sur le plus pour sélectionner une carte
- On clique sur le moins pour déselectionner une carte

<br><br><hr>

[Passer à l'étape 5 ▶](etape5.md)

<hr><br>

[◀ Retourner à l'étape 3](etape3.md)
