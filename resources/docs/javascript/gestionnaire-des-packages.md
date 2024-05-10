[TOC]

# <b> Gestion des packages en javaScript </b>
## **Objectifs d'apprentissage**

- Utiliser npm comme système de progiciels.

## **Description**

Dans cette leçon, vous apprendrez à utiliser le code préparé par quelqu'un d'autre dans votre projet de manière efficace en utilisant le gestionnaire de paquets.

## **Pourquoi est-ce important?**

Si vous pouvez utiliser le code de quelqu'un d'autre pour construire votre application, il n'est pas nécessaire de réinventer la roue. Cette réutilisation du code est considérée comme une bonne pratique.

Une collection de code réutilisable qui peut fournir à votre application des fonctionnalités supplémentaires s'appelle un **paquet**. Cependant, il est parfois aussi appelé un **bibliothèque** ou **dépendance**.

Vous pouvez accéder aux packages que d'autres développeurs ont écrits via un **gestionnaire de paquets**, qui est l'outil CLI qui vous permet de les télécharger et de les installer sur votre machine locale.

## **Gestionnaire de paquets**

Tout d'abord, lisez à propos [dépendances dans votre projet](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Understanding_client-side_tools/Package_management#a_dependency_in_your_project).

Ensuite, lisez la partie [Qu'est-ce qu'un gestionnaire de paquets?](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Understanding_client-side_tools/Package_management#what_exactly_is_a_package_manager) pour avoir une idée générale de ce concept.

### **npm en tant que gestionnaire de paquets**

- `npm`[Pourquoi Avez-vous Besoin de Nœud pour un Projet Front End?](https://www.freecodecamp.org/news/how-to-set-up-a-front-end-development-project/#why-do-you-need-node-for-a-front-end-project)
    
    est associé à node.js et cela peut être déroutant. Lisez donc d'abord le fragment suivant
    
- Ensuite, lisez ["Qu'est-ce que npm?"](https://docs.npmjs.com/about-npm)  et ["Qu'est-ce que npm?" par w3schools](https://www.w3schools.com/whatis/whatis_npm.asp)
- npm est installé avec Node.js. Cela signifie que vous devez installer Node.js pour que npm soit installé sur votre ordinateur.
    - [Téléchargez-le](https://nodejs.org/en/download/)
    - Vérifier l'installation
    
    ```js
      node -v
      npm -v
    ```
    

**Alerte spoiler:** Ci-dessus, nous vous pointons vers les parties spécifiques de l'article "Comment mettre en place un projet de développement frontal". Vous pouvez voir dans cet article également une partie sur Webpack. Veuillez l'ignorer, pour l'instant, vous en apprendrez plus sur Webpack dans une leçon distincte.

## **Modules et packages ES6**

Réfléchissons un peu aux modules ES6. Rappelez-vous comment vous pouvez importer vos modules? Voici la bonne nouvelle: vous pouvez également importer des modules à partir du code externe que vous ajoutez à votre projet sous forme de package. Jetez un œil à l'exemple de la bibliothèque Three.js: [Installer à partir de npm](https://threejs.org/docs/index.html#manual/en/introduction/Installation). Pour utiliser ses fonctions, vous devez:

- Installez-le avec npm:

```js
npm install --save three
```

- Importez-le dans votre code:

```js
import * as THREE from 'three';
```

## **Organisation de votre code ES6**

Avec des packages externes et vos propres modules, vous pouvez mieux organiser votre code frontal.

- Vérifier [Comment ajouter des bibliothèques à votre projet JavaScript](https://www.freecodecamp.org/news/how-to-set-up-a-front-end-development-project#how-to-add-libraries-to-your-javascript-project) pour voir un exemple de projet bien structuré.
    

**Alerte spoiler:** Ci-dessus, nous vous pointons vers les parties spécifiques de l'article "Comment mettre en place un projet de développement frontal". Vous pouvez voir dans cet article également une partie sur Webpack. Veuillez l'ignorer, pour l'instant, vous en apprendrez plus sur Webpack dans une leçon distincte.