1) On PowerShell:

mkdir my-app && cd my-app   // Se necessario
ni .gitignore // Se necessario
npm init -y
npm install laravel-mix --save-dev

ni webpack.mix.js

-----------------------------------------------------

2) Create a src folder:

mkdir src
cd src
ni app.js
ni app.scss

-----------------------------------------------------

3) on webpack.mix.js:

let mix = require('laravel-mix');

mix
.js('src/app.js', 'dist/')
.sass('src/app.scss', 'dist/')
.options({
    processCssUrls: false
});

-----------------------------------------------------

4) Create a index.htm:

ni index.html

-----------------------------------------------------

5) Run Laravel Mix:

npx mix
npx mix watch 



