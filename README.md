# npmdoc-gulp-gh-pages

#### api documentation for  [gulp-gh-pages (v0.5.4)](https://github.com/shinnn/gulp-gh-pages#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-gh-pages.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-gh-pages) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-gh-pages.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-gh-pages)

#### gulp plugin to publish contents to Github pages

[![NPM](https://nodei.co/npm/gulp-gh-pages.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-gh-pages)

- [https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-gh-pages/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Micheal Benedict",
        "url": "https://github.com/rowoot"
    },
    "bugs": {
        "url": "https://github.com/shinnn/gulp-gh-pages/issues"
    },
    "contributors": [
        {
            "name": "Shinnosuke Watanabe",
            "url": "https://github.com/shinnn"
        }
    ],
    "dependencies": {
        "gift": "^0.6.1",
        "gulp-util": "^3.0.7",
        "readable-stream": "^2.0.2",
        "rimraf": "^2.4.3",
        "vinyl-fs": "^2.2.1",
        "wrap-promise": "^1.0.1"
    },
    "description": "gulp plugin to publish contents to Github pages",
    "devDependencies": {
        "@shinnn/eslint-config-node-legacy": "^1.0.0",
        "eslint": "^1.7.2",
        "graceful-fs": "^4.1.2",
        "istanbul": "^0.4.0",
        "log-symbols": "^1.0.2",
        "mocha": "^2.3.3",
        "node-uuid": "^1.4.3",
        "octonode": "^0.7.4",
        "read-remove-file": "^3.0.0",
        "vinyl": "^1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a6732ca475ab9b5a53253c1c24734c40c21b6546",
        "tarball": "https://registry.npmjs.org/gulp-gh-pages/-/gulp-gh-pages-0.5.4.tgz"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "e740e1c4d8789317db706b3fdb712d82454cbc03",
    "homepage": "https://github.com/shinnn/gulp-gh-pages#readme",
    "keywords": [
        "git",
        "push",
        "commit",
        "branch",
        "deploy",
        "deployment",
        "publish",
        "site",
        "website",
        "gulp",
        "gulpplugin",
        "gh-pages",
        "dist",
        "github"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "rowoot"
        },
        {
            "name": "shinnn"
        }
    ],
    "name": "gulp-gh-pages",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/shinnn/gulp-gh-pages.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha test.js -x=test.js -- --timeout 50000",
        "pretest": "eslint --config @shinnn/node-legacy --env mocha --rule 'no-underscore-dangle: 0' --rule 'camelcase: 0' index.js test.js lib",
        "test": "mocha test.js --timeout 50000 --full-trace",
        "test-only": "mocha test.js --timeout 50000 --full-trace"
    },
    "version": "0.5.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
