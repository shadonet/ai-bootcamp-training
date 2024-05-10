[TOC]

# <b> ES6 de quoi s'agit-il ? </b>

## Objectifs d'apprentissage

- Apprenez à utiliser la syntaxe ES6 appropriée.
- Comprenez les améliorations que ES6 apporte à JavaScript.

## ECMAScript 6 ( ES6 )

Le nom officiel de JavaScript est ECMAScript (ES en abrégé). Jusqu'en 2015, les versions ultérieures de ES étaient numérotées consécutivement avec des entiers, mais à partir de la version 6, les créateurs ont décidé de nommer de nouvelles versions d'ES en utilisant l'année de publication au lieu d'entiers.Pour cette raison, vous pouvez rencontrer le nom ES2015 utilisé de manière interchangeable pour ES6.

## Pourquoi est-ce important?

La sixième édition d'ES a apporté de nombreuses excellentes solutions et améliorations à la langue. Les bibliothèques *Transpilers*, *shim*,  *polyfill*  associées au développement dynamique des navigateurs signifient que les programmeurs peuvent très rapidement utiliser toutes les possibilités que JavaScript a maintenant à offrir, ce qui en fait l'un des langages de programmation les plus populaires au monde.

## `let`, `const` et *portée de bloc*

Une des idées les plus fondamentales de tout langage de programmation est **portée**. Chaque variable déclarée par le programmeur vit dans une certaine portée. Avant ES6, JavaScript utilisait un mot-clé pour déclarer des variables `var` - et deux étendues principales où les variables vivaient:

- **Portée Globale.**
- **Portée locale (fonction)**

Entre autres nouveaux changements de syntaxe, ES6 a introduit deux nouveaux mots-clés pour les déclarations de variables `const` et `let`. Il a également introduit *portée niveau bloc* pour les variables déclarées avec ces nouveaux mots clés. La déclaration correcte des variables est absolument essentielle pour toute application. Comprendre le fonctionnement de la portée et des nouveaux mots clés rendra votre code plus résistant aux erreurs inattendues et aux comportements indésirables.

### Pour apprendre ces concepts:

- [Lire à propos de la *portée*](https://dev.to/sandy8111112004/javascript-introduction-to-scope-function-scope-block-scope-d11).
- [Lire à propos `const`, `let` et en quoi elle diffère de `var`](https://dev.to/sandy8111112004/javascript-var-let-const-41he).

## Arrow functions

Une autre nouvelle fonctionnalité introduite dans la 6 ème version d'EcmaScript est la **Arrow functions**. Il a une nouvelle syntaxe plus courte, mais surtout, il n'a pas `this` de son propre. Problèmes de liaison `this` dans les fonctions JavaScript traditionnelles étaient la principale raison de l'introduction de la fonction flèche dans ES6. Nous avons maintenant une nouvelle façon puissante et prévisible d'écrire et d'utiliser des fonctions dans nos applications.

- Lisez à propos de *[Arrow functions](https://www.w3schools.com/js/js_arrow_function.asp)*.
- [Regardez cette courte vidéo](https://youtu.be/NAN7U3MrX6o)　pour vous familiariser avec eux.

## `Promises`

`Promises` est un nouvel intermédiaire fiable entre notre fonction d'appel et notre code asynchrone. Nous pouvons les considérer comme *valeur future* conteneurs. `Promises` représente une étape importante dans le développement de la programmation asynchrone en JavaScript. Ils introduisent l'ordre et garantissent la prévisibilité des événements.

- Lire à propos [créer et utiliser des promesses](https://javascript.info/promise-basics) dans ES6.

### `Spread` et `destructuring`


ES6 introduit un nouvel opérateur `...` (*propagation*) et une nouvelle capacité syntaxique appelée *déstructuration*. Les deux concepts ont rapidement fait partie de la communauté JavaScript et sont devenus partie intégrante de la plupart des applications modernes. Parmi les nombreux autres avantages de l'utilisation de la *propagation* opérateur, il vous permet d'appliquer facilement le concept d'"immutabilité", qui est crucial lors de la construction d'applications plus grandes et est devenu la base de bibliothèques telles que ReduxJS. La destruction, à son tour, est devenue la syntaxe principale de l'écriture *crochets* dans la bibliothèque populaire React. Comprendre ces deux concepts est essentiel pour les développeurs JavaSript.

Pour vous familiariser avec ces concepts:

- [Lire à propos *propagation* opérateur](https://www.geeksforgeeks.org/javascript-spread-operator/).
- [Lire à propos *déstructuration*](https://javascript.info/destructuring-assignment).
    

## Défiez-vous

Vérifiez votre compréhension de cette leçon. Essayez de répondre aux questions ci-dessous, puis exécutez les extraits de code dans la console pour voir si vous avez obtenu les bonnes réponses.

- **Question 1 - Quelle est la sortie de chacun des journaux de la console?**

```js
var color = "red";
let animal = "dog"
{
    var color = "blue";
    let animal = "cat"

    console.log(`log 1 - color: ${color}`);
    console.log(`log 2 - animal: ${animal}`);
}
console.log(`log 3 - color: ${color}`);
console.log(`log 4 - animal: ${animal}`);
```

- **Question 2 - Quelle est la sortie du journal de la console ?**

```js
const pr = new Promise(function(resolve,reject){
    setTimeout(() => resolve("foo"), 1000);
    setTimeout(() => resolve("bar"), 500);
})

pr.then(
    res => {
        console.log(res);
    },
    err => {
        console.log(err);
    }
)
```

## Matériaux supplémentaires

**Ceux-ci sont tous facultatifs, mais si vous êtes intéressé à explorer ce sujet plus loin, voici quelques ressources pour vous aider. Toute exploration ici devrait être faite en dehors du temps du programme.**

Dans cette leçon, nous avons couvert uniquement les nouvelles fonctionnalités ES6 les plus couramment utilisées. Pour certains, comme *classe* ou *module*, nous avons créé des leçons distinctes parce qu'elles sont plus complexes et nécessitent une étude plus détaillée. D'autres, cependant, ne seront pas discutés en détail parce que leur utilisation est trop spécifique et vous n'aurez probablement pas besoin d'eux à ce stade de l'apprentissage. Mais si vous voulez vous familiariser avec toutes les nouvelles fonctionnalités d'ES6, alors [consultez la documentation ES6 ici](http://es6-features.org/).

Vous pouvez également marquer [cette feuille de cheet](https://devhints.io/es6) pour référence future.