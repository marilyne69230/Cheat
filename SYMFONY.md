**INSTALLATION PROJET SYMFONY**
    symfony new —webapp nomProjet
    
    - créer un fichier .env.local et ajouter :
-
    symfony console doctrine:database:create 


**INSTALLATION WEBPACK**
    composer require symfony/webpack-encore-bundle
    yarn install
    yarn add sass-loader --dev
    (si on veut du typescript sinon pas besoin)
    yarn add typescript ts-loader --dev

    - dans le fichier webpack.config, décommenter .enableSassLoader() & .enableTypeScriptLoader()


**INSTALLATION BOOTSTRAP**
    yarn add bootstrap
    yarn add @popperjs/core

    - renommer le fichier asset/style/app.css en app.scss
    - dans le fichier app.js changer le import './styles/app.css' —> import './styles/app.scss' et ajouter import 'bootstrap/dist/js/bootstrap'
    - dans le fichier app. scss ajouter avant le body @import"~bootstrap/scss/bootstrap" 
-
    yarn watch
    symfony serve


**CREATION ENTITY**
    symfony console make:entity
    symfony console make:migration
    symfony console d:m:m


**RELATION ENTITY**
    symfony console make:entity nomClass


**CONNEXION**
    symfony console make:user
    symfony console make:auth
    symfony console make:registration-form


**CREATION CONTROLLER**
    symfony console make:controller
    