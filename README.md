# npmdoc-react-monocle

#### api documentation for  [react-monocle (v0.1.6)](https://github.com/team-gryff/react-monocle#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-monocle.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-monocle) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-monocle.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-monocle)

#### A developer tool to visualize a React application's component hierarchy.

[![NPM](https://nodei.co/npm/react-monocle.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-monocle)

- [https://npmdoc.github.io/node-npmdoc-react-monocle/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-monocle/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-monocle/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael-Bryant Choa"
    },
    "babel": {
        "presets": [
            "airbnb",
            "react",
            "es2015",
            "stage-1"
        ],
        "plugins": [
            "transform-runtime"
        ]
    },
    "bin": {
        "monocle": "./bin/cmd.js"
    },
    "bugs": {
        "url": "https://github.com/team-gryff/react-monocle/issues"
    },
    "dependencies": {
        "acorn": "^3.2.0",
        "acorn-bfs": "^0.1.0",
        "acorn-jsx": "^3.0.1",
        "app-root-path": "^1.2.1",
        "commander": "^2.9.0",
        "d3": "^4.1.0",
        "escodegen": "^1.8.0",
        "glob": "^7.0.5",
        "lodash.assign": "^4.0.9",
        "lodash.clonedeep": "^4.3.2",
        "lodash.isequal": "^4.2.0",
        "react": "^15.1.0",
        "react-dom": "^15.1.0",
        "react-popover": "^0.4.4",
        "react-redux": "^4.4.5",
        "redux": "^3.5.2",
        "strip-comments": "^0.4.4"
    },
    "description": "A developer tool to visualize a React application's component hierarchy.",
    "devDependencies": {
        "babel-cli": "^6.9.0",
        "babel-core": "^6.9.0",
        "babel-eslint": "^6.0.4",
        "babel-loader": "^6.2.4",
        "babel-plugin-transform-runtime": "^6.9.0",
        "babel-polyfill": "^6.9.0",
        "babel-preset-airbnb": "^2.0.0",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-react": "^6.5.0",
        "babel-preset-stage-1": "^6.5.0",
        "babel-register": "^6.9.0",
        "babel-runtime": "^6.9.2",
        "chai": "^3.5.0",
        "eslint": "^2.9.0",
        "eslint-config-airbnb": "^9.0.1",
        "eslint-plugin-import": "^1.10.0",
        "eslint-plugin-jsx-a11y": "^1.5.3",
        "eslint-plugin-react": "^5.2.2",
        "express": "^4.13.4",
        "jsdom": "^9.2.1",
        "mocha": "^2.5.3",
        "nodemon": "^1.9.2",
        "react-addons-test-utils": "^15.1.0",
        "react-hot-loader": "^1.3.0",
        "rebass": "^0.3.0",
        "svg-inline-loader": "^0.6.1",
        "uglify-loader": "^1.3.0",
        "webpack": "^1.13.1",
        "webpack-dev-middleware": "^1.6.1",
        "webpack-dev-server": "^1.14.1",
        "webpack-hot-middleware": "^2.10.0"
    },
    "directories": {},
    "dist": {
        "shasum": "2ac3a247981f77520f13d0dc83b72218a7c286f7",
        "tarball": "https://registry.npmjs.org/react-monocle/-/react-monocle-0.1.6.tgz"
    },
    "gitHead": "5dbc35df3cac2104731a410667a8b24357123921",
    "homepage": "https://github.com/team-gryff/react-monocle#readme",
    "keywords": [
        "react",
        "visualization",
        "d3",
        "developer",
        "tool"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "jdavis218"
        },
        {
            "name": "jerrymao"
        },
        {
            "name": "mbchoa"
        }
    ],
    "name": "react-monocle",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/team-gryff/react-monocle.git"
    },
    "scripts": {
        "build": "webpack --progress --colors --config  webpack.production.config.js --watch",
        "bundle-d3tree": "webpack --watch -d ./src/d3Tree/index.js ./src/d3Tree/bundle.js",
        "lint": "eslint src",
        "start": "nodemon server/server.js",
        "test": "npm run lint || true && npm run unit-tests",
        "unit-tests": "mocha ./src/test/test.js"
    },
    "version": "0.1.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
