# `Étape 3` - Réusinage

Nous venons de faire une classe `Army` avec des personnages (`Perso`). On mélange un peu les idées et le code peut vite devenir chaotique. Que se passe-t-il si on a besoin de faire faire quelque chose de plus complexe qu'un simple click? Nous aurons une classe qui devient extrêmement longue qui va gérer de multiples idées. Revenons un peu sur nos pas afin de réorganiser le tout.

Nous allons maintenant créer une classe Perso.

### La classe Perso

1. Vous allez créer la classe `Perso` dans un fichier du même nom.
   - La classe doit être importable
   - Elle doit contenir un constructeur et un init.

### De retour à la classe Army

1. Mettez la méthode `togglePerso` en commentaire, on va la réutiliser plus tard.
1. Pour garder en mémoire tous les personnages de notre armée :
   - Dans le constructeur, créez une variable globale `army` qui sera de type tableau.

Pour créer un tableau vide, on peut utiliser une instance de la classe `Array` qui existe nativement en JavaScript. Il faut donc simplement utiliser le mot clé `new` avec le nom de cette classe en oubliant pas les parenthèses.

3. Dans la boucle que vous avez fait pour les `persos`,  effacez au complet la ligne de l'écouteur sur un clic, elle ne sera plus utile.

   - Toujours dans la boucle, créez une variable `instance` qui contiendra une référence de l'instance de la classe `Perso`. Essentiellement, quand vous crééz une instance de quelque chose, vous pouvez l'assigner à une variable, ce qu'on veut ici. `const instance = new Perso();`
   - N'oubliez pas de passer en paramètre à votre classe `Perso`, l'élément HTML qui correspond, soit votre variable `perso`.
>Finalement, nous voulons conserver chacune des instances que nous crééons dans la boucle et les stocker dans la variable globale `army`.

5. À la suite de l'étape suivante, dans la boucle, on va _pusher_ dans le tableau avec la méthode `push`.
   - La ligne devrait ressembler à ceci : `this.army.push(instance)`

<br><br><hr>

[Passer à l'étape suivante ▶](d.md)

<hr><br>

[◀ Retourner à l'étape précédente](b.md)
