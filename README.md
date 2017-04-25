# npmdoc-mssql

#### basic api documentation for  [mssql (v4.0.2)](https://github.com/patriksimek/node-mssql#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mssql.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mssql) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mssql.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mssql)

#### Microsoft SQL Server client for Node.js.

[![NPM](https://nodei.co/npm/mssql.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mssql)

- [https://npmdoc.github.io/node-npmdoc-mssql/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mssql/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mssql/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mssql/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mssql/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mssql/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Patrik Simek",
        "url": "https://patriksimek.cz"
    },
    "bin": {
        "mssql": "./bin/mssql"
    },
    "bugs": {
        "url": "https://github.com/patriksimek/node-mssql/issues"
    },
    "dependencies": {
        "debug": "^2.6.3",
        "generic-pool": "^3.1.7",
        "tedious": "^2.0.0"
    },
    "description": "Microsoft SQL Server client for Node.js.",
    "devDependencies": {
        "mocha": "^2.1.0",
        "standard": "^9.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "827c663b8657536e75a1df89fb7d8fc79cf31967",
        "tarball": "https://registry.npmjs.org/mssql/-/mssql-4.0.2.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "1a490f355969a995d17aafd5e217221c67127906",
    "homepage": "https://github.com/patriksimek/node-mssql#readme",
    "keywords": [
        "database",
        "mssql",
        "sql",
        "server",
        "msnodesql",
        "sqlserver",
        "tds",
        "node-tds",
        "tedious",
        "node-sqlserver",
        "sqlserver",
        "msnodesqlv8",
        "azure",
        "node-mssql"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "patriksimek"
        }
    ],
    "name": "mssql",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/patriksimek/node-mssql.git"
    },
    "scripts": {
        "test": "standard && node_modules/.bin/mocha test/common/unit.js",
        "test-cli": "mocha test/common/cli.js",
        "test-msnodesqlv8": "mocha test/msnodesqlv8",
        "test-tedious": "mocha test/tedious"
    },
    "version": "4.0.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
