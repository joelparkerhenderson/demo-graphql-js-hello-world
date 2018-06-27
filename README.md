# Demo GraphQL.js hello world

Demonsrate:

  * [GraphQL.js](https://github.com/graphql/graphql-js) that prints "hello world".
  * [Babel](https://babeljs.io/): The compiler for next generation JavaScript
  * [npm](https://npm.js): Node package manager


## Init

```sh
$ npm init
```


## demo.js

Create a file such as [demo.js](demo.js) (see the file in this repo).

The demo file will do two things:

 * Build a GraphQL type schema which maps to your code base.

 * Serve the result of a query against that type schema.


## Babel

As of this writing, Node.js doesn't support ES6 imports yet. However, you can use them today with the help of Babel.

```sh
$ npm install babel-register babel-preset-env --save-dev
```

Create a file such as [start.js](start.js) (see the file in this repo).

The file does two things:

  * Transpile all code with babel and using 'env' preset.

  * Import the rest of our application.

Babel solves this error message:

```sh
(function (exports, require, module, __filename, __dirname) { import {
SyntaxError: Unexpected token
```


## Run

Run the app:

```sh
$ node start.js
{ data: { hello: 'world' } }
```
