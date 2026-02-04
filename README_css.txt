Le mode "retina" correspond aux écrans de certains "Apple" qui ont une très grande résolution et qui peuvent afficher énormément de pixels
----
besoin soit de media-query pour utiliser alternativement plusieurs versions d'une image (en haute et basse résolution).
       soit d'exploiter l'attribut srcset de la balise <img > d'HTML moderne pour spécifier une liste d'images que le navigateur choisira selon la résolution de l'écran 
Tout est bien expliqué au bout de ce lien hypertexte:
       https://buzut.developpez.com/tutoriels/optimiser-images-responsive-ecrans-retina/
========================

Accessibilité / ARIA:

Accessible Rich Internet Applications (ARIA) (qu'on pourrait traduire par « applications internet riches et accessibles ») est un ensemble de rôles et d'attributs d'attributs qui définissent comment rendre le contenu et les applications web accessibles (notamment ceux développés avec JavaScript) pour les personnes avec des handicaps.

Attention: les navigateurs gèrent pas trop mal "ARIA" sur les composants standards HTML et les balises sémantiques
Si l'on se code soit même de nouveau composants à base de <div> , il faudrait idéalement ajouter des paramétrages aria-xyz .
Et attention , code du mauvais aria peut être pire que pas d'aria du tout !!!
-----
Les rôles ARIA sont des attributs ajoutés au code HTML pour améliorer l'accessibilité . Ils définissent des finalités spécifiques pour les éléments d'une page web, permettant ainsi aux technologies d'assistance, comme les lecteurs d'écran, de les comprendre et d'interagir avec eux.
----
en France, Référentiel général d’amélioration de l’accessibilité (RGAA) (document pdf édité par le gouvernement: https://accessibilite.numerique.gouv.fr/)
---
https://www.accede-web.com/