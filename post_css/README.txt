https://github.com/postcss/postcss-cli
https://www.npmjs.com/package/postcss-import
https://jolicode.com/blog/passer-a-postcss-pour-un-projet-sans-sass
======
npm install --save-dev postcss postcss-cli
npm install --save-dev postcss-import
npm install --save-dev postcss-nested
npm install --save-dev autoprefixer
npm install --save-dev tailwindcss @tailwindcss/postcss
======
Les différents plugins postcss à utiliser (avec ou sans options) 
doivent être renseignés dans le fichier 
postcss.config.js 
======
NB: postcss-cli permet un déclenchement en ligne de commande (in peu comme saas)

    le plugin postcss-import permet de gérer @import 'sxyz'; dès la phase de dev
    ce qui évitera de multiples téléchargement successifs au runtime

    le plugin postcss-nested permet de gérer l'imbrication de styles 
    avec même syntaxe que scss (&:hover { ... })

    Attention: ne pas utiliser  @apply du plugin postcss-apply qui ne fonctionne pas bien .
    D'ailleurs cette version de @apply n'a pas été retenu par la norme css (pas gére par navigateur)
    il vaut mieux utiliser le @apply spécifique à tailwind 
=====
pour reproduire le comportement de saas , on pourrait utiliser les plugins postcss suivants:
    postcss-extend-rule , postcss-mixin, postcss-define-function mais avec beaucoup de restrictions , de sources de conflits possibles , ...
    et donc au final , tout ça n'est pas très conseillé !!!!
======
postcss input.css -o global.css
postcss src/input-styles/app.css --dir src/output-styles
====
npm run pcss si script de lancement postcss dans package.json
