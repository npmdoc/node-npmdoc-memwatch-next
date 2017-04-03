# api documentation for  [memwatch-next (v0.3.0)](https://github.com/marcominetti/node-memwatch#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-memwatch-next.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-memwatch-next) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-memwatch-next.svg)](https://travis-ci.org/npmdoc/node-npmdoc-memwatch-next)
#### Keep an eye on your memory usage, and discover and isolate leaks.

[![NPM](https://nodei.co/npm/memwatch-next.png?downloads=true)](https://www.npmjs.com/package/memwatch-next)

[![apidoc](https://npmdoc.github.io/node-npmdoc-memwatch-next/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-memwatch-next_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-memwatch-next/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-memwatch-next/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-memwatch-next/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Lloyd Hilaiel",
        "url": "http://lloyd.io"
    },
    "bugs": {
        "url": "https://github.com/marcominetti/node-memwatch/issues"
    },
    "contributors": [
        {
            "name": "Jed Parsons",
            "url": "@jedp"
        },
        {
            "name": "Jeff Haynie",
            "url": "@jhaynie"
        },
        {
            "name": "Justin Matthews",
            "url": "@jmatthewsr-ms"
        }
    ],
    "dependencies": {
        "bindings": "^1.2.1",
        "nan": "^2.3.2"
    },
    "description": "Keep an eye on your memory usage, and discover and isolate leaks.",
    "devDependencies": {
        "mocha": "^2.4.5",
        "should": "^8.3.1"
    },
    "directories": {},
    "dist": {
        "shasum": "2111050f9a906e0aa2d72a4ec0f0089c78726f8f",
        "tarball": "https://registry.npmjs.org/memwatch-next/-/memwatch-next-0.3.0.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "23b2da5b986b9f6db776e4a236437500a6ddbf68",
    "gypfile": true,
    "homepage": "https://github.com/marcominetti/node-memwatch#readme",
    "licenses": [
        {
            "type": "wtfpl"
        }
    ],
    "main": "include.js",
    "maintainers": [
        {
            "name": "marcominetti",
            "email": "marco.minetti@novetica.org"
        }
    ],
    "name": "memwatch-next",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/marcominetti/node-memwatch.git"
    },
    "scripts": {
        "install": "node-gyp rebuild",
        "test": "mocha tests --reporter spec"
    },
    "version": "0.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module memwatch-next](#apidoc.module.memwatch-next)
1.  [function <span class="apidocSignatureSpan">memwatch-next.</span>HeapDiff ()](#apidoc.element.memwatch-next.HeapDiff)
1.  [function <span class="apidocSignatureSpan">memwatch-next.</span>gc ()](#apidoc.element.memwatch-next.gc)
1.  number <span class="apidocSignatureSpan">memwatch-next.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">memwatch-next.</span>HeapDiff.prototype
1.  object <span class="apidocSignatureSpan">memwatch-next.</span>_events
1.  object <span class="apidocSignatureSpan">memwatch-next.</span>domain

#### [module memwatch-next.HeapDiff](#apidoc.module.memwatch-next.HeapDiff)
1.  [function <span class="apidocSignatureSpan">memwatch-next.</span>HeapDiff ()](#apidoc.element.memwatch-next.HeapDiff.HeapDiff)

#### [module memwatch-next.HeapDiff.prototype](#apidoc.module.memwatch-next.HeapDiff.prototype)
1.  [function <span class="apidocSignatureSpan">memwatch-next.HeapDiff.prototype.</span>end ()](#apidoc.element.memwatch-next.HeapDiff.prototype.end)



# <a name="apidoc.module.memwatch-next"></a>[module memwatch-next](#apidoc.module.memwatch-next)

#### <a name="apidoc.element.memwatch-next.HeapDiff"></a>[function <span class="apidocSignatureSpan">memwatch-next.</span>HeapDiff ()](#apidoc.element.memwatch-next.HeapDiff)
- description and source-code
```javascript
function HeapDiff() { [native code] }
```
- example usage
```shell
...

So far we have seen how 'memwatch' can aid in leak detection.  For
leak isolation, it provides a 'HeapDiff' class that takes two snapshots
and computes a diff between them.  For example:

'''javascript
// Take first snapshot
var hd = new memwatch.HeapDiff();

// do some things ...

// Take the second snapshot and compute the diff
var diff = hd.end();
'''
...
```

#### <a name="apidoc.element.memwatch-next.gc"></a>[function <span class="apidocSignatureSpan">memwatch-next.</span>gc ()](#apidoc.element.memwatch-next.gc)
- description and source-code
```javascript
function gc() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.memwatch-next.HeapDiff"></a>[module memwatch-next.HeapDiff](#apidoc.module.memwatch-next.HeapDiff)

#### <a name="apidoc.element.memwatch-next.HeapDiff.HeapDiff"></a>[function <span class="apidocSignatureSpan">memwatch-next.</span>HeapDiff ()](#apidoc.element.memwatch-next.HeapDiff.HeapDiff)
- description and source-code
```javascript
function HeapDiff() { [native code] }
```
- example usage
```shell
...

So far we have seen how 'memwatch' can aid in leak detection.  For
leak isolation, it provides a 'HeapDiff' class that takes two snapshots
and computes a diff between them.  For example:

'''javascript
// Take first snapshot
var hd = new memwatch.HeapDiff();

// do some things ...

// Take the second snapshot and compute the diff
var diff = hd.end();
'''
...
```



# <a name="apidoc.module.memwatch-next.HeapDiff.prototype"></a>[module memwatch-next.HeapDiff.prototype](#apidoc.module.memwatch-next.HeapDiff.prototype)

#### <a name="apidoc.element.memwatch-next.HeapDiff.prototype.end"></a>[function <span class="apidocSignatureSpan">memwatch-next.HeapDiff.prototype.</span>end ()](#apidoc.element.memwatch-next.HeapDiff.prototype.end)
- description and source-code
```javascript
function end() { [native code] }
```
- example usage
```shell
...
'''javascript
// Take first snapshot
var hd = new memwatch.HeapDiff();

// do some things ...

// Take the second snapshot and compute the diff
var diff = hd.end();
'''

The contents of 'diff' will look something like:

'''javascript
{
"before": { "nodes": 11625, "size_bytes": 1869904, "size": "1.78 mb" },
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
