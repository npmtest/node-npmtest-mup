# npmtest-mup

#### basic test coverage for  [mup (v1.2.6)](https://github.com/kadirahq/meteor-up#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-mup.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-mup) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-mup.svg)](https://travis-ci.org/npmtest/node-npmtest-mup)

#### Production Quality Meteor Deployments

[![NPM](https://nodei.co/npm/mup.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mup)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-mup/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-mup/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-mup/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-mup/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-mup/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-mup/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-mup/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-mup/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-mup/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-mup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-mup/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-mup/build/test-report.html](https://npmtest.github.io/node-npmtest-mup/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-mup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-mup/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-mup/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mup/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mup/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-mup/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-mup/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "mup",
    "version": "1.2.6",
    "description": "Production Quality Meteor Deployments",
    "main": "lib/index.js",
    "bin": {
        "mup": "./index.js"
    },
    "scripts": {
        "prepublish": "npm run build -s",
        "build": "babel src --out-dir lib --sourceRoot=./ --copy-files --presets=es2015,es2016,es2017,stage-3",
        "build:watch": "npm run build -s -- -w",
        "test": "bash ./tests/run.sh",
        "test:custom-server": "nofat test",
        "test:parallel": "bash ./tests/run-parallel.sh",
        "lint": "eslint . && npm run lint:defaultConfig -s",
        "lint:defaultConfig": "eslint --ext=\".sample\" -c .eslintrc.yml --rule=\"comma-dangle: 0\" .",
        "lint:code": "eslint ."
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kadirahq/meteor-up.git"
    },
    "keywords": [
        "meteor"
    ],
    "author": "Kadira Inc.",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/kadirahq/meteor-up/issues"
    },
    "homepage": "https://github.com/kadirahq/meteor-up#readme",
    "devDependencies": {
        "babel-eslint": "^7.1.1",
        "babel-preset-es2015": "^6.22.0",
        "babel-preset-stage-3": "^6.22.0",
        "eslint": "^3.15.0",
        "eslint-plugin-babel": "^4.1.0",
        "nofat": "1.0.x",
        "babel-cli": "^6.23.0",
        "babel-preset-es2016": "^6.22.0",
        "babel-preset-es2017": "^6.22.0",
        "mocha": "^3.2.0"
    },
    "dependencies": {
        "archiver": "1.x.x",
        "async": "^2.1.5",
        "babel-polyfill": "6.6.1",
        "bluebird": "3.x.x",
        "boxen": "^1.0.0",
        "chai": "^3.5.0",
        "chalk": "^1.1.3",
        "commander": "2.9.x",
        "debug": "2.x.x",
        "expand-tilde": "^2.0.2",
        "joi": "^10.2.1",
        "nodemiral": "1.x.x",
        "parse-json": "^2.2.0",
        "random-seed": "^0.3.0",
        "shelljs": "0.5.x",
        "silent-npm-registry-client": "2.x.x",
        "ssh2": "0.4.x",
        "underscore": "1.x.x",
        "uuid": "2.x.x"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
