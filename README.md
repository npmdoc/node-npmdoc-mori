# npmdoc-mori

#### api documentation for  [mori (v0.3.2)](https://github.com/swannodette/mori)  [![npm package](https://img.shields.io/npm/v/npmdoc-mori.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mori) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mori.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mori)

#### Persistent Data Structures for JavaScript

[![NPM](https://nodei.co/npm/mori.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mori)

- [https://npmdoc.github.io/node-npmdoc-mori/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mori/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mori/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David Nolen",
        "url": "https://github.com/swannodette"
    },
    "bugs": {
        "url": "https://github.com/swannodette/mori/issues"
    },
    "contributors": [
        {
            "name": "David Nolen",
            "url": "https://github.com/swannodette"
        }
    ],
    "dependencies": {},
    "description": "Persistent Data Structures for JavaScript",
    "devDependencies": {
        "immutable": "3.5.0",
        "jasmine-node": "1.7.0"
    },
    "directories": {
        "test": "./spec"
    },
    "dist": {
        "shasum": "1a53da165287f3bef0cab62398c4931bece80a3f",
        "tarball": "https://registry.npmjs.org/mori/-/mori-0.3.2.tgz"
    },
    "engines": {
        "node": ">=0.8.22"
    },
    "gitHead": "391df0b7cadf12236c982588d8336b44cefd0fa2",
    "homepage": "https://github.com/swannodette/mori",
    "keywords": [
        "data",
        "structure",
        "persistent",
        "clojure",
        "clojurescript",
        "map",
        "filter",
        "reduce"
    ],
    "licenses": [
        {
            "type": "EPL",
            "url": "https://raw.github.com/swannodette/mori/master/epl-v10.html"
        }
    ],
    "main": "./mori.js",
    "maintainers": [
        {
            "name": "dnolen"
        }
    ],
    "name": "mori",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/swannodette/mori.git"
    },
    "scripts": {
        "build": "./scripts/build.sh",
        "build-clean": "./scripts/build_clean.sh",
        "clean": "./scripts/clean.sh",
        "docs": "./scripts/docs.sh",
        "prepublish": "npm run-script build-clean",
        "test": "jasmine-node spec"
    },
    "version": "0.3.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
