## Сборка проекта на gulp. Версия 1. 
Описание:
Данная сборка создает красивый, но не минимизарованный код.
### Вариант №1
Для начала работы скопировать в нужную папку package.json, 
gulpfile.js и запустить в командной строке:  
    
    npm i
### Вариант №2.
Создать структуру проекта:

    mkdir -p app/{html,fonts,img,js,less} build
Создать основные файлы:
    
    touch app/html/index.html app/less/styles.less app/less/normalize.less app/js/1.js 
Инициализация проекта. Создается package.json:
    
    npm init -y
Установка gulp локально:

    npm install gulp --save-dev
Установка плагинов:

    npm i browser-sync del gulp-autoprefixer gulp-clean-css gulp-concat gulp-imagemin gulp-less gulp-pretty-html 
    gulp-sourcemaps normalize.less gulp-newer ---save-dev

Создать gulpfile.js    
    
    touch gulpfile.js 

Создать .gitignore следующего содержания: 

    .idea/*
    .gitignore
    #.idea/CorporateBlue.iml
    #.idea/encodings.xml
    #.idea/misc.xml
    #.idea/modules.xml
    #.idea/workspace.xml
    build/
    node_modules/
    package-lock.json
    package.json
