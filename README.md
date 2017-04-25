# npmdoc-norch

#### basic api documentation for  [norch (v0.8.12)](https://github.com/fergiemcdowall/norch#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-norch.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-norch) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-norch.svg)](https://travis-ci.org/npmdoc/node-npmdoc-norch)

#### A search engine based on Node.js and LevelDB

[![NPM](https://nodei.co/npm/norch.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/norch)

- [https://npmdoc.github.io/node-npmdoc-norch/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-norch/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-norch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-norch/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-norch/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-norch/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "norch": "./bin/norch"
    },
    "bugs": {
        "url": "https://github.com/fergiemcdowall/norch/issues"
    },
    "dependencies": {
        "JSONStream": "^1.2.1",
        "bunyan": "^1.8.4",
        "colors": "^1.1.2",
        "commander": "^2.9.0",
        "lodash": "^4.16.6",
        "restify": "^4.2.0",
        "search-index": "^0.9.15"
    },
    "description": "A search engine based on Node.js and LevelDB",
    "devDependencies": {
        "browser-run": "^3.3.0",
        "browserify": "^13.1.1",
        "left-pad": "^1.1.3",
        "request": "^2.69.0",
        "reuters-21578-json": "^0.0.8",
        "standard": "^8.5.0",
        "tape": "^4.6.2",
        "written-number": "^0.5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "ce6fb5b094afc3c2c0579005c0c75b20caec8f17",
        "tarball": "https://registry.npmjs.org/norch/-/norch-0.8.12.tgz"
    },
    "engines": {
        "node": ">3"
    },
    "gitHead": "3d04be3485f4364aa3452fe6bbb420a313b48a7f",
    "homepage": "https://github.com/fergiemcdowall/norch#readme",
    "keywords": [
        "elasticsearch",
        "search",
        "server",
        "solr",
        "free text",
        "big data"
    ],
    "license": "MIT",
    "main": "./lib/norch",
    "maintainers": [
        {
            "name": "fergie"
        }
    ],
    "name": "norch",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fergiemcdowall/norch.git"
    },
    "scripts": {
        "start": "./bin/norch",
        "test": "rm -rf test/sandbox && mkdir test/sandbox && date && tape test/*test.js && npm run test-cli && npm run test-browser && standard --fix",
        "test-browser": "./bin/norch -i test/sandbox/browser-test -p 9999 & tape test/browser/runtest.js && kill $!",
        "test-cli": "./bin/norch -p 9090 -i test/sandbox/norch-cli & sleep 5s && bats test/test.bats && kill $!"
    },
    "version": "0.8.12"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
