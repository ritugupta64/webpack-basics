Webpack for zero configuration...

Initialize a package.json by running:

npm init -y

and pull webpack 4 in:

npm i webpack --save-dev

We need webpack-cli also, which lives as a separate package:

npm i webpack-cli --save-dev

Now open up package.json and add a build script:

"scripts": {
  "build": "webpack"
}



before it...

create the folder like src/index.js// its the default name

after that put the script along with dist/main.js


=====================================

Add "build":"webpack --mode production"

"dev":"webpack --mode development"

npm run build for minified the version
npm run dev for production

=======================================

overriding the defaults entry/output

Add "build":"webpack --mode production ./src/js/index.js"

"dev":"webpack --mode development"

its just the entry point and you can also set the o/p point --output ./foo/main.js in both build and dev

=======================================

Webpack dev server

- npm i webpack-dev-server --save-dev

- add on 

First method..
which is not correct

"start":"webpack-dev-server --mode development --open"
"build":"webpack --mode production"

- npm run start

-We should have the dist folder..


Second method..

"build":"webpack-dev-server --mode production --entry ./src/js/index.js --output-filename ./dist/main.js"

npm run build

