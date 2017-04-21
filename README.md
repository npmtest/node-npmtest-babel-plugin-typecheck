# npmtest-babel-plugin-typecheck

#### basic test coverage for  [babel-plugin-typecheck (v3.9.0)](https://github.com/codemix/babel-plugin-typecheck)  [![npm package](https://img.shields.io/npm/v/npmtest-babel-plugin-typecheck.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-babel-plugin-typecheck) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-babel-plugin-typecheck.svg)](https://travis-ci.org/npmtest/node-npmtest-babel-plugin-typecheck)

#### Transforms flow type annotations into runtime type checks.

[![NPM](https://nodei.co/npm/babel-plugin-typecheck.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/babel-plugin-typecheck)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-babel-plugin-typecheck/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-babel-plugin-typecheck/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/test-report.html](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-babel-plugin-typecheck/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-babel-plugin-typecheck/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-babel-plugin-typecheck/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-babel-plugin-typecheck/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-babel-plugin-typecheck/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charles Pick"
    },
    "bugs": {
        "url": "https://github.com/codemix/babel-plugin-typecheck/issues"
    },
    "dependencies": {
        "babel-generator": "^6.7.7"
    },
    "description": "Transforms flow type annotations into runtime type checks.",
    "devDependencies": {
        "babel-cli": "^6.7.7",
        "babel-core": "^6.1.0",
        "babel-plugin-syntax-class-properties": "^6.1.18",
        "babel-plugin-syntax-flow": "^6.0.14",
        "babel-plugin-transform-decorators-legacy": "^1.0.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.1.3",
        "babel-plugin-transform-flow-strip-types": "^6.0.14",
        "babel-polyfill": "^6.0.16",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-react": "^6.5.0",
        "babel-preset-stage-0": "^6.5.0",
        "babel-preset-stage-1": "^6.5.0",
        "mocha": "~2.2.4",
        "should": "^6.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0edac7573ae24ee58c6f91319f574bc5124b0f0f",
        "tarball": "https://registry.npmjs.org/babel-plugin-typecheck/-/babel-plugin-typecheck-3.9.0.tgz"
    },
    "gitHead": "04146f2e008b6ec9cd7e455b57c1408e6028f637",
    "homepage": "https://github.com/codemix/babel-plugin-typecheck",
    "keywords": [
        "babel",
        "babel-plugin",
        "types",
        "typing",
        "typecheck",
        "type check",
        "flow"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "codemix"
        }
    ],
    "name": "babel-plugin-typecheck",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/codemix/babel-plugin-typecheck.git"
    },
    "scripts": {
        "build": "babel --plugins syntax-flow,transform-flow-strip-types -d ./lib ./src",
        "build-typed": "npm run build && babel --plugins ../lib,syntax-flow,transform-flow-strip-types -d ./lib-checked ./src",
        "prepublish": "npm run test-checked",
        "pretest": "npm run build",
        "test": "mocha ./test/index.js",
        "test-checked": "npm run build-typed && TYPECHECK_USE_LIBCHECKED=1 mocha ./test/index.js",
        "watch": "NODE_WATCH=1 mocha --watch"
    },
    "version": "3.9.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
