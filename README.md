# npmtest-flyd

#### basic test coverage for  [flyd (v0.2.4)](https://github.com/paldepind/flyd)  [![npm package](https://img.shields.io/npm/v/npmtest-flyd.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-flyd) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-flyd.svg)](https://travis-ci.org/npmtest/node-npmtest-flyd)

#### The less is more, modular, functional reactive programming library

[![NPM](https://nodei.co/npm/flyd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/flyd)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-flyd/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-flyd/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-flyd/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-flyd/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-flyd/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-flyd/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-flyd/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-flyd/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-flyd/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-flyd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-flyd/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-flyd/build/test-report.html](https://npmtest.github.io/node-npmtest-flyd/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-flyd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-flyd/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-flyd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-flyd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-flyd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-flyd/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-flyd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-flyd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Simon Friis Vindum"
    },
    "bugs": {
        "url": "https://github.com/paldepind/flyd/issues"
    },
    "dependencies": {
        "ramda": "^0.19.1"
    },
    "description": "The less is more, modular, functional reactive programming library",
    "devDependencies": {
        "benchmark": "^1.0.0",
        "bluebird": "^2.9.13",
        "browserify": "^10.2.4",
        "coveralls": "^2.11.2",
        "eslint": "^2.7.0",
        "istanbul": "^0.3.15",
        "mocha": "^2.2.1",
        "mocha-lcov-reporter": "0.0.2",
        "transducers.js": "0.3.x",
        "uglifyjs": "^2.4.10"
    },
    "directories": {
        "example": "examples",
        "test": "test"
    },
    "dist": {
        "shasum": "0414c837c34fae69b1277752cf004382effb9900",
        "tarball": "https://registry.npmjs.org/flyd/-/flyd-0.2.4.tgz"
    },
    "gitHead": "40abf488967f95666b09cf1576d8915abd87fa0b",
    "homepage": "https://github.com/paldepind/flyd",
    "keywords": [
        "functional",
        "reactive",
        "modular",
        "library"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "paldepind"
        }
    ],
    "name": "flyd",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/paldepind/flyd.git"
    },
    "scripts": {
        "build": "browserify -s flyd lib/index.js > flyd.js && uglifyjs flyd.js -o flyd.min.js",
        "docs": "documentation -f md lib/index.js > API.md",
        "perf": "./perf/run-benchmarks",
        "post-to-coveralls-io": "istanbul cover _mocha --report lcovonly -- -R spec && cat ./coverage/lcov.info | coveralls && rm -rf ./coverage",
        "test": "eslint lib/ test/ module/ && mocha -R dot test/*.js module/**/test/*.js",
        "test-lib": "mocha"
    },
    "testling": {
        "harness": "mocha",
        "files": "test/*.js",
        "browsers": [
            "ie/8..latest",
            "firefox/16..latest",
            "firefox/nightly",
            "chrome/22..latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ]
    },
    "version": "0.2.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
