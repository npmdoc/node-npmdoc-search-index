# api documentation for  [search-index (v0.9.17)](https://github.com/fergiemcdowall/search-index)  [![npm package](https://img.shields.io/npm/v/npmdoc-search-index.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-search-index) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-search-index.svg)](https://travis-ci.org/npmdoc/node-npmdoc-search-index)
#### A persistent full text search engine for the browser and Node.js

[![NPM](https://nodei.co/npm/search-index.png?downloads=true)](https://www.npmjs.com/package/search-index)

[![apidoc](https://npmdoc.github.io/node-npmdoc-search-index/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-search-index_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-search-index/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-search-index/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-search-index/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fergus McDowall",
        "email": "fergusmcdowall@gmail.com"
    },
    "browser": {
        "leveldown": "level-js"
    },
    "bugs": {
        "url": "https://github.com/fergiemcdowall/search-index/issues"
    },
    "dependencies": {
        "bunyan": "^1.8.10",
        "leveldown": "^1.6.0",
        "levelup": "^1.3.5",
        "search-index-adder": "^0.2.0",
        "search-index-searcher": "^0.1.28"
    },
    "description": "A persistent full text search engine for the browser and Node.js",
    "devDependencies": {
        "JSONStream": "^1.1.4",
        "brfs": "^1.4.3",
        "browser-run": "^3.3.0",
        "browserify": "^13.1.0",
        "disc": "^1.3.2",
        "highland": "^2.10.0",
        "left-pad": "^1.1.3",
        "level-js": "^2.2.4",
        "mocha": "^3.2.0",
        "request": "^2.78.0",
        "reuters-21578-json": "0.0.8",
        "should": "^10.0.0",
        "sqldown": "^2.1.0",
        "sqlite3": "^3.1.4",
        "standard": "8.1.0",
        "stopword": "^0.1.1",
        "tape": "^4.6.0",
        "term-vector": "0.1.2",
        "uglifyjs": "^2.4.10",
        "written-number": "^0.5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "7780c24dac94aa98902e05e9181c987d6b8363a5",
        "tarball": "https://registry.npmjs.org/search-index/-/search-index-0.9.17.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "4c77d6d3736a392e2418a3a510b05b21136f0058",
    "homepage": "https://github.com/fergiemcdowall/search-index",
    "keywords": [
        "index",
        "language",
        "lucene",
        "natural",
        "offline",
        "search"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "fergie",
            "email": "fergusmcdowall@gmail.com"
        },
        {
            "name": "mewwts",
            "email": "mats@plysjbyen.net"
        }
    ],
    "name": "search-index",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fergiemcdowall/search-index.git"
    },
    "scripts": {
        "anylize-web-bundle": "browserify --full-paths lib/index.js --standalone SearchIndex > dist/search-index-full-paths.js && discify dist/search-index-full-paths.js > dist/out.html",
        "dist": "browserify lib/index.js --standalone SearchIndex > dist/search-index.js",
        "dist-min": "npm run dist && cat dist/search-index.js | uglifyjs -c dead_code > dist/search-index.min.js",
        "empty-sandbox": "rm -rf test/sandbox && mkdir test/sandbox",
        "test": "npm run empty-sandbox && date && npm run test-node && npm run test-browser && standard test/* lib/*",
        "test-browser": "node test/browser/runtest.js",
        "test-node": "tape test/node/tape-tests/*.js && mocha test/node/mocha-tests --recursive --timeout 10000"
    },
    "version": "0.9.17"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module search-index](#apidoc.module.search-index)



# <a name="apidoc.module.search-index"></a>[module search-index](#apidoc.module.search-index)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
