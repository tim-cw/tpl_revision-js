# Révision Les généraux de la TIM

## `Étape 3` - Réusinage

Nous venons de faire une classe Armée avec des personnages. On mélange un peu les idées et le code peut vite devenir chaotique. Que se passe-t-il si on a besoin de faire faire autre chose à nos personnages qu'un simple clic? Nous aurons une classe qui devient êxtrement longue qui va gérer de multiple idées. Nous allons essayer de regrouper nos idées dans des classes séparées.

Donc, on va créer une classe Perso, mais avant adaptons notre classe Army.

### Classe Army

1. Mettez la méthode `togglePerso` en commentaire, on va la réutiliser plus tard
1. Pour garder en mémoire tous les personnages de notre armée
   - Dans le constructeur, créez une variable globale `army` qui est de type tableau
1. Dans la boucle que vous avez fait à l'étape 2, effacez au complet la ligne de l'écouteur sur un clic
   - Créer une variable `perso` sous `qui créera une nouvelle instance de votre classe Perso en lui passant en paramètre la variable `element`.
   - Ajouter votre variable `perso` dans votre tableau(array) `army`. [Méthode d'un array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#instance_methods)

<br><br><hr>

[Passer à l'étape 4 ▶](etape4.md)

<hr><br>

[◀ Retourner à l'étape 2](etape2.md)
