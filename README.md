# npmdoc-quill

#### api documentation for  [quill (v1.2.4)](http://quilljs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-quill.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-quill) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-quill.svg)](https://travis-ci.org/npmdoc/node-npmdoc-quill)

#### Your powerful, rich text editor

[![NPM](https://nodei.co/npm/quill.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/quill)

- [https://npmdoc.github.io/node-npmdoc-quill/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-quill/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-quill/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-quill/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-quill/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-quill/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jason Chen"
    },
    "bugs": {
        "url": "https://github.com/quilljs/quill/issues"
    },
    "config": {
        "ports": {
            "proxy": "9000",
            "jekyll": "4000",
            "karma": "9876",
            "webpack": "9080"
        }
    },
    "dependencies": {
        "clone": "~2.1.1",
        "deep-equal": "~1.0.1",
        "eventemitter3": "~2.0.3",
        "extend": "~3.0.0",
        "parchment": "1.0.9",
        "quill-delta": "3.5.0"
    },
    "description": "Your powerful, rich text editor",
    "devDependencies": {
        "babel-core": "^6.24.1",
        "babel-loader": "^6.4.1",
        "babel-plugin-istanbul": "^4.1.1",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.24.1",
        "babel-preset-es2015": "^6.24.1",
        "css-loader": "~0.28.0",
        "eslint": "^3.19.0",
        "eslint-loader": "^1.7.1",
        "extract-text-webpack-plugin": "^2.1.0",
        "html-loader": "~0.4.5",
        "http-proxy": "^1.16.2",
        "jasmine-core": "^2.5.2",
        "karma": "^1.6.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.1.1",
        "karma-jasmine": "^1.1.0",
        "karma-sauce-launcher": "^1.1.0",
        "lodash": "^4.17.4",
        "style-loader": "~0.16.1",
        "stylus": "~0.54.5",
        "stylus-loader": "^3.0.1",
        "ts-loader": "^2.0.3",
        "typescript": "^2.2.2",
        "wdio-jasmine-framework": "~0.3.0",
        "wdio-spec-reporter": "~0.1.0",
        "webdriver-manager": "^12.0.4",
        "webdriverio": "^4.6.2",
        "webpack": "^2.4.1",
        "webpack-dev-server": "^2.4.2"
    },
    "directories": {},
    "dist": {
        "shasum": "2a822fb10f4346e63845b37637ee3d6bf0d20b65",
        "tarball": "https://registry.npmjs.org/quill/-/quill-1.2.4.tgz"
    },
    "files": [
        "assets",
        "blots",
        "core",
        "formats",
        "modules",
        "themes",
        "ui",
        "dist/quill.bubble.css",
        "dist/quill.snow.css",
        "dist/quill.core.css",
        "dist/quill.js",
        "dist/quill.core.js",
        "dist/quill.min.js.map",
        "dist/quill.min.js",
        "core.js",
        "quill.js"
    ],
    "gitHead": "706287fb2ce5ff22647fb71dc29bd2f07fa5b294",
    "homepage": "http://quilljs.com",
    "keywords": [
        "editor",
        "rich text",
        "wysiwyg"
    ],
    "license": "BSD-3-Clause",
    "main": "dist/quill.js",
    "maintainers": [
        {
            "name": "jhchen"
        }
    ],
    "name": "quill",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/quilljs/quill.git"
    },
    "scripts": {
        "build": "webpack --config _develop/webpack.config.js; rm dist/quill.core dist/quill.bubble dist/quill.snow;",
        "build:release": "./_develop/scripts/release.sh",
        "start": "npm run build; foreman start -f _develop/procfile",
        "test": "npm run test:unit",
        "test:all": "npm run test:unit; npm run test:functional",
        "test:coverage": "webpack --env.coverage --config _develop/webpack.config.js; karma start _develop/karma.config.js --reporters coverage",
        "test:functional": "./_develop/scripts/webdriver.sh",
        "test:unit": "npm run build; karma start _develop/karma.config.js",
        "travis": "karma start _develop/karma.config.js --reporters dots,saucelabs",
        "webdriver:start": "webdriver-manager start",
        "webdriver:update": "webdriver-manager update"
    },
    "version": "1.2.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
