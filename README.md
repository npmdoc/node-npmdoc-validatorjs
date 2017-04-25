# npmdoc-validatorjs

#### basic api documentation for  [validatorjs (v3.12.0)](https://github.com/skaterdav85/validatorjs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-validatorjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-validatorjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-validatorjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-validatorjs)

#### Validation library inspired by Laravel's Validator

[![NPM](https://nodei.co/npm/validatorjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/validatorjs)

- [https://npmdoc.github.io/node-npmdoc-validatorjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-validatorjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-validatorjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David"
    },
    "bugs": {
        "url": "https://github.com/skaterdav85/validatorjs/issues?labels=bug&milestone=1&page=1&state=open"
    },
    "contributors": [
        {
            "name": "Gary Green"
        },
        {
            "name": "Karol Janyst"
        },
        {
            "name": "Mike Erickson"
        }
    ],
    "dependencies": {},
    "description": "Validation library inspired by Laravel's Validator",
    "devDependencies": {
        "browserify": "^13.0.1",
        "chai": "~3.5.0",
        "grunt": "1.0.1",
        "grunt-browserify": "^5.0.0",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-concat": "~1.0.1",
        "grunt-contrib-jshint": "1.0.0",
        "grunt-contrib-uglify": "1.0.1",
        "grunt-contrib-watch": "~1.0.0",
        "jit-grunt": "^0.10.0",
        "karma": "~1.1.0",
        "karma-browserify": "^5.0.5",
        "karma-chai": "~0.1.0",
        "karma-chrome-launcher": "~1.0.1",
        "karma-coverage": "~1.0.0",
        "karma-growl-notifications-reporter": "0.0.2",
        "karma-mocha": "~1.1.1",
        "karma-phantomjs-launcher": "~1.0.1",
        "mocha": "~2.5.3",
        "mocha-better-spec-reporter": "github:mikeerickson/mocha-better-spec-reporter"
    },
    "directories": {},
    "dist": {
        "shasum": "6319f4ea872a323dd459000e2cbe9e632fd4816b",
        "tarball": "https://registry.npmjs.org/validatorjs/-/validatorjs-3.12.0.tgz"
    },
    "gitHead": "b41d4fcca458f243a596ce73b7302bf59c739485",
    "homepage": "https://github.com/skaterdav85/validatorjs#readme",
    "keywords": [
        "validatorjs",
        "validator.js",
        "data validation",
        "validator",
        "validate",
        "validation",
        "data",
        "laravel",
        "laravel-validator-for-js"
    ],
    "license": "MIT",
    "main": "./src/validator.js",
    "maintainers": [
        {
            "name": "garygreen"
        },
        {
            "name": "mikeerickson"
        },
        {
            "name": "skaterdav85"
        }
    ],
    "name": "validatorjs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/skaterdav85/validatorjs.git"
    },
    "scripts": {
        "test": "npm run test-node && npm run test-browser",
        "test-browser": "grunt dist && node node_modules/karma/bin/karma start --single-run --browsers PhantomJS",
        "test-node": "node node_modules/mocha/bin/mocha spec",
        "test-node:watch": "node node_modules/mocha/bin/mocha --watch spec"
    },
    "version": "3.12.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
