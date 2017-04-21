# npmtest-v8-debug

#### basic test coverage for  [v8-debug (v1.0.1)](http://github.com/node-inspector/v8-debug)  [![npm package](https://img.shields.io/npm/v/npmtest-v8-debug.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-v8-debug) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-v8-debug.svg)](https://travis-ci.org/npmtest/node-npmtest-v8-debug)

#### v8 debugger extending API

[![NPM](https://nodei.co/npm/v8-debug.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/v8-debug)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-v8-debug/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-v8-debug/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-v8-debug/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-v8-debug/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-v8-debug/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-v8-debug/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-v8-debug/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-v8-debug/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-v8-debug/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-v8-debug/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-v8-debug/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-v8-debug/build/test-report.html](https://npmtest.github.io/node-npmtest-v8-debug/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-v8-debug/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-v8-debug/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-v8-debug/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-v8-debug/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-v8-debug/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-v8-debug/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-v8-debug/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-v8-debug/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "v8-debug",
    "version": "1.0.1",
    "description": "v8 debugger extending API",
    "homepage": "http://github.com/node-inspector/v8-debug",
    "author": "3y3 Ghoti <3y3@bk.ru>",
    "repository": {
        "type": "git",
        "url": "git://github.com/node-inspector/v8-debug.git"
    },
    "license": {
        "name": "BSD",
        "url": "https://github.com/node-inspector/v8-debug/blob/master/LICENSE"
    },
    "binary": {
        "module_name": "debug",
        "module_path": "./build/{module_name}/v{version}/{node_abi}-{platform}-{arch}/",
        "remote_path": "./{module_name}/v{version}/",
        "package_name": "{node_abi}-{platform}-{arch}.tar.gz",
        "host": "https://node-inspector.s3.amazonaws.com/"
    },
    "keywords": [
        "v8",
        "debugger"
    ],
    "engines": {
        "node": ">=0.10"
    },
    "main": "v8-debug",
    "dependencies": {
        "nan": "^2.3.2",
        "node-pre-gyp": "^0.6.5"
    },
    "devDependencies": {
        "aws-sdk": "^2.1.8",
        "mocha": "^2.1.0",
        "chai": "^1.10.0",
        "rimraf": "^2.4.4"
    },
    "scripts": {
        "preinstall": "node -e 'process.exit(0)'",
        "install": "node-pre-gyp install --fallback-to-build",
        "rebuild": "node-pre-gyp rebuild",
        "release": "node ./tools/release.js $@",
        "test": "mocha --debug"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
