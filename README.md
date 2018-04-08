# mern-stack
Another boilerplate code for getting started with MERN stack using Webpack

## Introduction
This is an example generic code to help you (and me) to get started with the MERN (MongoDB, ExpressJS, ReactJS and NodeJS) stack.

* M ongoDB - https://www.mongodb.com/
* E xpressJS - https://www.expressjs.com/
* R eactJS - https://facebook.github.io/react/
* N odeJS - https://nodejs.org/en/

As well as:

* BabelJS - https://www.babeljs.io/
* css-loader - https://github.com/webpack/css-loader/
* node-sass - https://github.com/sass/node-sass/
* sass-loader - https://github.com/jtangelder/sass-loader/
* react-bootstrap - https://react-bootstrap.github.io/
* style-loader - https://github.com/webpack/style-loader/
* Webpack - https://webpack.github.io/
* webpack-dev-middleware - https://github.com/webpack/webpack-dev-middleware/
* webpack-hot-middleware - https://github.com/glenjamin/webpack-hot-middleware/

## Install
On this step you should be able to run the project typing:
```
  git clone https://github.com/ateixeira/mern-stack.git
  git checkout tags/4-hot-assets-build-first-layout-and-sass
  cd mern-stack
  npm install
```
## Build the app
```
  npm run build
```
## Run the development server
```
  npm start
```
## Production deployment
The webpack configuration file was separeted in **webpack.prod.config.js** and **webpack.dev.config.js**. On server/server.js file, based on the env variable ENV_NODE, the proper configuration file is loaded on webpack hot/dev middleware in case of development env.

When deployed to production (first tests were made using Heroku), the npm **postintall** directive when called runs **npm run build**, that sets the ENV_NODE to production and bundles the app with the --config flag pointing to the production config file.

To try it on heroku just push the app up and it will transparently be set-UP.


## Additional Information
It's already 4 years since I first read about the possibilities of Javascript taking place as a complete (Full Stack) architecture for web applications. In the last 3 years I gradually started some changes on this way while coding urbanizo.com, at first migrating it's models to [MongoDB](https://www.mongodb.org), as well as using [BackboneJS](http://www.backbonejs.org/) in the whole application interface. I created this project to get used to Node.js, the piece that was missing to take javascript to the whole web stack of one of my projects.

### ~~Isomorphic~~ Universal Javascript
From now on I will focus **mern-stack** development on a major advantage of Node.js, the capability to run javascript both on **client** and **server**. This ability makes room to a new way of producing javascript that is not enviroment dependent, also known as Universal Javascript.

I will avoid going to far on this subject, since there are lots of very good content about it's advantages on the web, and the purpose of this project is to share an example on how to implement it.
