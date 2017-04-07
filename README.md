# api documentation for  [react-monocle (v0.1.6)](https://github.com/team-gryff/react-monocle#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-monocle.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-monocle) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-monocle.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-monocle)
#### A developer tool to visualize a React application's component hierarchy.

[![NPM](https://nodei.co/npm/react-monocle.png?downloads=true)](https://www.npmjs.com/package/react-monocle)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-monocle_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-monocle/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-monocle/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael-Bryant Choa",
        "email": "mbchoa@gmail.com"
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
            "name": "jdavis218",
            "email": "jennadavis92@gmail.com"
        },
        {
            "name": "jerrymao",
            "email": "jerryy.mao@gmail.com"
        },
        {
            "name": "mbchoa",
            "email": "mbchoa@gmail.com"
        }
    ],
    "name": "react-monocle",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-monocle](#apidoc.module.react-monocle)
1.  [function <span class="apidocSignatureSpan">react-monocle.</span>esquery (ast, selector)](#apidoc.element.react-monocle.esquery)
1.  object <span class="apidocSignatureSpan">react-monocle.</span>esrecurse
1.  object <span class="apidocSignatureSpan">react-monocle.</span>estraverse
1.  object <span class="apidocSignatureSpan">react-monocle.</span>parser
1.  object <span class="apidocSignatureSpan">react-monocle.</span>previewParser
1.  object <span class="apidocSignatureSpan">react-monocle.</span>reactParser
1.  object <span class="apidocSignatureSpan">react-monocle.</span>stringRegexHelper

#### [module react-monocle.esquery](#apidoc.module.react-monocle.esquery)
1.  [function <span class="apidocSignatureSpan">react-monocle.</span>esquery (ast, selector)](#apidoc.element.react-monocle.esquery.esquery)
1.  [function <span class="apidocSignatureSpan">react-monocle.esquery.</span>match (ast, selector)](#apidoc.element.react-monocle.esquery.match)
1.  [function <span class="apidocSignatureSpan">react-monocle.esquery.</span>matches (node, selector, ancestry)](#apidoc.element.react-monocle.esquery.matches)
1.  [function <span class="apidocSignatureSpan">react-monocle.esquery.</span>parse (selector)](#apidoc.element.react-monocle.esquery.parse)
1.  [function <span class="apidocSignatureSpan">react-monocle.esquery.</span>query (ast, selector)](#apidoc.element.react-monocle.esquery.query)

#### [module react-monocle.esrecurse](#apidoc.module.react-monocle.esrecurse)
1.  [function <span class="apidocSignatureSpan">react-monocle.esrecurse.</span>Visitor (visitor, options)](#apidoc.element.react-monocle.esrecurse.Visitor)
1.  [function <span class="apidocSignatureSpan">react-monocle.esrecurse.</span>visit (node, visitor, options)](#apidoc.element.react-monocle.esrecurse.visit)

#### [module react-monocle.estraverse](#apidoc.module.react-monocle.estraverse)
1.  [function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>Controller ()](#apidoc.element.react-monocle.estraverse.Controller)
1.  [function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>attachComments (tree, providedComments, tokens)](#apidoc.element.react-monocle.estraverse.attachComments)
1.  [function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>cloneEnvironment ()](#apidoc.element.react-monocle.estraverse.cloneEnvironment)
1.  [function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>replace (root, visitor)](#apidoc.element.react-monocle.estraverse.replace)
1.  [function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>traverse (root, visitor)](#apidoc.element.react-monocle.estraverse.traverse)
1.  object <span class="apidocSignatureSpan">react-monocle.estraverse.</span>Syntax
1.  object <span class="apidocSignatureSpan">react-monocle.estraverse.</span>VisitorKeys
1.  object <span class="apidocSignatureSpan">react-monocle.estraverse.</span>VisitorOption
1.  string <span class="apidocSignatureSpan">react-monocle.estraverse.</span>version

#### [module react-monocle.parser](#apidoc.module.react-monocle.parser)
1.  [function <span class="apidocSignatureSpan">react-monocle.parser.</span>SyntaxError (expected, found, offset, line, column)](#apidoc.element.react-monocle.parser.SyntaxError)
1.  [function <span class="apidocSignatureSpan">react-monocle.parser.</span>parse (input, startRule)](#apidoc.element.react-monocle.parser.parse)
1.  [function <span class="apidocSignatureSpan">react-monocle.parser.</span>toSource ()](#apidoc.element.react-monocle.parser.toSource)

#### [module react-monocle.previewParser](#apidoc.module.react-monocle.previewParser)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>getComponentName (bundle, startingIndex)](#apidoc.element.react-monocle.previewParser.getComponentName)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>getDivs (modifiedBundle)](#apidoc.element.react-monocle.previewParser.getDivs)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyBundleFile (bundlejs)](#apidoc.element.react-monocle.previewParser.modifyBundleFile)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyInitialState (modifiedBundle)](#apidoc.element.react-monocle.previewParser.modifyInitialState)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifySetStateStrings (bundleFilePath)](#apidoc.element.react-monocle.previewParser.modifySetStateStrings)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyTestBundleFile (bundle)](#apidoc.element.react-monocle.previewParser.modifyTestBundleFile)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>queryES5Ast (bundlejs)](#apidoc.element.react-monocle.previewParser.queryES5Ast)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>queryES6Ast (bundlejs)](#apidoc.element.react-monocle.previewParser.queryES6Ast)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>structureInitialES5StateObj (bundle, arr)](#apidoc.element.react-monocle.previewParser.structureInitialES5StateObj)
1.  [function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>structureInitialES6StateObj (bundle, arr)](#apidoc.element.react-monocle.previewParser.structureInitialES6StateObj)

#### [module react-monocle.reactParser](#apidoc.module.react-monocle.reactParser)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>componentChecker (ast)](#apidoc.element.react-monocle.reactParser.componentChecker)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>forInFinder (arr, name)](#apidoc.element.react-monocle.reactParser.forInFinder)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>forLoopFinder (arr, name)](#apidoc.element.react-monocle.reactParser.forLoopFinder)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getES5ReactComponents (ast)](#apidoc.element.react-monocle.reactParser.getES5ReactComponents)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getES6ReactComponents (ast)](#apidoc.element.react-monocle.reactParser.getES6ReactComponents)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getStatelessFunctionalComponents (ast, name)](#apidoc.element.react-monocle.reactParser.getStatelessFunctionalComponents)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>higherOrderFunctionFinder (arr, name)](#apidoc.element.react-monocle.reactParser.higherOrderFunctionFinder)
1.  [function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>jsToAst (js)](#apidoc.element.react-monocle.reactParser.jsToAst)

#### [module react-monocle.stringRegexHelper](#apidoc.module.react-monocle.stringRegexHelper)
1.  [function <span class="apidocSignatureSpan">react-monocle.stringRegexHelper.</span>regexIndexOf (string, regex, startpos)](#apidoc.element.react-monocle.stringRegexHelper.regexIndexOf)
1.  [function <span class="apidocSignatureSpan">react-monocle.stringRegexHelper.</span>regexLastIndexOf (string, regex, startpos)](#apidoc.element.react-monocle.stringRegexHelper.regexLastIndexOf)



# <a name="apidoc.module.react-monocle"></a>[module react-monocle](#apidoc.module.react-monocle)

#### <a name="apidoc.element.react-monocle.esquery"></a>[function <span class="apidocSignatureSpan">react-monocle.</span>esquery (ast, selector)](#apidoc.element.react-monocle.esquery)
- description and source-code
```javascript
function query(ast, selector) {
    return match(ast, parse(selector));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-monocle.esquery"></a>[module react-monocle.esquery](#apidoc.module.react-monocle.esquery)

#### <a name="apidoc.element.react-monocle.esquery.esquery"></a>[function <span class="apidocSignatureSpan">react-monocle.</span>esquery (ast, selector)](#apidoc.element.react-monocle.esquery.esquery)
- description and source-code
```javascript
function query(ast, selector) {
    return match(ast, parse(selector));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.esquery.match"></a>[function <span class="apidocSignatureSpan">react-monocle.esquery.</span>match (ast, selector)](#apidoc.element.react-monocle.esquery.match)
- description and source-code
```javascript
function match(ast, selector) {
    var ancestry = [], results = [], altSubjects, i, l, k, m;
    if (!selector) { return results; }
    altSubjects = subjects(selector);
    estraverse.traverse(ast, {
        enter: function (node, parent) {
            if (parent != null) { ancestry.unshift(parent); }
            if (matches(node, selector, ancestry)) {
                if (altSubjects.length) {
                    for (i = 0, l = altSubjects.length; i < l; ++i) {
                        if (matches(node, altSubjects[i], ancestry)) { results.push(node); }
                        for (k = 0, m = ancestry.length; k < m; ++k) {
                            if (matches(ancestry[k], altSubjects[i], ancestry.slice(k + 1))) {
                                results.push(ancestry[k]);
                            }
                        }
                    }
                } else {+
                    results.push(node);
                }
            }
        },
        leave: function () { ancestry.shift(); }
    });
    return results;
}
```
- example usage
```shell
...
result.css = findCSS(stringed, path.replace(/\/.*?\.html/, '').replace(/\/?.*?\.html/, ''));

return result;
}

function findCSS(str, relPath) {
if (relPath !== '') relPath = relPath + '/';
const styleTags = str.match(/<style>(\n|.)*?(<\/style>)/g) || [''];
const cssLinks = str.match(/<link.*?css.*?>/g);
if (!cssLinks && !styleTags) return [];
if (!cssLinks) return styleTags;
return cssLinks.map(ele => {
  if (!ele) return;
  if (ele.search(/http/) !== -1) return ele;
  if (ele.search(/href(\s?)=(\s?)(\\?)('|")\/{2}/)) {
...
```

#### <a name="apidoc.element.react-monocle.esquery.matches"></a>[function <span class="apidocSignatureSpan">react-monocle.esquery.</span>matches (node, selector, ancestry)](#apidoc.element.react-monocle.esquery.matches)
- description and source-code
```javascript
function matches(node, selector, ancestry) {
    var path, ancestor, i, l, p;
    if (!selector) { return true; }
    if (!node) { return false; }
    if (!ancestry) { ancestry = []; }

    switch(selector.type) {
        case 'wildcard':
            return true;

        case 'identifier':
            return selector.value.toLowerCase() === node.type.toLowerCase();

        case 'field':
            path = selector.name.split('.');
            ancestor = ancestry[path.length - 1];
            return inPath(node, ancestor, path);

        case 'matches':
            for (i = 0, l = selector.selectors.length; i < l; ++i) {
                if (matches(node, selector.selectors[i], ancestry)) { return true; }
            }
            return false;

        case 'compound':
            for (i = 0, l = selector.selectors.length; i < l; ++i) {
                if (!matches(node, selector.selectors[i], ancestry)) { return false; }
            }
            return true;

        case 'not':
            for (i = 0, l = selector.selectors.length; i < l; ++i) {
                if (matches(node, selector.selectors[i], ancestry)) { return false; }
            }
            return true;

        case 'child':
            if (matches(node, selector.right, ancestry)) {
                return matches(ancestry[0], selector.left, ancestry.slice(1));
            }
            return false;

        case 'descendant':
            if (matches(node, selector.right, ancestry)) {
                for (i = 0, l = ancestry.length; i < l; ++i) {
                    if (matches(ancestry[i], selector.left, ancestry.slice(i + 1))) {
                        return true;
                    }
                }
            }
            return false;

        case 'attribute':
            p = getPath(node, selector.name);
            switch (selector.operator) {
                case null:
                case void 0:
                    return p != null;
                case '=':
                    switch (selector.value.type) {
                        case 'regexp': return selector.value.value.test(p);
                        case 'literal': return '' + selector.value.value === '' + p;
                        case 'type': return selector.value.value === typeof p;
                    }
                case '!=':
                    switch (selector.value.type) {
                        case 'regexp': return !selector.value.value.test(p);
                        case 'literal': return '' + selector.value.value !== '' + p;
                        case 'type': return selector.value.value !== typeof p;
                    }
                case '<=': return p <= selector.value.value;
                case '<': return p < selector.value.value;
                case '>': return p > selector.value.value;
                case '>=': return p >= selector.value.value;
            }

        case 'sibling':
            return matches(node, selector.right, ancestry) &&
                sibling(node, selector.left, ancestry) ||
                matches(node, selector.left, ancestry) &&
                sibling(node, selector.right, ancestry);

        case 'adjacent':
            return matches(node, selector.right, ancestry) &&
                adjacent(node, selector.left, ancestry) ||
                matches(node, selector.left, ancestry) &&
                adjacent(node, selector.right, ancestry);

        case 'nth-child':
            return matches(node, selector.right, ancestry) &&
                nthChild(node, ancestry, function (length) {
                    return selector.index.value - 1;
                });

        case 'nth-last-child':
            return matches(node, selector.right, ancestry) &&
                nthChild(node, ancestry, function (length) {
                    return length - selector.index.value;
                });

        case 'class':
            if(!node.type) return false;
            switch(selector.name.toLowerCase()){
                case 'statement':
                    if(node.type.slice(-9) === 'Statement') return true; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.esquery.parse"></a>[function <span class="apidocSignatureSpan">react-monocle.esquery.</span>parse (selector)](#apidoc.element.react-monocle.esquery.parse)
- description and source-code
```javascript
function parse(selector) {
    return parser.parse(selector);
}
```
- example usage
```shell
...
    return results;
}

/**
 * Parse a selector string and return its AST.
 */
function parse(selector) {
    return parser.parse(selector);
}

/**
 * Query the code AST using the selector string.
 */
function query(ast, selector) {
    return match(ast, parse(selector));
...
```

#### <a name="apidoc.element.react-monocle.esquery.query"></a>[function <span class="apidocSignatureSpan">react-monocle.esquery.</span>query (ast, selector)](#apidoc.element.react-monocle.esquery.query)
- description and source-code
```javascript
function query(ast, selector) {
    return match(ast, parse(selector));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-monocle.esrecurse"></a>[module react-monocle.esrecurse](#apidoc.module.react-monocle.esrecurse)

#### <a name="apidoc.element.react-monocle.esrecurse.Visitor"></a>[function <span class="apidocSignatureSpan">react-monocle.esrecurse.</span>Visitor (visitor, options)](#apidoc.element.react-monocle.esrecurse.Visitor)
- description and source-code
```javascript
function Visitor(visitor, options) {
    options = options || {};

    this.__visitor = visitor ||  this;
    this.__childVisitorKeys = options.childVisitorKeys
        ? assign({}, estraverse.VisitorKeys, options.childVisitorKeys)
        : estraverse.VisitorKeys;
    if (options.fallback === 'iteration') {
        this.__fallback = objectKeys;
    } else if (typeof options.fallback === 'function') {
        this.__fallback = options.fallback;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.esrecurse.visit"></a>[function <span class="apidocSignatureSpan">react-monocle.esrecurse.</span>visit (node, visitor, options)](#apidoc.element.react-monocle.esrecurse.visit)
- description and source-code
```javascript
visit = function (node, visitor, options) {
    var v = new Visitor(visitor, options);
    v.visit(node);
}
```
- example usage
```shell
...
        for (i = 0, iz = children.length; i < iz; ++i) {
child = node[children[i]];
if (child) {
    if (isArray(child)) {
        for (j = 0, jz = child.length; j < jz; ++j) {
            if (child[j]) {
                if (isNode(child[j]) || isProperty(type, children[i])) {
                    this.visit(child[j]);
                }
            }
        }
    } else if (isNode(child)) {
        this.visit(child);
    }
}
...
```



# <a name="apidoc.module.react-monocle.estraverse"></a>[module react-monocle.estraverse](#apidoc.module.react-monocle.estraverse)

#### <a name="apidoc.element.react-monocle.estraverse.Controller"></a>[function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>Controller ()](#apidoc.element.react-monocle.estraverse.Controller)
- description and source-code
```javascript
function Controller() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.estraverse.attachComments"></a>[function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>attachComments (tree, providedComments, tokens)](#apidoc.element.react-monocle.estraverse.attachComments)
- description and source-code
```javascript
function attachComments(tree, providedComments, tokens) {
      // At first, we should calculate extended comment ranges.
  var comments = [], comment, len, i, cursor;

  if (!tree.range) {
    throw new Error('attachComments needs range information');
  }

      // tokens array is empty, we attach comments to tree as 'leadingComments'
  if (!tokens.length) {
    if (providedComments.length) {
      for (i = 0, len = providedComments.length; i < len; i += 1) {
          comment = deepCopy(providedComments[i]);
          comment.extendedRange = [0, tree.range[0]];
          comments.push(comment);
        }
      tree.leadingComments = comments;
    }
    return tree;
  }

  for (i = 0, len = providedComments.length; i < len; i += 1) {
    comments.push(extendCommentRange(deepCopy(providedComments[i]), tokens));
  }

      // This is based on John Freeman's implementation.
  cursor = 0;
  traverse(tree, {
    enter(node) {
      var comment;

      while (cursor < comments.length) {
          comment = comments[cursor];
          if (comment.extendedRange[1] > node.range[0]) {
              break;
            }

          if (comment.extendedRange[1] === node.range[0]) {
              if (!node.leadingComments) {
                  node.leadingComments = [];
                }
              node.leadingComments.push(comment);
              comments.splice(cursor, 1);
            } else {
              cursor += 1;
            }
        }

              // already out of owned node
      if (cursor === comments.length) {
          return VisitorOption.Break;
        }

      if (comments[cursor].extendedRange[0] > node.range[1]) {
          return VisitorOption.Skip;
        }
    },
  });

  cursor = 0;
  traverse(tree, {
    leave(node) {
      var comment;

      while (cursor < comments.length) {
          comment = comments[cursor];
          if (node.range[1] < comment.extendedRange[0]) {
              break;
            }

          if (node.range[1] === comment.extendedRange[0]) {
              if (!node.trailingComments) {
                  node.trailingComments = [];
                }
              node.trailingComments.push(comment);
              comments.splice(cursor, 1);
            } else {
              cursor += 1;
            }
        }

              // already out of owned node
      if (cursor === comments.length) {
          return VisitorOption.Break;
        }

      if (comments[cursor].extendedRange[0] > node.range[1]) {
          return VisitorOption.Skip;
        }
    },
  });

  return tree;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.estraverse.cloneEnvironment"></a>[function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>cloneEnvironment ()](#apidoc.element.react-monocle.estraverse.cloneEnvironment)
- description and source-code
```javascript
cloneEnvironment = function () { return clone({}); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.estraverse.replace"></a>[function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>replace (root, visitor)](#apidoc.element.react-monocle.estraverse.replace)
- description and source-code
```javascript
function replace(root, visitor) {
  var controller = new Controller();
  return controller.replace(root, visitor);
}
```
- example usage
```shell
...
* Any character may appear in the form of an escape sequence.
*
* For portability, we also escape escape all control and non-ASCII
* characters. Note that "\0" and "\v" escape sequences are not used
* because JSHint does not like the first and IE the second.
*/
return '"' + s
 .replace(/\\/g, '\\\\')  // backslash
 .replace(/"/g, '\\"')    // closing quote character
 .replace(/\x08/g, '\\b') // backspace
 .replace(/\t/g, '\\t')   // horizontal tab
 .replace(/\n/g, '\\n')   // line feed
 .replace(/\f/g, '\\f')   // form feed
 .replace(/\r/g, '\\r')   // carriage return
 .replace(/[\x00-\x07\x0B\x0E-\x1F\x80-\uFFFF]/g, escape)
...
```

#### <a name="apidoc.element.react-monocle.estraverse.traverse"></a>[function <span class="apidocSignatureSpan">react-monocle.estraverse.</span>traverse (root, visitor)](#apidoc.element.react-monocle.estraverse.traverse)
- description and source-code
```javascript
function traverse(root, visitor) {
  var controller = new Controller();
  return controller.traverse(root, visitor);
}
```
- example usage
```shell
...
/**
 * From a JS AST and a selector AST, collect all JS AST nodes that match the selector.
 */
function match(ast, selector) {
    var ancestry = [], results = [], altSubjects, i, l, k, m;
    if (!selector) { return results; }
    altSubjects = subjects(selector);
    estraverse.traverse(ast, {
        enter: function (node, parent) {
            if (parent != null) { ancestry.unshift(parent); }
            if (matches(node, selector, ancestry)) {
                if (altSubjects.length) {
                    for (i = 0, l = altSubjects.length; i < l; ++i) {
                        if (matches(node, altSubjects[i], ancestry)) { results.push(node); }
                        for (k = 0, m = ancestry.length; k < m; ++k) {
...
```



# <a name="apidoc.module.react-monocle.parser"></a>[module react-monocle.parser](#apidoc.module.react-monocle.parser)

#### <a name="apidoc.element.react-monocle.parser.SyntaxError"></a>[function <span class="apidocSignatureSpan">react-monocle.parser.</span>SyntaxError (expected, found, offset, line, column)](#apidoc.element.react-monocle.parser.SyntaxError)
- description and source-code
```javascript
SyntaxError = function (expected, found, offset, line, column) {
  function buildMessage(expected, found) {
    var expectedHumanized, foundHumanized;

    switch (expected.length) {
      case 0:
        expectedHumanized = "end of input";
        break;
      case 1:
        expectedHumanized = expected[0];
        break;
      default:
        expectedHumanized = expected.slice(0, expected.length - 1).join(", ")
          + " or "
          + expected[expected.length - 1];
    }

    foundHumanized = found ? quote(found) : "end of input";

    return "Expected " + expectedHumanized + " but " + foundHumanized + " found.";
  }

  this.name = "SyntaxError";
  this.expected = expected;
  this.found = found;
  this.message = buildMessage(expected, found);
  this.offset = offset;
  this.line = line;
  this.column = column;
}
```
- example usage
```shell
...
 * handle these states.
 */
if (result === null || pos !== input.length) {
  var offset = Math.max(pos, rightmostFailuresPos);
  var found = offset < input.length ? input.charAt(offset) : null;
  var errorPosition = computeErrorPosition();

  throw new this.SyntaxError(
    cleanupExpected(rightmostFailuresExpected),
    found,
    offset,
    errorPosition.line,
    errorPosition.column
  );
}
...
```

#### <a name="apidoc.element.react-monocle.parser.parse"></a>[function <span class="apidocSignatureSpan">react-monocle.parser.</span>parse (input, startRule)](#apidoc.element.react-monocle.parser.parse)
- description and source-code
```javascript
parse = function (input, startRule) {
  var parseFunctions = {
    "start": parse_start,
    "_": parse__,
    "identifierName": parse_identifierName,
    "binaryOp": parse_binaryOp,
    "selectors": parse_selectors,
    "selector": parse_selector,
    "sequence": parse_sequence,
    "atom": parse_atom,
    "wildcard": parse_wildcard,
    "identifier": parse_identifier,
    "attr": parse_attr,
    "attrOps": parse_attrOps,
    "attrEqOps": parse_attrEqOps,
    "attrName": parse_attrName,
    "attrValue": parse_attrValue,
    "string": parse_string,
    "number": parse_number,
    "path": parse_path,
    "type": parse_type,
    "regex": parse_regex,
    "field": parse_field,
    "negation": parse_negation,
    "matches": parse_matches,
    "firstChild": parse_firstChild,
    "lastChild": parse_lastChild,
    "nthChild": parse_nthChild,
    "nthLastChild": parse_nthLastChild,
    "class": parse_class
  };

  if (startRule !== undefined) {
    if (parseFunctions[startRule] === undefined) {
      throw new Error("Invalid rule name: " + quote(startRule) + ".");
    }
  } else {
    startRule = "start";
  }

  var pos = 0;
  var reportFailures = 0;
  var rightmostFailuresPos = 0;
  var rightmostFailuresExpected = [];
  var cache = {};

  function padLeft(input, padding, length) {
    var result = input;

    var padLength = length - input.length;
    for (var i = 0; i < padLength; i++) {
      result = padding + result;
    }

    return result;
  }

  function escape(ch) {
    var charCode = ch.charCodeAt(0);
    var escapeChar;
    var length;

    if (charCode <= 0xFF) {
      escapeChar = 'x';
      length = 2;
    } else {
      escapeChar = 'u';
      length = 4;
    }

    return '\\' + escapeChar + padLeft(charCode.toString(16).toUpperCase(), '0', length);
  }

  function matchFailed(failure) {
    if (pos < rightmostFailuresPos) {
      return;
    }

    if (pos > rightmostFailuresPos) {
      rightmostFailuresPos = pos;
      rightmostFailuresExpected = [];
    }

    rightmostFailuresExpected.push(failure);
  }

  function parse_start() {
    var cacheKey = "start@" + pos;
    var cachedResult = cache[cacheKey];
    if (cachedResult) {
      pos = cachedResult.nextPos;
      return cachedResult.result;
    }

    var result0, result1, result2;
    var pos0, pos1;

    pos0 = pos;
    pos1 = pos;
    result0 = parse__();
    if (result0 !== null) {
      result1 = parse_selectors();
      if (result1 !== null) {
        result2 = parse__();
        if (result2 !== null) {
          result0 = [result0, result1, result2];
        } else {
          result0 = null;
          pos = pos1;
        }
      } else {
        result0 = null;
        pos = pos1;
      }
    } else {
      result0 = null;
      pos = pos1;
    }
    if (result0 !== null) {
      result0 = (function(offset, ss) { return ss.length === 1 ? ss[0] : { type: 'matches', selectors: ss }; })(pos0, result0[1]);
    }
    if (result0 === null) {
      pos = pos0;
    }
    if (result0 === null) {
      pos0 = pos;
      result0 = parse__();
      if (result0 !== null) {
        result0 = (function(offset) { return void 0; })(pos0);
      }
      if (result0 === null) {
        pos = pos0;
      }
    }

    cache[cacheKey] = {
      nextPos: pos,
      result:  result0
    };
    return result0;
  }

  function parse__() {
    var cacheKey = "_@" + pos;
    var cachedResult = cache[cacheKey];
    if (cachedResult) {
      pos = cachedResult.nextPos;
      return cachedResult.result;
    }

    var result0, result1;

    result0 = [];
    if (input.charCodeAt(pos) === 32) {
      result1 = " ";
      pos++;
    } else {
      result1 = null;
      if (reportFailures === 0) {
        matchFailed("\" \"");
      }
    }
    while (result1 !== null) {
      result0.push(result1);
      if (input.charCodeAt(pos) === 32) {
        result1 = " ";
        pos++;
      } else {
        result1 = null;
        if (reportFailures === 0) {
          matchFailed("\" \"");
        }
      }
    }

    cache[cacheKey ...
```
- example usage
```shell
...
    return results;
}

/**
 * Parse a selector string and return its AST.
 */
function parse(selector) {
    return parser.parse(selector);
}

/**
 * Query the code AST using the selector string.
 */
function query(ast, selector) {
    return match(ast, parse(selector));
...
```

#### <a name="apidoc.element.react-monocle.parser.toSource"></a>[function <span class="apidocSignatureSpan">react-monocle.parser.</span>toSource ()](#apidoc.element.react-monocle.parser.toSource)
- description and source-code
```javascript
toSource = function () { return this._source; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-monocle.previewParser"></a>[module react-monocle.previewParser](#apidoc.module.react-monocle.previewParser)

#### <a name="apidoc.element.react-monocle.previewParser.getComponentName"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>getComponentName (bundle, startingIndex)](#apidoc.element.react-monocle.previewParser.getComponentName)
- description and source-code
```javascript
function getComponentName(bundle, startingIndex) {
  let bundleSearchIndicesMap = {};
  // get index of component declaration
  bundleSearchIndicesMap[regexLastIndexOf(bundle, /(var )?\w+\s*?=\s*(\(\d+\, )?_react(\d+\[\"\w+\"\])?.createClass/, startingIndex
)] = 'WEBPACKES5';
  // let's try ES6...
  bundleSearchIndicesMap[regexLastIndexOf(bundle, /(var )?\w+\s*?=\s*?function\s*?\(_(React\$)?Component\)/, startingIndex)] = '
WEBPACKES6';
  // let's try GULP
  bundleSearchIndicesMap[regexLastIndexOf(bundle, /var \w+ = React.createClass\({/, startingIndex)] = 'GULP';
  // let's try Rollup ex: var Slick = (function (superclass) {
  bundleSearchIndicesMap[regexLastIndexOf(bundle, /var \w+ = \(function \(superclass\) {/, startingIndex)] = 'ROLLUP';
  const targetIndex = Object.keys(bundleSearchIndicesMap)
  	.filter(index => index >= 0)
  	.reduce((prev, curr) => {
  	  return Math.abs(curr-startingIndex) < Math.abs(prev-startingIndex)
  	  	? curr
  	  	: prev;
  	});

  let componentMatch;
  switch(bundleSearchIndicesMap[targetIndex]) {
  	case 'WEBPACKES5':
  	  componentMatch = bundle.slice(targetIndex)
  	  	.match(/(var )?\w+\s*?=\s*(\(\d+\, )?_react(\d+\[\"\w+\"\])?.createClass/)
  	  break;
    case 'WEBPACKES6':
   	  componentMatch = bundle.slice(targetIndex)
  	    .match(/(var )?\w+\s*?=\s*?function\s*?\(_(React\$)?Component\)/)
   	  break;
    case 'GULP':
      componentMatch = bundle.slice(targetIndex)
        .match(/var \w+ = React.createClass\({/)
      break;
    case 'ROLLUP':
      componentMatch = bundle.slice(targetIndex)
        .match(/var \w+ = \(function \(superclass\) {/)
      break;
    default:
    	throw new Error('Unable to find component from bundle file');
  }

  // need to normalize component name (remove declarator ex. var, const)
  return componentMatch[0]
    .replace(/var |const /, '')
    .replace(/ /g, '')
    .split('=')[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.getDivs"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>getDivs (modifiedBundle)](#apidoc.element.react-monocle.previewParser.getDivs)
- description and source-code
```javascript
function getDivs(modifiedBundle) {
  let index = modifiedBundle.indexOf('getElementById(', 0);
  let divsArr = [];
  while (index !== -1) {
    let openParenIdx = modifiedBundle.indexOf('(', index - 1);
    let currentIdx = openParenIdx + 1;
    const parensStack = ['('];
    while (parensStack.length !== 0) {
      if (modifiedBundle[currentIdx] === '(') parensStack.push(modifiedBundle[currentIdx]);
      if (modifiedBundle[currentIdx] === ')') parensStack.pop();
      currentIdx++;
    }
    divsArr.push(modifiedBundle.slice(openParenIdx + 2, currentIdx - 2));
    index = modifiedBundle.indexOf('getElementById(', index + 1);
  }
  divsArr = divsArr.map(ele => {
    return '<div id='${ele}'></div>';
  });
  const uniqueArr = [];
  for (let i = 0; i < divsArr.length; i++) {
    if (uniqueArr.indexOf(divsArr[i]) < 0) {
      uniqueArr.push(divsArr[i]);
    }
  }
  return uniqueArr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.modifyBundleFile"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyBundleFile (bundlejs)](#apidoc.element.react-monocle.previewParser.modifyBundleFile)
- description and source-code
```javascript
function modifyBundleFile(bundlejs) {
  const bundle = fs.readFileSync(bundlejs, { encoding: 'utf-8' });
  if (bundle.length === 0) throw new Error('Empty AST input');
  const searchState = /this.setState/g;
  const wrappedFunc = 'wrapper(this.setState)';
  const searchElem = /(getElementById\([\'\"])\w+[\'\"]/;
  const newMount = 'getElementById("preview"';
  const replacedState = bundle.replace(searchState, wrappedFunc);
  return replacedState.replace(searchElem, newMount);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.modifyInitialState"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyInitialState (modifiedBundle)](#apidoc.element.react-monocle.previewParser.modifyInitialState)
- description and source-code
```javascript
function modifyInitialState(modifiedBundle) {
  let index = -1;
  if (modifiedBundle.indexOf('_this.state') >= 0) {
    // do webpack
    index = modifiedBundle.indexOf('_this.state', 0);
  } else if (modifiedBundle.indexOf('getInitialState() {', 0) >= 0) {
    // do gulp
    index = modifiedBundle.indexOf('getInitialState() {', 0) + 19;
  } else if (modifiedBundle.indexOf('this.state', 0) >= 0) {
    // do rollup
    index = modifiedBundle.indexOf('this.state = {');
  } else {
    throw new Error('Unable to find component initial state');
  }

  while (index !== -1) {
    let openBraceIdx = modifiedBundle.indexOf('{', index); // looking for index of follow brace, after return statement
    let currentIdx = openBraceIdx + 1;
    const parensStack = ['{'];
    while (parensStack.length !== 0) {
      if (modifiedBundle[currentIdx] === '{') parensStack.push(modifiedBundle[currentIdx]);
      if (modifiedBundle[currentIdx] === '}') parensStack.pop();
      currentIdx++;
    }

    let injection,
        componentName = getComponentName(modifiedBundle, index),
        stateStr = modifiedBundle.slice(openBraceIdx, currentIdx);
    if (modifiedBundle.indexOf('_this.state', 0) >= 0) {
      injection = '_this.state = grabInitialState('${componentName}', ${stateStr}),';
    } else if (modifiedBundle.indexOf('getInitialState() {', 0) >= 0) {
      injection = 'return grabInitialState('${componentName}', ${stateStr}),';
    } else if (modifiedBundle.indexOf('this.state = {', 0) >= 0) {
      injection = 'this.state = grabInitialState('${componentName}', ${stateStr}),';
    }

    modifiedBundle = modifiedBundle.slice(0, index) + injection + modifiedBundle.slice(currentIdx + 1);

    // need to take into account that length of bundle now changes since injected wrapper string length can be different than original
    const oldLength = currentIdx - index;
    const newLength = injection.length;

    if (modifiedBundle.indexOf('_this.state') >= 0) {
      index = modifiedBundle.indexOf('_this.state', index + 1 + newLength - oldLength);
    } else if (modifiedBundle.indexOf('getInitialState() {') >= 0) {
      index = modifiedBundle.indexOf('getInitialState() {', index + 1 + newLength - oldLength);
    } else if (modifiedBundle.indexOf('this.state = grabInitialState') >= 0) {
      index = modifiedBundle.indexOf('this.state = grabInitialState', index + 1 + newLength - oldLength);
    } else {
      throw new Error('Unable to find next initial state index');
    }
  }
  return modifiedBundle;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.modifySetStateStrings"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifySetStateStrings (bundleFilePath)](#apidoc.element.react-monocle.previewParser.modifySetStateStrings)
- description and source-code
```javascript
function modifySetStateStrings(bundleFilePath) {
  let bundle;
  try {
    bundle = fs.readFileSync(bundleFilePath, { encoding: 'utf-8' });
  } catch(error) {
    throw new Error('Invalid bundle file path specified. Please enter a valid path to your app\'s bundle file');
  }

  if (bundle.length == 0) throw new Error('Bundle string is empty, provide valid bundle string input');

  console.log('Starting to strip comments from bundle file...');
  const start = Date.now();
  let modifiedBundle = strip(bundle.slice());
  console.log('Took ${(Date.now() - start) / 1000} seconds to strip comments input bundle file');
  let index = modifiedBundle.indexOf('this.setState', 0);
  while (index !== -1) {
    let openBraceIdx = modifiedBundle.indexOf('{', index);
    let currentIdx = openBraceIdx + 1;
    const parensStack = ['{'];
    while (parensStack.length !== 0) {
      if (modifiedBundle[currentIdx] === '{') parensStack.push(modifiedBundle[currentIdx]);
      if (modifiedBundle[currentIdx] === '}') parensStack.pop();
      currentIdx++;
    }
    const stateStr = modifiedBundle.slice(openBraceIdx, currentIdx);
    const functionStartIdx = currentIdx;
    parensStack.push('(');
    while (parensStack.length !== 0) {
      if (modifiedBundle[currentIdx] === '(') parensStack.push(modifiedBundle[currentIdx]);
      if (modifiedBundle[currentIdx] === ')') parensStack.pop();
      currentIdx++;
    }
    currentIdx--;
    const callbackStr = modifiedBundle.slice(functionStartIdx, currentIdx);
    const injection = 'wrapper('${getComponentName(modifiedBundle, index)}',this)(${ stateStr }${ callbackStr })';
    modifiedBundle = modifiedBundle.slice(0, index) + injection + modifiedBundle.slice(currentIdx + 1);
    // need to take into account that length of bundle now changes since injected wrapper string length can be different than original
    const oldLength = currentIdx - index;
    const newLength = injection.length;

    index = modifiedBundle.indexOf('this.setState', index+1+newLength-oldLength);
  }
  return modifiedBundle;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.modifyTestBundleFile"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>modifyTestBundleFile (bundle)](#apidoc.element.react-monocle.previewParser.modifyTestBundleFile)
- description and source-code
```javascript
function modifyTestBundleFile(bundle) {
  if (bundle.length === 0) throw new Error('Empty AST input');
  const searchState = /this.setState/g;
  const wrappedFunc = 'wrapper(this.setState)';
  const searchElem = /(getElementById\([\'\"])\w+[\'\"]/;
  const newMount = 'getElementById("preview"';
  const replacedState = bundle.replace(searchState, wrappedFunc);
  return replacedState.replace(searchElem, newMount);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.queryES5Ast"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>queryES5Ast (bundlejs)](#apidoc.element.react-monocle.previewParser.queryES5Ast)
- description and source-code
```javascript
function queryES5Ast(bundlejs) {
  if (!bundlejs) throw new Error('Empty bundle file input');
  const bundle = fs.readFileSync(bundlejs, { encoding: 'utf-8' });
  const ast = acorn.parse(bundle);
  if (ast.body.length === 0) throw new Error('Empty AST input');
  const parseInfo = esquery.parse('[id.name="getInitialState"]');
  const match = esquery.match(ast, parseInfo);
  const finalStateArr = [];
  if (match.length === 0) return {};
  match.map(ele => {
    const valueObj = {};
    ele.body.body.map(index => {
      if (index.type === 'ReturnStatement') {
        index.argument.properties.map(node => {
          if (node.value.hasOwnProperty('value')) {
            valueObj[node.key.name] = node.value.value;
          } else if (node.value.hasOwnProperty('name')) {
            valueObj[node.key.name] = node.value.name;
          } else if (node.value.hasOwnProperty('elements')) {
            valueObj[node.key.name] = node.value.elements;
          }
        });
        finalStateArr.push(valueObj);
      }
    });
  });
  return structureInitialES5StateObj(bundlejs, finalStateArr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.queryES6Ast"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>queryES6Ast (bundlejs)](#apidoc.element.react-monocle.previewParser.queryES6Ast)
- description and source-code
```javascript
function queryES6Ast(bundlejs) {
  if (!bundlejs) throw new Error('Empty bundle file input');
  const bundle = fs.readFileSync(bundlejs, { encoding: 'utf-8' });
  const ast = acorn.parse(bundle);
  if (ast.body.length === 0) throw new Error('Empty AST input');
  const parseInfo = esquery.parse('ExpressionStatement');
  const match = esquery.match(ast, parseInfo);
  const finalStateArr = [];
  if (match.length === 0) return {};
  match.map(ele => {
    const valueObj = {};
    if (ele.expression.left) {
      if (ele.expression.left.object) {
        if (ele.expression.left.object.name === '_this') {
          const valueNode = ele.expression.right.properties;
          valueNode.map(node => {
            const finalValArr = [];
            if (node.value.elements) {
              node.value.elements.map(index => {
                finalValArr.push(index.value);
              });
            }
            valueObj[node.key.name] = node.value.value || finalValArr;
          });
          finalStateArr.push(valueObj);
        }
      }
    }
  });
  return structureInitialES6StateObj(bundle, finalStateArr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.structureInitialES5StateObj"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>structureInitialES5StateObj (bundle, arr)](#apidoc.element.react-monocle.previewParser.structureInitialES5StateObj)
- description and source-code
```javascript
function structureInitialES5StateObj(bundle, arr) {
  if (arr.length === 0) return {};
  let initialStateIndex = bundle.indexOf('getInitialState()', 0);
  const objForReduxStore = {};
  for (let i = 0; i < arr.length; i++) {
    const arrOfStateObjs = [];
    for (const key in arr[i]) {
      arrOfStateObjs.push({
        name: key,
        value: arr[i][key],
      });
      objForReduxStore[getComponentName(bundle, initialStateIndex)] = arrOfStateObjs;
    }
    initialStateIndex = bundle.indexOf('getInitialState()', initialStateIndex + 1);
  }
  return objForReduxStore;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.previewParser.structureInitialES6StateObj"></a>[function <span class="apidocSignatureSpan">react-monocle.previewParser.</span>structureInitialES6StateObj (bundle, arr)](#apidoc.element.react-monocle.previewParser.structureInitialES6StateObj)
- description and source-code
```javascript
function structureInitialES6StateObj(bundle, arr) {
  if (arr.length === 0) return {};
  let initialStateIndex = bundle.indexOf('_this.state', 0);
  const objForReduxStore = {};
  for (let i = 0; i < arr.length; i++) {
    const arrOfStateObjs = [];
    for (const key in arr[i]) {
      arrOfStateObjs.push({
        name: key,
        value: arr[i][key],
      });
      objForReduxStore[getComponentName(bundle, initialStateIndex)] = arrOfStateObjs;
    }
    initialStateIndex = bundle.indexOf('_this.state', initialStateIndex + 1);
  }
  return objForReduxStore;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-monocle.reactParser"></a>[module react-monocle.reactParser](#apidoc.module.react-monocle.reactParser)

#### <a name="apidoc.element.react-monocle.reactParser.componentChecker"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>componentChecker (ast)](#apidoc.element.react-monocle.reactParser.componentChecker)
- description and source-code
```javascript
function componentChecker(ast) {
  for (let i = 0; i < ast.body.length; i++) {
    if (ast.body[i].type === 'ClassDeclaration') return 'ES6';
    if (ast.body[i].type === 'ExportDefaultDeclaration' && ast.body[i].declaration.type === 'ClassDeclaration') return 'ES6';
    if (ast.body[i].type === 'VariableDeclaration' && ast.body[i].declarations[0].init
     && ast.body[i].declarations[0].init.callee
    && ast.body[i].declarations[0].init.callee.object && ast.body[i].declarations[0].init.callee.object.name === 'React'
    && ast.body[i].declarations[0].init.callee.property.name === 'createClass') return 'ES5'
  }
  return 'SFC';
}
```
- example usage
```shell
...
function d3DataBuilder(obj) {
if (!obj.ENTRY) throw new Error('Entry component not found');
const formatted = {};

// parsing AST into formatted objects based on ES5/ES6 syntax
for (const key in obj) {
  if (key === 'ENTRY') continue;
  const componentChecker = reactParser.componentChecker(obj[key]);
  // componentChecker returns true for es6 classes, false for everything else
  if (componentChecker === 'ES6') formatted[key] = reactParser.getES6ReactComponents(obj[key]);
  else if (componentChecker === 'ES5') formatted[key] = reactParser.getES5ReactComponents(obj[key]);
  else formatted[key] = reactParser.getStatelessFunctionalComponents(obj[key], key)
}

for (const key in formatted) {
...
```

#### <a name="apidoc.element.react-monocle.reactParser.forInFinder"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>forInFinder (arr, name)](#apidoc.element.react-monocle.reactParser.forInFinder)
- description and source-code
```javascript
function forInFinder(arr, name) {
  const result = arr.map(ele => {
    const jsxnode = esquery(ele, 'JSXElement')[0];
    const obj = {};
    obj.variables = {};
    esquery(ele, 'VariableDeclarator').forEach(vars => {
      if (vars.id.name !== 'i' && vars.init) {
        obj.variables[vars.id.name] = escodegen.generate(vars.init).replace('this.', '');
      }
    });
    if (ele.left.declarations) obj.variables[ele.left.declarations[0].id.name] = '[key]';
    else if (ele.left.type === 'Identifier') obj.variables[ele.left.name] = '[key]';

    if (jsxnode && htmlElements.indexOf(jsxnode.openingElement.name.name)) {
      let current = ele.right;
      let found;
      while (current && current.property) {
        found = '.${current.property.name}${found || ''}';
        current = current.object;
        if (current.type === 'Identifier') {
          found = '.${current.name}${found || ''}';
          break;
        }
      }

      obj.jsx = {
        name: jsxnode.openingElement.name.name,
        children: getChildJSXElements(jsxnode, name),
        props: getReactProps(jsxnode, name),
        state: {},
        methods: [],
        iterated: 'forIn',
        source: found.replace('.', ''),
      };
      const propsArr = obj.jsx.props;
      for (let i = 0; i < propsArr.length; i++) {
        for (const key in obj.variables) {
          if (propsArr[i].value.includes(key)) {
            if (obj.variables[key] === '[key]') propsArr[i].value = propsArr[i].value.replace('.${key}', obj.variables[key]);
            else propsArr[i].value = propsArr[i].value.replace(key, obj.variables[key]);
          }
        }
      }
    }
    return obj;
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.reactParser.forLoopFinder"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>forLoopFinder (arr, name)](#apidoc.element.react-monocle.reactParser.forLoopFinder)
- description and source-code
```javascript
function forLoopFinder(arr, name) {
  const result = arr.map(ele => {
    const jsxnode = esquery(ele, 'JSXElement')[0];
    const obj = {};
    obj.variables = {};

    // finding variables in case information was reassigned
    esquery(ele, 'VariableDeclarator').forEach(vars => {
      if (vars.id.name !== 'i' && vars.init) {
        obj.variables[vars.id.name] = escodegen.generate(vars.init).replace('this.', '').replace('.length', '');
      }
    });

    // defaulting each iteration to be represented by 'i'
    if (ele.init.declarations) obj.variables[ele.init.declarations[0].id.name] = '[i]';
    else if (ele.init.type === 'AssignmentExpression') obj.variables[ele.init.left.name] = '[i]';

    // building the object name
    if (jsxnode && htmlElements.indexOf(jsxnode.openingElement.name.name)) {
      let current = ele.test.right;
      let found;
      while (current && current.property) {
        found = '.${current.property.name}${found || ''}';
        current = current.object;
        if (current.type === 'Identifier') {
          found = '.${current.name}${found || ''}';
          break;
        }
      }

      obj.jsx = {
        name: jsxnode.openingElement.name.name,
        children: getChildJSXElements(jsxnode, name),
        props: getReactProps(jsxnode, name),
        state: {},
        methods: [],
        iterated: 'forLoop',
        source: found.replace('.', '').replace('.length', ''),
      };

      // replacing variables with their properties
      const propsArr = obj.jsx.props;
      for (let i = 0; i < propsArr.length; i++) {
        for (const key in obj.variables) {
          if (propsArr[i].value.includes(key)) {
            if (obj.variables[key] === '[i]') propsArr[i].value = propsArr[i].value.replace('.${key}', obj.variables[key]);
            else propsArr[i].value = propsArr[i].value.replace(key, obj.variables[key]);
          }
        }
      }
    }
    return obj;
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.reactParser.getES5ReactComponents"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getES5ReactComponents (ast)](#apidoc.element.react-monocle.reactParser.getES5ReactComponents)
- description and source-code
```javascript
function getES5ReactComponents(ast) {
  const output = {
    name: '',
    state: {},
    props: {},
    methods: [],
    children: [],
  };
  let iter = [];
  let topJsxComponent;
  let outside;
  const checker = {};
  esrecurse.visit(ast, {
    VariableDeclarator(node) {
      topJsxComponent = node.id.name;
      this.visitChildren(node);
    },
    MemberExpression(node) {
      if (node.property && node.property.name === 'createClass') {
        output.name = topJsxComponent;
      }
      this.visitChildren(node);
    },
    ObjectExpression(node) {
      node.properties.forEach(prop => {
        if (reactMethods.indexOf(prop.key.name) < 0
          && prop.value.type === 'FunctionExpression') {
          output.methods.push(prop.key.name);
        }
      });
      this.visitChildren(node);
    },
    JSXElement(node) {
      output.children = getChildJSXElements(node, output.name);
      output.props = getReactProps(node, output.name);
      if (htmlElements.indexOf(node.openingElement.name.name) < 0) {
        outside = {
          name: node.openingElement.name.name,
          children: getChildJSXElements(node, output.name),
          props: getReactProps(node, output.name),
          state: {},
          methods: [],
        };
      }
    },
  });

  const forIn = esquery(ast, 'ForInStatement').filter(ele => {
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    return searched.length > 0;
  });
  if (forIn.length > 0) iter = iter.concat(forInFinder(forIn, output.name));

  const forLoop = esquery(ast, 'ForStatement').filter(ele => {
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    return searched.length > 0;
  });
  if (forLoop.length > 0) iter = iter.concat(forLoopFinder(forLoop, output.name));

  const higherOrderFunc = esquery(ast, 'CallExpression').filter(ele => {
    let higherOrderChecker = false;
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    if (ele.callee.property && ele.callee.property.name.match(/(map|forEach|filter|reduce)/)) {
      higherOrderChecker = ele.callee.property.name.match(/(map|forEach|filter|reduce)/);
    }
    return searched.length > 0 && higherOrderChecker;
  });
  if (higherOrderFunc.length > 0) iter = iter.concat(higherOrderFunctionFinder(higherOrderFunc, output.name));

  if (outside) output.children.push(outside);
  output.children.forEach((ele, i) => {
    checker[ele.name] = i;
  });

  for (let i = 0; i < iter.length; i++) {
    if (checker.hasOwnProperty(iter[i].jsx.name)) {
      output.children[checker[iter[i].jsx.name]] = iter[i].jsx;
    }
  }

  return output;
}
```
- example usage
```shell
...

// parsing AST into formatted objects based on ES5/ES6 syntax
for (const key in obj) {
  if (key === 'ENTRY') continue;
  const componentChecker = reactParser.componentChecker(obj[key]);
  // componentChecker returns true for es6 classes, false for everything else
  if (componentChecker === 'ES6') formatted[key] = reactParser.getES6ReactComponents(obj[key]);
  else if (componentChecker === 'ES5') formatted[key] = reactParser.getES5ReactComponents(obj[key]);
  else formatted[key] = reactParser.getStatelessFunctionalComponents(obj[key], key)
}

for (const key in formatted) {
  formatted[key].children.forEach(ele => {
    if (Array.isArray(ele.props)) {
      ele.props.forEach((propped, i) => {
...
```

#### <a name="apidoc.element.react-monocle.reactParser.getES6ReactComponents"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getES6ReactComponents (ast)](#apidoc.element.react-monocle.reactParser.getES6ReactComponents)
- description and source-code
```javascript
function getES6ReactComponents(ast) {
  const output = {
    name: '',
    props: {},
    state: {},
    methods: [],
    children: [],
  };
  let iter = [];
  let outside;
  const checker = {};
  esrecurse.visit(ast, {
    ClassDeclaration(node) {
      if (isES6ReactComponent(node)) {
        output.name = node.id.name;
        this.visitChildren(node);
      }
    },
    MethodDefinition(node) {
      if (reactMethods.indexOf(node.key.name) < 0) output.methods.push(node.key.name);
      this.visitChildren(node);
    },
    // ExpressionStatement(node) {
    //   if (node.expression.left && node.expression.left.property && node.expression.left.property.name === 'state') {
    //     output.state = getReactStates(node.expression.right);
    //   }
    //   this.visitChildren(node);
    // },
    JSXElement(node) {
      // TODO: DO STUFF WITH JSX AFTER FINDING STUFF BOI
      output.children = getChildJSXElements(node, output.name);
      output.props = getReactProps(node, output.name);
      if (htmlElements.indexOf(node.openingElement.name.name) < 0) {
        outside = {
          name: node.openingElement.name.name,
          children: getChildJSXElements(node, output.name),
          props: getReactProps(node, output.name),
          state: {},
          methods: [],
        };
      }
      const forIn = esquery(ast, 'ForInStatement').filter(ele => {
        const searched = bfs(ele).filter(n => {
          return n.type === 'JSXElement';
        });
        return searched.length > 0;
      });
      if (forIn.length > 0) iter = iter.concat(forInFinder(forIn, output.name));

      const forLoop = esquery(ast, 'ForStatement').filter(ele => {
        const searched = bfs(ele).filter(n => {
          return n.type === 'JSXElement';
        });
        return searched.length > 0;
      });
      if (forLoop.length > 0) iter = iter.concat(forLoopFinder(forLoop, output.name));

      const higherOrderFunc = esquery(ast, 'CallExpression').filter(ele => {
        let higherOrderChecker = false;
        const searched = bfs(ele).filter(n => {
          return n.type === 'JSXElement';
        });
        if (ele.callee.property && ele.callee.property.name.match(/(map|forEach|filter|reduce)/)) {
          higherOrderChecker = ele.callee.property.name.match(/(map|forEach|filter|reduce)/);
        }
        return searched.length > 0 && higherOrderChecker;
      });
      if (higherOrderFunc.length > 0) iter = iter.concat(higherOrderFunctionFinder(higherOrderFunc, output.name));
    },
  });

  if (outside) output.children.push(outside);
  output.children.forEach((ele, i) => {
    checker[ele.name] = i;
  });

  for (let i = 0; i < iter.length; i++) {
    if (checker.hasOwnProperty(iter[i].jsx.name)) {
      output.children[checker[iter[i].jsx.name]] = iter[i].jsx;
    }
  }
  return output;
}
```
- example usage
```shell
...
const formatted = {};

// parsing AST into formatted objects based on ES5/ES6 syntax
for (const key in obj) {
  if (key === 'ENTRY') continue;
  const componentChecker = reactParser.componentChecker(obj[key]);
  // componentChecker returns true for es6 classes, false for everything else
  if (componentChecker === 'ES6') formatted[key] = reactParser.getES6ReactComponents(obj[key]);
  else if (componentChecker === 'ES5') formatted[key] = reactParser.getES5ReactComponents(obj[key]);
  else formatted[key] = reactParser.getStatelessFunctionalComponents(obj[key], key)
}

for (const key in formatted) {
  formatted[key].children.forEach(ele => {
    if (Array.isArray(ele.props)) {
...
```

#### <a name="apidoc.element.react-monocle.reactParser.getStatelessFunctionalComponents"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>getStatelessFunctionalComponents (ast, name)](#apidoc.element.react-monocle.reactParser.getStatelessFunctionalComponents)
- description and source-code
```javascript
function getStatelessFunctionalComponents(ast, name) {
  const output = {
    name: name,
    state: {},
    props: {},
    methods: [],
    children: [],
  };

  let iter = [];
  let outside;
  const checker = {};
  esrecurse.visit(ast, {
    ObjectExpression(node) {
      node.properties.forEach(prop => {
        if (reactMethods.indexOf(prop.key.name) < 0
          && prop.value.type === 'FunctionExpression') {
          output.methods.push(prop.key.name);
        }
      });
      this.visitChildren(node);
    },
    JSXElement(node) {
      output.children = getChildJSXElements(node, output.name);
      output.props = getReactProps(node, output.name);
      if (htmlElements.indexOf(node.openingElement.name.name) < 0) {
        outside = {
          name: node.openingElement.name.name,
          children: getChildJSXElements(node, output.name),
          props: getReactProps(node, output.name),
          state: {},
          methods: [],
        };
      }
    },
  });

  const forIn = esquery(ast, 'ForInStatement').filter(ele => {
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    return searched.length > 0;
  });
  if (forIn.length > 0) iter = iter.concat(forInFinder(forIn, output.name));

  const forLoop = esquery(ast, 'ForStatement').filter(ele => {
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    return searched.length > 0;
  });
  if (forLoop.length > 0) iter = iter.concat(forLoopFinder(forLoop, output.name));

  const higherOrderFunc = esquery(ast, 'CallExpression').filter(ele => {
    let higherOrderChecker = false;
    const searched = bfs(ele).filter(n => {
      return n.type === 'JSXElement';
    });
    if (ele.callee.property && ele.callee.property.name.match(/(map|forEach|filter|reduce)/)) {
      higherOrderChecker = ele.callee.property.name.match(/(map|forEach|filter|reduce)/);
    }
    return searched.length > 0 && higherOrderChecker;
  });
  if (higherOrderFunc.length > 0) iter = iter.concat(higherOrderFunctionFinder(higherOrderFunc, output.name));

  if (outside) output.children.push(outside);
  output.children.forEach((ele, i) => {
    checker[ele.name] = i;
  });

  for (let i = 0; i < iter.length; i++) {
    if (checker.hasOwnProperty(iter[i].jsx.name)) {
      output.children[checker[iter[i].jsx.name]] = iter[i].jsx;
    }
  }
  return output;
}
```
- example usage
```shell
...
// parsing AST into formatted objects based on ES5/ES6 syntax
for (const key in obj) {
  if (key === 'ENTRY') continue;
  const componentChecker = reactParser.componentChecker(obj[key]);
  // componentChecker returns true for es6 classes, false for everything else
  if (componentChecker === 'ES6') formatted[key] = reactParser.getES6ReactComponents(obj[key]);
  else if (componentChecker === 'ES5') formatted[key] = reactParser.getES5ReactComponents(obj[key]);
  else formatted[key] = reactParser.getStatelessFunctionalComponents(obj[key], key)
}

for (const key in formatted) {
  formatted[key].children.forEach(ele => {
    if (Array.isArray(ele.props)) {
      ele.props.forEach((propped, i) => {
        if (typeof propped.value === 'object' && propped.value.name && propped.value.children) {
...
```

#### <a name="apidoc.element.react-monocle.reactParser.higherOrderFunctionFinder"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>higherOrderFunctionFinder (arr, name)](#apidoc.element.react-monocle.reactParser.higherOrderFunctionFinder)
- description and source-code
```javascript
function higherOrderFunctionFinder(arr, name) {
  const result = arr.map(ele => {
    // since every higher order function will have some parameter
    // will be used to replace with what it actually is
    const param = ele.arguments[0].params[0].name;
    const jsxnode = esquery(ele, 'JSXElement')[0];
    const obj = {};
    obj.variables = {};
    esquery(ele, 'VariableDeclarator').forEach(vars => {
      obj.variables[vars.id.name] = escodegen.generate(vars.init);
    });

    if (jsxnode && htmlElements.indexOf(jsxnode.openingElement.name.name)) {
      let current = ele.callee.object;
      let found;
      while (current && current.property) {
        found = '.${current.property.name}${found || ''}';
        current = current.object;
        if (current.type === 'Identifier') {
          found = '.${current.name}${found || ''}';
          break;
        }
      }

      obj.jsx = {
        name: jsxnode.openingElement.name.name,
        children: getChildJSXElements(jsxnode, name),
        props: getReactProps(jsxnode, name),
        state: {},
        methods: [],
        iterated: 'higherOrder',
        source: found.replace('.', ''),
      };

      const propsArr = obj.jsx.props;
      for (let i = 0; i < propsArr.length; i++) {
        propsArr[i].value = propsArr[i].value.replace(param, '${obj.jsx.source}[i]');
        for (const key in obj.variables) {
          if (propsArr[i].value.includes(key)) {
            propsArr[i].value = propsArr[i].value.replace(key, obj.variables[key]);
          }
        }
      }
    }
    return obj;
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.reactParser.jsToAst"></a>[function <span class="apidocSignatureSpan">react-monocle.reactParser.</span>jsToAst (js)](#apidoc.element.react-monocle.reactParser.jsToAst)
- description and source-code
```javascript
function jsToAst(js) {
  const ast = acorn.parse(js, {
    plugins: { jsx: true },
  });
  if (ast.body.length === 0) throw new Error('Empty AST input');
  return ast;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-monocle.stringRegexHelper"></a>[module react-monocle.stringRegexHelper](#apidoc.module.react-monocle.stringRegexHelper)

#### <a name="apidoc.element.react-monocle.stringRegexHelper.regexIndexOf"></a>[function <span class="apidocSignatureSpan">react-monocle.stringRegexHelper.</span>regexIndexOf (string, regex, startpos)](#apidoc.element.react-monocle.stringRegexHelper.regexIndexOf)
- description and source-code
```javascript
regexIndexOf(string, regex, startpos) {
  var indexOf = string.substring(startpos || 0).search(regex);
  return (indexOf >= 0) ? (indexOf + (startpos || 0)) : indexOf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-monocle.stringRegexHelper.regexLastIndexOf"></a>[function <span class="apidocSignatureSpan">react-monocle.stringRegexHelper.</span>regexLastIndexOf (string, regex, startpos)](#apidoc.element.react-monocle.stringRegexHelper.regexLastIndexOf)
- description and source-code
```javascript
regexLastIndexOf(string, regex, startpos) {
    regex = (regex.global)
      ? regex
      : new RegExp(regex.source, "g" + (regex.ignoreCase ? "i" : "") + (regex.multiLine ? "m" : ""));
    if(typeof (startpos) == "undefined") {
        startpos = string.length;
    } else if(startpos < 0) {
        startpos = 0;
    }
    var stringToWorkWith = string.substring(0, startpos + 1);
    var lastIndexOf = -1;
    let result = regex.exec(stringToWorkWith);
    while (result !== null) {
      lastIndexOf = result.index;
      regex.lastIndex = result.index + result[0].length;
      result = regex.exec(stringToWorkWith);
    }
    return lastIndexOf;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
