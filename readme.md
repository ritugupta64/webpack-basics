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


After that...

Add "build":"webpack --mode production"

"dev":"webpack --mode development"

npm run build for minified the version
npm run dev for production