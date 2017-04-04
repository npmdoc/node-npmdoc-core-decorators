# api documentation for  [core-decorators (v0.17.0)](https://github.com/jayphelps/core-decorators.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-core-decorators.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-core-decorators) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-core-decorators.svg)](https://travis-ci.org/npmdoc/node-npmdoc-core-decorators)
#### Library of JavaScript stage-0 decorators (aka ES2016/ES7 decorators but that's not accurate!) inspired by languages that come with built-ins like @​override, @​deprecate, @​autobind, @​mixin and more! Works great with React/Angular/more!

[![NPM](https://nodei.co/npm/core-decorators.png?downloads=true)](https://www.npmjs.com/package/core-decorators)

[![apidoc](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-core-decorators_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-core-decorators/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-core-decorators/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jay Phelps",
        "email": "hello@jayphelps"
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
            "name": "jayphelps",
            "email": "hello@jayphelps.com"
        }
    ],
    "module": "es/core-decorators.js",
    "name": "core-decorators",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module core-decorators](#apidoc.module.core-decorators)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>applyDecorators (Class, props)](#apidoc.element.core-decorators.applyDecorators)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>autobind ()](#apidoc.element.core-decorators.autobind)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>debounce ()](#apidoc.element.core-decorators.debounce)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>decorate ()](#apidoc.element.core-decorators.decorate)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>deprecate ()](#apidoc.element.core-decorators.deprecate)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>deprecated ()](#apidoc.element.core-decorators.deprecated)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>enumerable ()](#apidoc.element.core-decorators.enumerable)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>extendDescriptor ()](#apidoc.element.core-decorators.extendDescriptor)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>lazyInitialize ()](#apidoc.element.core-decorators.lazyInitialize)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>memoize ()](#apidoc.element.core-decorators.memoize)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>mixin ()](#apidoc.element.core-decorators.mixin)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>mixins ()](#apidoc.element.core-decorators.mixins)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>nonconfigurable ()](#apidoc.element.core-decorators.nonconfigurable)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>nonenumerable ()](#apidoc.element.core-decorators.nonenumerable)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>override ()](#apidoc.element.core-decorators.override)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>profile ()](#apidoc.element.core-decorators.profile)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>readonly ()](#apidoc.element.core-decorators.readonly)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>suppressWarnings ()](#apidoc.element.core-decorators.suppressWarnings)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>throttle ()](#apidoc.element.core-decorators.throttle)
1.  [function <span class="apidocSignatureSpan">core-decorators.</span>time ()](#apidoc.element.core-decorators.time)
1.  object <span class="apidocSignatureSpan">core-decorators.</span>lazy_initialize
1.  object <span class="apidocSignatureSpan">core-decorators.</span>suppress_warnings

#### [module core-decorators.applyDecorators](#apidoc.module.core-decorators.applyDecorators)
1.  [function <span class="apidocSignatureSpan">core-decorators.applyDecorators.</span>default (Class, props)](#apidoc.element.core-decorators.applyDecorators.default)

#### [module core-decorators.autobind](#apidoc.module.core-decorators.autobind)
1.  [function <span class="apidocSignatureSpan">core-decorators.autobind.</span>default ()](#apidoc.element.core-decorators.autobind.default)

#### [module core-decorators.debounce](#apidoc.module.core-decorators.debounce)
1.  [function <span class="apidocSignatureSpan">core-decorators.debounce.</span>default ()](#apidoc.element.core-decorators.debounce.default)

#### [module core-decorators.decorate](#apidoc.module.core-decorators.decorate)
1.  [function <span class="apidocSignatureSpan">core-decorators.decorate.</span>default ()](#apidoc.element.core-decorators.decorate.default)

#### [module core-decorators.deprecate](#apidoc.module.core-decorators.deprecate)
1.  [function <span class="apidocSignatureSpan">core-decorators.deprecate.</span>default ()](#apidoc.element.core-decorators.deprecate.default)

#### [module core-decorators.enumerable](#apidoc.module.core-decorators.enumerable)
1.  [function <span class="apidocSignatureSpan">core-decorators.enumerable.</span>default ()](#apidoc.element.core-decorators.enumerable.default)

#### [module core-decorators.extendDescriptor](#apidoc.module.core-decorators.extendDescriptor)
1.  [function <span class="apidocSignatureSpan">core-decorators.extendDescriptor.</span>default ()](#apidoc.element.core-decorators.extendDescriptor.default)

#### [module core-decorators.lazy_initialize](#apidoc.module.core-decorators.lazy_initialize)
1.  [function <span class="apidocSignatureSpan">core-decorators.lazy_initialize.</span>default ()](#apidoc.element.core-decorators.lazy_initialize.default)

#### [module core-decorators.memoize](#apidoc.module.core-decorators.memoize)
1.  [function <span class="apidocSignatureSpan">core-decorators.memoize.</span>default ()](#apidoc.element.core-decorators.memoize.default)

#### [module core-decorators.mixin](#apidoc.module.core-decorators.mixin)
1.  [function <span class="apidocSignatureSpan">core-decorators.mixin.</span>default ()](#apidoc.element.core-decorators.mixin.default)

#### [module core-decorators.nonconfigurable](#apidoc.module.core-decorators.nonconfigurable)
1.  [function <span class="apidocSignatureSpan">core-decorators.nonconfigurable.</span>default ()](#apidoc.element.core-decorators.nonconfigurable.default)

#### [module core-decorators.nonenumerable](#apidoc.module.core-decorators.nonenumerable)
1.  [function <span class="apidocSignatureSpan">core-decorators.nonenumerable.</span>default ()](#apidoc.element.core-decorators.nonenumerable.default)

#### [module core-decorators.override](#apidoc.module.core-decorators.override)
1.  [function <span class="apidocSignatureSpan">core-decorators.override.</span>default ()](#apidoc.element.core-decorators.override.default)

#### [module core-decorators.profile](#apidoc.module.core-decorators.profile)
1.  [function <span class="apidocSignatureSpan">core-decorators.profile.</span>default ()](#apidoc.element.core-decorators.profile.default)
1.  object <span class="apidocSignatureSpan">core-decorators.profile.</span>defaultConsole

#### [module core-decorators.readonly](#apidoc.module.core-decorators.readonly)
1.  [function <span class="apidocSignatureSpan">core-decorators.readonly.</span>default ()](#apidoc.element.core-decorators.readonly.default)

#### [module core-decorators.suppress_warnings](#apidoc.module.core-decorators.suppress_warnings)
1.  [function <span class="apidocSignatureSpan">core-decorators.suppress_warnings.</span>default ()](#apidoc.element.core-decorators.suppress_warnings.default)

#### [module core-decorators.throttle](#apidoc.module.core-decorators.throttle)
1.  [function <span class="apidocSignatureSpan">core-decorators.throttle.</span>default ()](#apidoc.element.core-decorators.throttle.default)

#### [module core-decorators.time](#apidoc.module.core-decorators.time)
1.  [function <span class="apidocSignatureSpan">core-decorators.time.</span>default ()](#apidoc.element.core-decorators.time.default)
1.  object <span class="apidocSignatureSpan">core-decorators.time.</span>defaultConsole



# <a name="apidoc.module.core-decorators"></a>[module core-decorators](#apidoc.module.core-decorators)

#### <a name="apidoc.element.core-decorators.applyDecorators"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>applyDecorators (Class, props)](#apidoc.element.core-decorators.applyDecorators)
- description and source-code
```javascript
function applyDecorators(Class, props) {
  var prototype = Class.prototype;


  for (var key in props) {
    var decorators = props[key];

    for (var i = 0, l = decorators.length; i < l; i++) {
      var decorator = decorators[i];

      defineProperty(prototype, key, decorator(prototype, key, getOwnPropertyDescriptor(prototype, key)));
    }
  }

  return Class;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.autobind"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>autobind ()](#apidoc.element.core-decorators.autobind)
- description and source-code
```javascript
function autobind() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  if (args.length === 0) {
    return function () {
      return handle(arguments);
    };
  } else {
    return handle(args);
  }
}
```
- example usage
```shell
...

This can be consumed by any transpiler that supports stage-0 of the decorators spec, like [babel.js](https://babeljs.io/) version
 5. *Babel 6 [does not yet support decorators natively](https://phabricator.babeljs.io/T2645), but you can include [babel-plugin
-transform-decorators-legacy](https://github.com/loganfsmyth/babel-plugin-transform-decorators-legacy) or use the ['applyDecorators
()' helper](#applydecorators-helper).*

core-decorators does not officially support TypeScript. There are known incompatibilities with the way it transpiles the output.
PRs certainly welcome to fix that!

##### Bower/globals

A globals version is available [here in the artifact repo](https://github.com/jayphelps/core-decorators-artifacts), or via '$ bower
 install core-decorators'. It defines a global variable 'CoreDecorators', which can then be used as you might expect: '@CoreDecorators
.autobind()', etc.

I *highly* recommend against using that globals build as it's quite strange you're using decorators (a proposed future feature of
 JavaScript) while not using ES2015 modules, a spec ratified feature used by nearly every modern framework. Also--[bower is on its
 deathbed](https://github.com/bower/bower/pull/1748) and IMO for very good reasons.

## Decorators

##### For Properties and Methods
* [@readonly](#readonly)
...
```

#### <a name="apidoc.element.core-decorators.debounce"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>debounce ()](#apidoc.element.core-decorators.debounce)
- description and source-code
```javascript
function debounce() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.decorate"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>decorate ()](#apidoc.element.core-decorators.decorate)
- description and source-code
```javascript
function decorate() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.deprecate"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>deprecate ()](#apidoc.element.core-decorators.deprecate)
- description and source-code
```javascript
function deprecate() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.deprecated"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>deprecated ()](#apidoc.element.core-decorators.deprecated)
- description and source-code
```javascript
function deprecate() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.enumerable"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>enumerable ()](#apidoc.element.core-decorators.enumerable)
- description and source-code
```javascript
function enumerable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.extendDescriptor"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>extendDescriptor ()](#apidoc.element.core-decorators.extendDescriptor)
- description and source-code
```javascript
function extendDescriptor() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.lazyInitialize"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>lazyInitialize ()](#apidoc.element.core-decorators.lazyInitialize)
- description and source-code
```javascript
function lazyInitialize() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.memoize"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>memoize ()](#apidoc.element.core-decorators.memoize)
- description and source-code
```javascript
function memoize() {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.mixin"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>mixin ()](#apidoc.element.core-decorators.mixin)
- description and source-code
```javascript
function mixin() {
  for (var _len = arguments.length, mixins = Array(_len), _key = 0; _key < _len; _key++) {
    mixins[_key] = arguments[_key];
  }

  if (typeof mixins[0] === 'function') {
    return handleClass(mixins[0], []);
  } else {
    return function (target) {
      return handleClass(target, mixins);
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.mixins"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>mixins ()](#apidoc.element.core-decorators.mixins)
- description and source-code
```javascript
function mixin() {
  for (var _len = arguments.length, mixins = Array(_len), _key = 0; _key < _len; _key++) {
    mixins[_key] = arguments[_key];
  }

  if (typeof mixins[0] === 'function') {
    return handleClass(mixins[0], []);
  } else {
    return function (target) {
      return handleClass(target, mixins);
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.nonconfigurable"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>nonconfigurable ()](#apidoc.element.core-decorators.nonconfigurable)
- description and source-code
```javascript
function nonconfigurable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.nonenumerable"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>nonenumerable ()](#apidoc.element.core-decorators.nonenumerable)
- description and source-code
```javascript
function nonenumerable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.override"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>override ()](#apidoc.element.core-decorators.override)
- description and source-code
```javascript
function override() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.profile"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>profile ()](#apidoc.element.core-decorators.profile)
- description and source-code
```javascript
function profile() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
...

  var ran = false;

  return _extends({}, descriptor, {
    value: function value() {
var label = '' + prefix;
if (!once || once && !ran) {
  console.profile(label);
  ran = true;
}

try {
  return fn.apply(this, arguments);
} finally {
  console.profileEnd(label);
...
```

#### <a name="apidoc.element.core-decorators.readonly"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>readonly ()](#apidoc.element.core-decorators.readonly)
- description and source-code
```javascript
function readonly() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.suppressWarnings"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>suppressWarnings ()](#apidoc.element.core-decorators.suppressWarnings)
- description and source-code
```javascript
function suppressWarnings() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.throttle"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>throttle ()](#apidoc.element.core-decorators.throttle)
- description and source-code
```javascript
function throttle() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-decorators.time"></a>[function <span class="apidocSignatureSpan">core-decorators.</span>time ()](#apidoc.element.core-decorators.time)
- description and source-code
```javascript
function time() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
...
var bird = new Bird();
bird.sing(); // console.time label will be 'sing-0'
bird.sing(); // console.time label will be 'sing-1'
'''

Will polyfill 'console.time' if the current environment does not support it. You can also supply a custom 'console' object as the
 second argument with the following methods:

* 'myConsole.time(label)'
* 'myConsole.timeEnd(label)'
* 'myConsole.log(value)'

'''js
let myConsole = {
time: function(label) { /* custom time() method */ },
timeEnd: function(label) { /* custom timeEnd method */ },
...
```



# <a name="apidoc.module.core-decorators.applyDecorators"></a>[module core-decorators.applyDecorators](#apidoc.module.core-decorators.applyDecorators)

#### <a name="apidoc.element.core-decorators.applyDecorators.default"></a>[function <span class="apidocSignatureSpan">core-decorators.applyDecorators.</span>default (Class, props)](#apidoc.element.core-decorators.applyDecorators.default)
- description and source-code
```javascript
function applyDecorators(Class, props) {
  var prototype = Class.prototype;


  for (var key in props) {
    var decorators = props[key];

    for (var i = 0, l = decorators.length; i < l; i++) {
      var decorator = decorators[i];

      defineProperty(prototype, key, decorator(prototype, key, getOwnPropertyDescriptor(prototype, key)));
    }
  }

  return Class;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.autobind"></a>[module core-decorators.autobind](#apidoc.module.core-decorators.autobind)

#### <a name="apidoc.element.core-decorators.autobind.default"></a>[function <span class="apidocSignatureSpan">core-decorators.autobind.</span>default ()](#apidoc.element.core-decorators.autobind.default)
- description and source-code
```javascript
function autobind() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  if (args.length === 0) {
    return function () {
      return handle(arguments);
    };
  } else {
    return handle(args);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.debounce"></a>[module core-decorators.debounce](#apidoc.module.core-decorators.debounce)

#### <a name="apidoc.element.core-decorators.debounce.default"></a>[function <span class="apidocSignatureSpan">core-decorators.debounce.</span>default ()](#apidoc.element.core-decorators.debounce.default)
- description and source-code
```javascript
function debounce() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.decorate"></a>[module core-decorators.decorate](#apidoc.module.core-decorators.decorate)

#### <a name="apidoc.element.core-decorators.decorate.default"></a>[function <span class="apidocSignatureSpan">core-decorators.decorate.</span>default ()](#apidoc.element.core-decorators.decorate.default)
- description and source-code
```javascript
function decorate() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.deprecate"></a>[module core-decorators.deprecate](#apidoc.module.core-decorators.deprecate)

#### <a name="apidoc.element.core-decorators.deprecate.default"></a>[function <span class="apidocSignatureSpan">core-decorators.deprecate.</span>default ()](#apidoc.element.core-decorators.deprecate.default)
- description and source-code
```javascript
function deprecate() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.enumerable"></a>[module core-decorators.enumerable](#apidoc.module.core-decorators.enumerable)

#### <a name="apidoc.element.core-decorators.enumerable.default"></a>[function <span class="apidocSignatureSpan">core-decorators.enumerable.</span>default ()](#apidoc.element.core-decorators.enumerable.default)
- description and source-code
```javascript
function enumerable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.extendDescriptor"></a>[module core-decorators.extendDescriptor](#apidoc.module.core-decorators.extendDescriptor)

#### <a name="apidoc.element.core-decorators.extendDescriptor.default"></a>[function <span class="apidocSignatureSpan">core-decorators.extendDescriptor.</span>default ()](#apidoc.element.core-decorators.extendDescriptor.default)
- description and source-code
```javascript
function extendDescriptor() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.lazy_initialize"></a>[module core-decorators.lazy_initialize](#apidoc.module.core-decorators.lazy_initialize)

#### <a name="apidoc.element.core-decorators.lazy_initialize.default"></a>[function <span class="apidocSignatureSpan">core-decorators.lazy_initialize.</span>default ()](#apidoc.element.core-decorators.lazy_initialize.default)
- description and source-code
```javascript
function lazyInitialize() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.memoize"></a>[module core-decorators.memoize](#apidoc.module.core-decorators.memoize)

#### <a name="apidoc.element.core-decorators.memoize.default"></a>[function <span class="apidocSignatureSpan">core-decorators.memoize.</span>default ()](#apidoc.element.core-decorators.memoize.default)
- description and source-code
```javascript
function memoize() {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.mixin"></a>[module core-decorators.mixin](#apidoc.module.core-decorators.mixin)

#### <a name="apidoc.element.core-decorators.mixin.default"></a>[function <span class="apidocSignatureSpan">core-decorators.mixin.</span>default ()](#apidoc.element.core-decorators.mixin.default)
- description and source-code
```javascript
function mixin() {
  for (var _len = arguments.length, mixins = Array(_len), _key = 0; _key < _len; _key++) {
    mixins[_key] = arguments[_key];
  }

  if (typeof mixins[0] === 'function') {
    return handleClass(mixins[0], []);
  } else {
    return function (target) {
      return handleClass(target, mixins);
    };
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.nonconfigurable"></a>[module core-decorators.nonconfigurable](#apidoc.module.core-decorators.nonconfigurable)

#### <a name="apidoc.element.core-decorators.nonconfigurable.default"></a>[function <span class="apidocSignatureSpan">core-decorators.nonconfigurable.</span>default ()](#apidoc.element.core-decorators.nonconfigurable.default)
- description and source-code
```javascript
function nonconfigurable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.nonenumerable"></a>[module core-decorators.nonenumerable](#apidoc.module.core-decorators.nonenumerable)

#### <a name="apidoc.element.core-decorators.nonenumerable.default"></a>[function <span class="apidocSignatureSpan">core-decorators.nonenumerable.</span>default ()](#apidoc.element.core-decorators.nonenumerable.default)
- description and source-code
```javascript
function nonenumerable() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.override"></a>[module core-decorators.override](#apidoc.module.core-decorators.override)

#### <a name="apidoc.element.core-decorators.override.default"></a>[function <span class="apidocSignatureSpan">core-decorators.override.</span>default ()](#apidoc.element.core-decorators.override.default)
- description and source-code
```javascript
function override() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.profile"></a>[module core-decorators.profile](#apidoc.module.core-decorators.profile)

#### <a name="apidoc.element.core-decorators.profile.default"></a>[function <span class="apidocSignatureSpan">core-decorators.profile.</span>default ()](#apidoc.element.core-decorators.profile.default)
- description and source-code
```javascript
function profile() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.readonly"></a>[module core-decorators.readonly](#apidoc.module.core-decorators.readonly)

#### <a name="apidoc.element.core-decorators.readonly.default"></a>[function <span class="apidocSignatureSpan">core-decorators.readonly.</span>default ()](#apidoc.element.core-decorators.readonly.default)
- description and source-code
```javascript
function readonly() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.suppress_warnings"></a>[module core-decorators.suppress_warnings](#apidoc.module.core-decorators.suppress_warnings)

#### <a name="apidoc.element.core-decorators.suppress_warnings.default"></a>[function <span class="apidocSignatureSpan">core-decorators.suppress_warnings.</span>default ()](#apidoc.element.core-decorators.suppress_warnings.default)
- description and source-code
```javascript
function suppressWarnings() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.throttle"></a>[module core-decorators.throttle](#apidoc.module.core-decorators.throttle)

#### <a name="apidoc.element.core-decorators.throttle.default"></a>[function <span class="apidocSignatureSpan">core-decorators.throttle.</span>default ()](#apidoc.element.core-decorators.throttle.default)
- description and source-code
```javascript
function throttle() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-decorators.time"></a>[module core-decorators.time](#apidoc.module.core-decorators.time)

#### <a name="apidoc.element.core-decorators.time.default"></a>[function <span class="apidocSignatureSpan">core-decorators.time.</span>default ()](#apidoc.element.core-decorators.time.default)
- description and source-code
```javascript
function time() {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return (0, _utils.decorate)(handleDescriptor, args);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
