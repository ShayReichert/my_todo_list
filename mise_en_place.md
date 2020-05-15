# Creer un package.json et lancer un script sass

// Copier-coller //

 "sass": "sass --watch ./sass/main.scss:./css/style.css"
 "prefix": "postcss ./css/style.css --use autoprefixer -d ./css/prefixed/"
 "browserslist": "last 4 versions"


Etapes :
1 Créer un package.json : npm init
    (installer sass : npm install sass -g puis sass --version)

2 Définir un script Sass :
"scripts": {
  "sass": "sass --watch ./css/style.scss:./css/style.css"
},

4  Enregistrer, puis lancer Sass 
npm run sass


5 A la suite, définir un script Prefix (pour compatibilité navigateurs) :
    "prefix": "postcss ./css/style.css --use autoprefixer -d ./css/prefixed/"

    Ajouter à la fin : 
    "browserslist": "last 4 versions"
    }

6 Pour lancer prefix : 
npm run prefix