# api documentation for  [core-decorators (v0.17.0)](https://github.com/jayphelps/core-decorators.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-core-decorators.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-core-decorators) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-core-decorators.svg)](https://travis-ci.org/npmdoc/node-npmdoc-core-decorators)
#### Library of JavaScript stage-0 decorators (aka ES2016/ES7 decorators but that's not accurate!) inspired by languages that come with built-ins like @​override, @​deprecate, @​autobind, @​mixin and more! Works great with React/Angular/more!

[![NPM](https://nodei.co/npm/core-decorators.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/core-decorators)

- [https://npmdoc.github.io/node-npmdoc-core-decorators/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-core-decorators/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-core-decorators/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jay Phelps"
    },
    "bugs": {
        "url": "https://github.com/jayphelps/core-decorators.js/issues"
    },
    "dependencies": {},
    "description": "Library of JavaScript stage-0 decorators (aka ES2016/ES7 decorators but that's not accurate!) inspired by languages that come with built-ins like @​override, @​deprecate, @​autobind, @​mixin and more! Works great with React/Angular/more!",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-core": "^6.24.0",
        "babel-plugin-transform-class-properties": "^6.23.0",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.24.0",
        "babel-plugin-transform-flow-strip-types": "^6.22.0",
        "babel-plugin-transform-object-rest-spread": "^6.23.0",
        "babel-polyfill": "^6.23.0",
        "babel-preset-es2015": "^6.24.0",
        "camelcase": "^4.1.0",
        "chai": "^3.5.0",
        "glob": "^7.1.1",
        "global-wrap": "^2.0.0",
        "interop-require": "1.0.0",
        "lodash": "4.17.4",
        "mocha": "^3.2.0",
        "sinon": "^2.1.0",
        "sinon-chai": "^2.9.0"
    },
    "directories": {},
    "dist": {
        "shasum": "3f43180a86d2ab0cc51069f46a1ec3e49e7cebd6",
        "tarball": "https://registry.npmjs.org/core-decorators/-/core-decorators-0.17.0.tgz"
    },
    "files": [
        "es",
        "lib",
        "src",
        "README.md",
        "LICENSE"
    ],
    "gitHead": "a52d02f6ba206f6d89b879c6936b840617059ded",
    "homepage": "https://github.com/jayphelps/core-decorators.js",
    "jsnext:main": "es/core-decorators.js",
    "keywords": [
        "es6",
        "es7",
        "es2015",
        "es2016",
        "babel",
        "decorators",
        "override",
        "deprecated",
        "java",
        "annotations",
        "autobind",
        "react",
        "angular",
        "lodash",
        "mixin",
        "mixins"
    ],
    "license": "MIT",
    "main": "lib/core-decorators.js",
    "maintainers": [
        {
            "name": "jayphelps"
        }
    ],
    "module": "es/core-decorators.js",
    "name": "core-decorators",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jayphelps/core-decorators.js.git"
    },
    "scripts": {
        "build": "babel --out-dir lib src",
        "build-bower": "babel-node scripts/build-bower.js",
        "build-es": "BABEL_ENV=es babel --out-dir es src",
        "test": "npm run build && mocha --compilers js:babel-core/register --require babel-polyfill \"test/**/*.spec.js\""
    },
    "version": "0.17.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
