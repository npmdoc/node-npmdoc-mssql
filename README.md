# api documentation for  [mssql (v3.3.0)](https://github.com/patriksimek/node-mssql#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mssql.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mssql)
#### Microsoft SQL Server client for Node.js.

[![NPM](https://nodei.co/npm/mssql.png?downloads=true)](https://www.npmjs.com/package/mssql)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mssql/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mssql_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mssql/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-mssql/build/screen-capture.npmPackageListing.svg)



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
        "generic-pool": "^2.2.0",
        "promise": "^7.0.1",
        "tedious": "~1.14.0"
    },
    "description": "Microsoft SQL Server client for Node.js.",
    "devDependencies": {
        "coffee-script": "^1.9.3",
        "mocha": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b6e6337ff123e87bf8aee1e6c8344b53ca5da856",
        "tarball": "https://registry.npmjs.org/mssql/-/mssql-3.3.0.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "817a555a37204edb63067967ae8f5b4b7e7491e3",
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
            "name": "patriksimek",
            "email": "patrik@patriksimek.cz"
        }
    ],
    "name": "mssql",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/patriksimek/node-mssql.git"
    },
    "scripts": {
        "compile": "coffee --compile --output ./lib ./src",
        "prepublish": "coffee --compile --output ./lib ./src",
        "test": "mocha test/unit",
        "test-cli": "mocha test/integration -g cli",
        "test-msnodesql": "mocha test/integration -g msnodesql",
        "test-msnodesqlv8": "mocha test/integration -g msnodesqlv8",
        "test-tds": "mocha test/integration -g tds",
        "test-tedious": "mocha test/integration -g tedious"
    },
    "version": "3.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mssql](#apidoc.module.mssql)
1.  boolean <span class="apidocSignatureSpan">mssql.</span>fix
1.  [function <span class="apidocSignatureSpan">mssql.</span>BIGINT ()](#apidoc.element.mssql.BIGINT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BINARY (length)](#apidoc.element.mssql.BINARY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BIT ()](#apidoc.element.mssql.BIT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit)
1.  [function <span class="apidocSignatureSpan">mssql.</span>CHAR (length)](#apidoc.element.mssql.CHAR)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Connection (config1, callback)](#apidoc.element.mssql.Connection)
1.  [function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DATE ()](#apidoc.element.mssql.DATE)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DATETIME ()](#apidoc.element.mssql.DATETIME)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DATETIME2 (scale)](#apidoc.element.mssql.DATETIME2)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DATETIMEOFFSET (scale)](#apidoc.element.mssql.DATETIMEOFFSET)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DECIMAL (precision, scale)](#apidoc.element.mssql.DECIMAL)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTimeOffset (scale)](#apidoc.element.mssql.DateTimeOffset)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal)
1.  [function <span class="apidocSignatureSpan">mssql.</span>FLOAT ()](#apidoc.element.mssql.FLOAT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float)
1.  [function <span class="apidocSignatureSpan">mssql.</span>GEOGRAPHY ()](#apidoc.element.mssql.GEOGRAPHY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>GEOMETRY ()](#apidoc.element.mssql.GEOMETRY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry)
1.  [function <span class="apidocSignatureSpan">mssql.</span>IMAGE ()](#apidoc.element.mssql.IMAGE)
1.  [function <span class="apidocSignatureSpan">mssql.</span>INT ()](#apidoc.element.mssql.INT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int)
1.  [function <span class="apidocSignatureSpan">mssql.</span>MONEY ()](#apidoc.element.mssql.MONEY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NCHAR (length)](#apidoc.element.mssql.NCHAR)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NTEXT ()](#apidoc.element.mssql.NTEXT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NUMERIC (precision, scale)](#apidoc.element.mssql.NUMERIC)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NVARCHAR (length)](#apidoc.element.mssql.NVARCHAR)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric)
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (connection)](#apidoc.element.mssql.PreparedStatement)
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Promise ()](#apidoc.element.mssql.Promise)
1.  [function <span class="apidocSignatureSpan">mssql.</span>REAL ()](#apidoc.element.mssql.REAL)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Request (connection)](#apidoc.element.mssql.Request)
1.  [function <span class="apidocSignatureSpan">mssql.</span>RequestError (message, code)](#apidoc.element.mssql.RequestError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SMALLDATETIME ()](#apidoc.element.mssql.SMALLDATETIME)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SMALLINT ()](#apidoc.element.mssql.SMALLINT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SMALLMONEY ()](#apidoc.element.mssql.SMALLMONEY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TEXT ()](#apidoc.element.mssql.TEXT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TIME (scale)](#apidoc.element.mssql.TIME)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TINYINT ()](#apidoc.element.mssql.TINYINT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Table (name)](#apidoc.element.mssql.Table)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Transaction (connection)](#apidoc.element.mssql.Transaction)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TransactionError (message, code)](#apidoc.element.mssql.TransactionError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>UNIQUEIDENTIFIER ()](#apidoc.element.mssql.UNIQUEIDENTIFIER)
1.  [function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VARBINARY (length)](#apidoc.element.mssql.VARBINARY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VARCHAR (length)](#apidoc.element.mssql.VARCHAR)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VARIANT ()](#apidoc.element.mssql.VARIANT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant)
1.  [function <span class="apidocSignatureSpan">mssql.</span>XML ()](#apidoc.element.mssql.XML)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml)
1.  [function <span class="apidocSignatureSpan">mssql.</span>batch ()](#apidoc.element.mssql.batch)
1.  [function <span class="apidocSignatureSpan">mssql.</span>close (callback)](#apidoc.element.mssql.close)
1.  [function <span class="apidocSignatureSpan">mssql.</span>connect (config, callback)](#apidoc.element.mssql.connect)
1.  [function <span class="apidocSignatureSpan">mssql.</span>init ()](#apidoc.element.mssql.init)
1.  [function <span class="apidocSignatureSpan">mssql.</span>on (event, handler)](#apidoc.element.mssql.on)
1.  [function <span class="apidocSignatureSpan">mssql.</span>query ()](#apidoc.element.mssql.query)
1.  number <span class="apidocSignatureSpan">mssql.</span>MAX
1.  object <span class="apidocSignatureSpan">mssql.</span>Connection.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>ConnectionError.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>DRIVERS
1.  object <span class="apidocSignatureSpan">mssql.</span>ISOLATION_LEVEL
1.  object <span class="apidocSignatureSpan">mssql.</span>PreparedStatement.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>Request.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>RequestError.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>TYPES
1.  object <span class="apidocSignatureSpan">mssql.</span>Table.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>Transaction.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>TransactionError.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>connection
1.  object <span class="apidocSignatureSpan">mssql.</span>connectionstring
1.  object <span class="apidocSignatureSpan">mssql.</span>datatypes
1.  object <span class="apidocSignatureSpan">mssql.</span>map
1.  object <span class="apidocSignatureSpan">mssql.</span>map.0
1.  object <span class="apidocSignatureSpan">mssql.</span>map.0.js.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>map.1
1.  object <span class="apidocSignatureSpan">mssql.</span>map.2
1.  object <span class="apidocSignatureSpan">mssql.</span>map.3
1.  object <span class="apidocSignatureSpan">mssql.</span>map.4
1.  object <span class="apidocSignatureSpan">mssql.</span>map.4.js.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>map.5
1.  object <span class="apidocSignatureSpan">mssql.</span>pool

#### [module mssql.BigInt](#apidoc.module.mssql.BigInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt.BigInt)
1.  [function <span class="apidocSignatureSpan">mssql.BigInt.</span>inspect ()](#apidoc.element.mssql.BigInt.inspect)
1.  string <span class="apidocSignatureSpan">mssql.BigInt.</span>declaration

#### [module mssql.Binary](#apidoc.module.mssql.Binary)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary.Binary)
1.  [function <span class="apidocSignatureSpan">mssql.Binary.</span>inspect ()](#apidoc.element.mssql.Binary.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Binary.</span>declaration

#### [module mssql.Bit](#apidoc.module.mssql.Bit)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit.Bit)
1.  [function <span class="apidocSignatureSpan">mssql.Bit.</span>inspect ()](#apidoc.element.mssql.Bit.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Bit.</span>declaration

#### [module mssql.Char](#apidoc.module.mssql.Char)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char.Char)
1.  [function <span class="apidocSignatureSpan">mssql.Char.</span>inspect ()](#apidoc.element.mssql.Char.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Char.</span>declaration

#### [module mssql.Connection](#apidoc.module.mssql.Connection)
1.  boolean <span class="apidocSignatureSpan">mssql.Connection.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">mssql.</span>Connection (config1, callback)](#apidoc.element.mssql.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.</span>EventEmitter ()](#apidoc.element.mssql.Connection.EventEmitter)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.</span>init ()](#apidoc.element.mssql.Connection.init)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Connection.listenerCount)
1.  number <span class="apidocSignatureSpan">mssql.Connection.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">mssql.Connection.</span>__super__

#### [module mssql.Connection.prototype](#apidoc.module.mssql.Connection.prototype)
1.  boolean <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>connected
1.  boolean <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>connecting
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_close (callback)](#apidoc.element.mssql.Connection.prototype._close)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_connect (callback)](#apidoc.element.mssql.Connection.prototype._connect)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_debug (msg)](#apidoc.element.mssql.Connection.prototype._debug)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>batch ()](#apidoc.element.mssql.Connection.prototype.batch)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>close (callback)](#apidoc.element.mssql.Connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>connect (callback)](#apidoc.element.mssql.Connection.prototype.connect)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>constructor (config1, callback)](#apidoc.element.mssql.Connection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>initializeDriver (driver)](#apidoc.element.mssql.Connection.prototype.initializeDriver)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>query ()](#apidoc.element.mssql.Connection.prototype.query)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>request ()](#apidoc.element.mssql.Connection.prototype.request)
1.  [function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>transaction ()](#apidoc.element.mssql.Connection.prototype.transaction)
1.  object <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>driver

#### [module mssql.ConnectionError](#apidoc.module.mssql.ConnectionError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError.ConnectionError)
1.  [function <span class="apidocSignatureSpan">mssql.ConnectionError.</span>captureStackTrace ()](#apidoc.element.mssql.ConnectionError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">mssql.ConnectionError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">mssql.ConnectionError.</span>__super__

#### [module mssql.ConnectionError.prototype](#apidoc.module.mssql.ConnectionError.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.ConnectionError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.ConnectionError.prototype.constructor)

#### [module mssql.Date](#apidoc.module.mssql.Date)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date.Date)
1.  [function <span class="apidocSignatureSpan">mssql.Date.</span>inspect ()](#apidoc.element.mssql.Date.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Date.</span>declaration

#### [module mssql.DateTime](#apidoc.module.mssql.DateTime)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime.DateTime)
1.  [function <span class="apidocSignatureSpan">mssql.DateTime.</span>inspect ()](#apidoc.element.mssql.DateTime.inspect)
1.  string <span class="apidocSignatureSpan">mssql.DateTime.</span>declaration

#### [module mssql.DateTime2](#apidoc.module.mssql.DateTime2)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2.DateTime2)
1.  [function <span class="apidocSignatureSpan">mssql.DateTime2.</span>inspect ()](#apidoc.element.mssql.DateTime2.inspect)
1.  string <span class="apidocSignatureSpan">mssql.DateTime2.</span>declaration

#### [module mssql.DateTimeOffset](#apidoc.module.mssql.DateTimeOffset)
1.  [function <span class="apidocSignatureSpan">mssql.</span>DateTimeOffset (scale)](#apidoc.element.mssql.DateTimeOffset.DateTimeOffset)
1.  [function <span class="apidocSignatureSpan">mssql.DateTimeOffset.</span>inspect ()](#apidoc.element.mssql.DateTimeOffset.inspect)
1.  string <span class="apidocSignatureSpan">mssql.DateTimeOffset.</span>declaration

#### [module mssql.Decimal](#apidoc.module.mssql.Decimal)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal.Decimal)
1.  [function <span class="apidocSignatureSpan">mssql.Decimal.</span>inspect ()](#apidoc.element.mssql.Decimal.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Decimal.</span>declaration

#### [module mssql.Float](#apidoc.module.mssql.Float)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float.Float)
1.  [function <span class="apidocSignatureSpan">mssql.Float.</span>inspect ()](#apidoc.element.mssql.Float.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Float.</span>declaration

#### [module mssql.Geography](#apidoc.module.mssql.Geography)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography.Geography)
1.  [function <span class="apidocSignatureSpan">mssql.Geography.</span>inspect ()](#apidoc.element.mssql.Geography.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Geography.</span>declaration

#### [module mssql.Geometry](#apidoc.module.mssql.Geometry)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry.Geometry)
1.  [function <span class="apidocSignatureSpan">mssql.Geometry.</span>inspect ()](#apidoc.element.mssql.Geometry.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Geometry.</span>declaration

#### [module mssql.Image](#apidoc.module.mssql.Image)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image.Image)
1.  [function <span class="apidocSignatureSpan">mssql.Image.</span>inspect ()](#apidoc.element.mssql.Image.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Image.</span>declaration

#### [module mssql.Int](#apidoc.module.mssql.Int)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int.Int)
1.  [function <span class="apidocSignatureSpan">mssql.Int.</span>inspect ()](#apidoc.element.mssql.Int.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Int.</span>declaration

#### [module mssql.Money](#apidoc.module.mssql.Money)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money.Money)
1.  [function <span class="apidocSignatureSpan">mssql.Money.</span>inspect ()](#apidoc.element.mssql.Money.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Money.</span>declaration

#### [module mssql.NChar](#apidoc.module.mssql.NChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar.NChar)
1.  [function <span class="apidocSignatureSpan">mssql.NChar.</span>inspect ()](#apidoc.element.mssql.NChar.inspect)
1.  string <span class="apidocSignatureSpan">mssql.NChar.</span>declaration

#### [module mssql.NText](#apidoc.module.mssql.NText)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText.NText)
1.  [function <span class="apidocSignatureSpan">mssql.NText.</span>inspect ()](#apidoc.element.mssql.NText.inspect)
1.  string <span class="apidocSignatureSpan">mssql.NText.</span>declaration

#### [module mssql.NVarChar](#apidoc.module.mssql.NVarChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar.NVarChar)
1.  [function <span class="apidocSignatureSpan">mssql.NVarChar.</span>inspect ()](#apidoc.element.mssql.NVarChar.inspect)
1.  string <span class="apidocSignatureSpan">mssql.NVarChar.</span>declaration

#### [module mssql.Numeric](#apidoc.module.mssql.Numeric)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric.Numeric)
1.  [function <span class="apidocSignatureSpan">mssql.Numeric.</span>inspect ()](#apidoc.element.mssql.Numeric.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Numeric.</span>declaration

#### [module mssql.PreparedStatement](#apidoc.module.mssql.PreparedStatement)
1.  boolean <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (connection)](#apidoc.element.mssql.PreparedStatement.PreparedStatement)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>EventEmitter ()](#apidoc.element.mssql.PreparedStatement.EventEmitter)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>init ()](#apidoc.element.mssql.PreparedStatement.init)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>listenerCount (emitter, type)](#apidoc.element.mssql.PreparedStatement.listenerCount)
1.  number <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>__super__

#### [module mssql.PreparedStatement.prototype](#apidoc.module.mssql.PreparedStatement.prototype)
1.  boolean <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_working
1.  boolean <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>multiple
1.  boolean <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>prepared
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_execute (values, callback)](#apidoc.element.mssql.PreparedStatement.prototype._execute)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_prepare (statement, callback)](#apidoc.element.mssql.PreparedStatement.prototype._prepare)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_unprepare (callback)](#apidoc.element.mssql.PreparedStatement.prototype._unprepare)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>constructor (connection)](#apidoc.element.mssql.PreparedStatement.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>execute (values, callback)](#apidoc.element.mssql.PreparedStatement.prototype.execute)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>input (name, type)](#apidoc.element.mssql.PreparedStatement.prototype.input)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>next ()](#apidoc.element.mssql.PreparedStatement.prototype.next)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>output (name, type)](#apidoc.element.mssql.PreparedStatement.prototype.output)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>prepare (statement, callback)](#apidoc.element.mssql.PreparedStatement.prototype.prepare)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>queue (callback)](#apidoc.element.mssql.PreparedStatement.prototype.queue)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>unprepare (callback)](#apidoc.element.mssql.PreparedStatement.prototype.unprepare)
1.  number <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_handle
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_pooledConnection
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_queue
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>connection
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>lastRequest
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>parameters
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>statement
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>stream
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>transaction

#### [module mssql.PreparedStatementError](#apidoc.module.mssql.PreparedStatementError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError.PreparedStatementError)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatementError.</span>captureStackTrace ()](#apidoc.element.mssql.PreparedStatementError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">mssql.PreparedStatementError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">mssql.PreparedStatementError.</span>__super__

#### [module mssql.PreparedStatementError.prototype](#apidoc.module.mssql.PreparedStatementError.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.PreparedStatementError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.PreparedStatementError.prototype.constructor)

#### [module mssql.Real](#apidoc.module.mssql.Real)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real.Real)
1.  [function <span class="apidocSignatureSpan">mssql.Real.</span>inspect ()](#apidoc.element.mssql.Real.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Real.</span>declaration

#### [module mssql.Request](#apidoc.module.mssql.Request)
1.  boolean <span class="apidocSignatureSpan">mssql.Request.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">mssql.</span>Request (connection)](#apidoc.element.mssql.Request.Request)
1.  [function <span class="apidocSignatureSpan">mssql.Request.</span>EventEmitter ()](#apidoc.element.mssql.Request.EventEmitter)
1.  [function <span class="apidocSignatureSpan">mssql.Request.</span>init ()](#apidoc.element.mssql.Request.init)
1.  [function <span class="apidocSignatureSpan">mssql.Request.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Request.listenerCount)
1.  number <span class="apidocSignatureSpan">mssql.Request.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">mssql.Request.</span>__super__

#### [module mssql.Request.prototype](#apidoc.module.mssql.Request.prototype)
1.  boolean <span class="apidocSignatureSpan">mssql.Request.prototype.</span>canceled
1.  boolean <span class="apidocSignatureSpan">mssql.Request.prototype.</span>multiple
1.  boolean <span class="apidocSignatureSpan">mssql.Request.prototype.</span>verbose
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_acquire (callback)](#apidoc.element.mssql.Request.prototype._acquire)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_batch (batch, callback)](#apidoc.element.mssql.Request.prototype._batch)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_bulk (table, callback)](#apidoc.element.mssql.Request.prototype._bulk)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_dedicated (connection)](#apidoc.element.mssql.Request.prototype._dedicated)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_execute (procedure, callback)](#apidoc.element.mssql.Request.prototype._execute)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_log (out)](#apidoc.element.mssql.Request.prototype._log)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_query (command, callback)](#apidoc.element.mssql.Request.prototype._query)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_release (connection)](#apidoc.element.mssql.Request.prototype._release)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_template (method, strings, values)](#apidoc.element.mssql.Request.prototype._template)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>batch (batch, callback)](#apidoc.element.mssql.Request.prototype.batch)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>bulk (table, callback)](#apidoc.element.mssql.Request.prototype.bulk)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>cancel ()](#apidoc.element.mssql.Request.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>constructor (connection)](#apidoc.element.mssql.Request.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>execute (command, callback)](#apidoc.element.mssql.Request.prototype.execute)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>input (name, type, value)](#apidoc.element.mssql.Request.prototype.input)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>output (name, type, value)](#apidoc.element.mssql.Request.prototype.output)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>pipe (stream)](#apidoc.element.mssql.Request.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>query (command, callback)](#apidoc.element.mssql.Request.prototype.query)
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>connection
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>parameters
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>pstatement
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>rowsAffected
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>stream
1.  object <span class="apidocSignatureSpan">mssql.Request.prototype.</span>transaction

#### [module mssql.RequestError](#apidoc.module.mssql.RequestError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>RequestError (message, code)](#apidoc.element.mssql.RequestError.RequestError)
1.  [function <span class="apidocSignatureSpan">mssql.RequestError.</span>captureStackTrace ()](#apidoc.element.mssql.RequestError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">mssql.RequestError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">mssql.RequestError.</span>__super__

#### [module mssql.RequestError.prototype](#apidoc.module.mssql.RequestError.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.RequestError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.RequestError.prototype.constructor)

#### [module mssql.SmallDateTime](#apidoc.module.mssql.SmallDateTime)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime.SmallDateTime)
1.  [function <span class="apidocSignatureSpan">mssql.SmallDateTime.</span>inspect ()](#apidoc.element.mssql.SmallDateTime.inspect)
1.  string <span class="apidocSignatureSpan">mssql.SmallDateTime.</span>declaration

#### [module mssql.SmallInt](#apidoc.module.mssql.SmallInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt.SmallInt)
1.  [function <span class="apidocSignatureSpan">mssql.SmallInt.</span>inspect ()](#apidoc.element.mssql.SmallInt.inspect)
1.  string <span class="apidocSignatureSpan">mssql.SmallInt.</span>declaration

#### [module mssql.SmallMoney](#apidoc.module.mssql.SmallMoney)
1.  [function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney.SmallMoney)
1.  [function <span class="apidocSignatureSpan">mssql.SmallMoney.</span>inspect ()](#apidoc.element.mssql.SmallMoney.inspect)
1.  string <span class="apidocSignatureSpan">mssql.SmallMoney.</span>declaration

#### [module mssql.TVP](#apidoc.module.mssql.TVP)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP.TVP)
1.  [function <span class="apidocSignatureSpan">mssql.TVP.</span>inspect ()](#apidoc.element.mssql.TVP.inspect)
1.  string <span class="apidocSignatureSpan">mssql.TVP.</span>declaration

#### [module mssql.TYPES](#apidoc.module.mssql.TYPES)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>BigInt ()](#apidoc.element.mssql.TYPES.BigInt)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Binary (length)](#apidoc.element.mssql.TYPES.Binary)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Bit ()](#apidoc.element.mssql.TYPES.Bit)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Char (length)](#apidoc.element.mssql.TYPES.Char)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Date ()](#apidoc.element.mssql.TYPES.Date)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime ()](#apidoc.element.mssql.TYPES.DateTime)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime2 (scale)](#apidoc.element.mssql.TYPES.DateTime2)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTimeOffset (scale)](#apidoc.element.mssql.TYPES.DateTimeOffset)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Decimal (precision, scale)](#apidoc.element.mssql.TYPES.Decimal)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Float ()](#apidoc.element.mssql.TYPES.Float)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geography ()](#apidoc.element.mssql.TYPES.Geography)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geometry ()](#apidoc.element.mssql.TYPES.Geometry)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Image ()](#apidoc.element.mssql.TYPES.Image)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Int ()](#apidoc.element.mssql.TYPES.Int)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Money ()](#apidoc.element.mssql.TYPES.Money)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>NChar (length)](#apidoc.element.mssql.TYPES.NChar)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>NText ()](#apidoc.element.mssql.TYPES.NText)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>NVarChar (length)](#apidoc.element.mssql.TYPES.NVarChar)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Numeric (precision, scale)](#apidoc.element.mssql.TYPES.Numeric)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Real ()](#apidoc.element.mssql.TYPES.Real)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallDateTime ()](#apidoc.element.mssql.TYPES.SmallDateTime)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallInt ()](#apidoc.element.mssql.TYPES.SmallInt)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallMoney ()](#apidoc.element.mssql.TYPES.SmallMoney)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>TVP (tvpType)](#apidoc.element.mssql.TYPES.TVP)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Text ()](#apidoc.element.mssql.TYPES.Text)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Time (scale)](#apidoc.element.mssql.TYPES.Time)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>TinyInt ()](#apidoc.element.mssql.TYPES.TinyInt)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>UDT ()](#apidoc.element.mssql.TYPES.UDT)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>UniqueIdentifier ()](#apidoc.element.mssql.TYPES.UniqueIdentifier)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarBinary (length)](#apidoc.element.mssql.TYPES.VarBinary)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarChar (length)](#apidoc.element.mssql.TYPES.VarChar)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Variant ()](#apidoc.element.mssql.TYPES.Variant)
1.  [function <span class="apidocSignatureSpan">mssql.TYPES.</span>Xml ()](#apidoc.element.mssql.TYPES.Xml)

#### [module mssql.Table](#apidoc.module.mssql.Table)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Table (name)](#apidoc.element.mssql.Table.Table)
1.  [function <span class="apidocSignatureSpan">mssql.Table.</span>fromRecordset (recordset, name)](#apidoc.element.mssql.Table.fromRecordset)
1.  [function <span class="apidocSignatureSpan">mssql.Table.</span>parseName (name)](#apidoc.element.mssql.Table.parseName)

#### [module mssql.Table.prototype](#apidoc.module.mssql.Table.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.Table.prototype.</span>_makeBulk ()](#apidoc.element.mssql.Table.prototype._makeBulk)
1.  [function <span class="apidocSignatureSpan">mssql.Table.prototype.</span>declare ()](#apidoc.element.mssql.Table.prototype.declare)

#### [module mssql.Text](#apidoc.module.mssql.Text)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text.Text)
1.  [function <span class="apidocSignatureSpan">mssql.Text.</span>inspect ()](#apidoc.element.mssql.Text.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Text.</span>declaration

#### [module mssql.Time](#apidoc.module.mssql.Time)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time.Time)
1.  [function <span class="apidocSignatureSpan">mssql.Time.</span>inspect ()](#apidoc.element.mssql.Time.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Time.</span>declaration

#### [module mssql.TinyInt](#apidoc.module.mssql.TinyInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt.TinyInt)
1.  [function <span class="apidocSignatureSpan">mssql.TinyInt.</span>inspect ()](#apidoc.element.mssql.TinyInt.inspect)
1.  string <span class="apidocSignatureSpan">mssql.TinyInt.</span>declaration

#### [module mssql.Transaction](#apidoc.module.mssql.Transaction)
1.  boolean <span class="apidocSignatureSpan">mssql.Transaction.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">mssql.</span>Transaction (connection)](#apidoc.element.mssql.Transaction.Transaction)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.</span>EventEmitter ()](#apidoc.element.mssql.Transaction.EventEmitter)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.</span>init ()](#apidoc.element.mssql.Transaction.init)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Transaction.listenerCount)
1.  number <span class="apidocSignatureSpan">mssql.Transaction.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">mssql.Transaction.</span>__super__

#### [module mssql.Transaction.prototype](#apidoc.module.mssql.Transaction.prototype)
1.  boolean <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_aborted
1.  boolean <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_working
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_abort ()](#apidoc.element.mssql.Transaction.prototype._abort)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_begin (isolationLevel, callback)](#apidoc.element.mssql.Transaction.prototype._begin)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_commit (callback)](#apidoc.element.mssql.Transaction.prototype._commit)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_rollback (callback)](#apidoc.element.mssql.Transaction.prototype._rollback)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>begin (isolationLevel, callback)](#apidoc.element.mssql.Transaction.prototype.begin)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>commit (callback)](#apidoc.element.mssql.Transaction.prototype.commit)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>constructor (connection)](#apidoc.element.mssql.Transaction.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>next ()](#apidoc.element.mssql.Transaction.prototype.next)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>queue (callback)](#apidoc.element.mssql.Transaction.prototype.queue)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>request ()](#apidoc.element.mssql.Transaction.prototype.request)
1.  [function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>rollback (callback)](#apidoc.element.mssql.Transaction.prototype.rollback)
1.  number <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>isolationLevel
1.  object <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_pooledConnection
1.  object <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_queue
1.  object <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>connection
1.  string <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>name

#### [module mssql.TransactionError](#apidoc.module.mssql.TransactionError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>TransactionError (message, code)](#apidoc.element.mssql.TransactionError.TransactionError)
1.  [function <span class="apidocSignatureSpan">mssql.TransactionError.</span>captureStackTrace ()](#apidoc.element.mssql.TransactionError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">mssql.TransactionError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">mssql.TransactionError.</span>__super__

#### [module mssql.TransactionError.prototype](#apidoc.module.mssql.TransactionError.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.TransactionError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.TransactionError.prototype.constructor)

#### [module mssql.UDT](#apidoc.module.mssql.UDT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT.UDT)
1.  [function <span class="apidocSignatureSpan">mssql.UDT.</span>inspect ()](#apidoc.element.mssql.UDT.inspect)
1.  string <span class="apidocSignatureSpan">mssql.UDT.</span>declaration

#### [module mssql.UniqueIdentifier](#apidoc.module.mssql.UniqueIdentifier)
1.  [function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier.UniqueIdentifier)
1.  [function <span class="apidocSignatureSpan">mssql.UniqueIdentifier.</span>inspect ()](#apidoc.element.mssql.UniqueIdentifier.inspect)
1.  string <span class="apidocSignatureSpan">mssql.UniqueIdentifier.</span>declaration

#### [module mssql.VarBinary](#apidoc.module.mssql.VarBinary)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary.VarBinary)
1.  [function <span class="apidocSignatureSpan">mssql.VarBinary.</span>inspect ()](#apidoc.element.mssql.VarBinary.inspect)
1.  string <span class="apidocSignatureSpan">mssql.VarBinary.</span>declaration

#### [module mssql.VarChar](#apidoc.module.mssql.VarChar)
1.  [function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar.VarChar)
1.  [function <span class="apidocSignatureSpan">mssql.VarChar.</span>inspect ()](#apidoc.element.mssql.VarChar.inspect)
1.  string <span class="apidocSignatureSpan">mssql.VarChar.</span>declaration

#### [module mssql.Variant](#apidoc.module.mssql.Variant)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant.Variant)
1.  [function <span class="apidocSignatureSpan">mssql.Variant.</span>inspect ()](#apidoc.element.mssql.Variant.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Variant.</span>declaration

#### [module mssql.Xml](#apidoc.module.mssql.Xml)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml.Xml)
1.  [function <span class="apidocSignatureSpan">mssql.Xml.</span>inspect ()](#apidoc.element.mssql.Xml.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Xml.</span>declaration

#### [module mssql.connectionstring](#apidoc.module.mssql.connectionstring)
1.  [function <span class="apidocSignatureSpan">mssql.connectionstring.</span>parse (string)](#apidoc.element.mssql.connectionstring.parse)
1.  [function <span class="apidocSignatureSpan">mssql.connectionstring.</span>resolve (string)](#apidoc.element.mssql.connectionstring.resolve)

#### [module mssql.datatypes](#apidoc.module.mssql.datatypes)
1.  [function <span class="apidocSignatureSpan">mssql.datatypes.</span>cast (value, type, options)](#apidoc.element.mssql.datatypes.cast)
1.  [function <span class="apidocSignatureSpan">mssql.datatypes.</span>declare (type, options)](#apidoc.element.mssql.datatypes.declare)
1.  object <span class="apidocSignatureSpan">mssql.datatypes.</span>DECLARATIONS
1.  object <span class="apidocSignatureSpan">mssql.datatypes.</span>TYPES

#### [module mssql.map](#apidoc.module.mssql.map)
1.  [function <span class="apidocSignatureSpan">mssql.map.</span>register (jstype, sqltype)](#apidoc.element.mssql.map.register)
1.  object <span class="apidocSignatureSpan">mssql.map.</span>0
1.  object <span class="apidocSignatureSpan">mssql.map.</span>1
1.  object <span class="apidocSignatureSpan">mssql.map.</span>2
1.  object <span class="apidocSignatureSpan">mssql.map.</span>3
1.  object <span class="apidocSignatureSpan">mssql.map.</span>4
1.  object <span class="apidocSignatureSpan">mssql.map.</span>5

#### [module mssql.map.0](#apidoc.module.mssql.map.0)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.</span>js ()](#apidoc.element.mssql.map.0.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.</span>sql (length)](#apidoc.element.mssql.map.0.sql)

#### [module mssql.map.0.js.prototype](#apidoc.module.mssql.map.0.js.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>entityify ()](#apidoc.element.mssql.map.0.js.prototype.entityify)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>isAlpha ( )](#apidoc.element.mssql.map.0.js.prototype.isAlpha)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>isDigit ()](#apidoc.element.mssql.map.0.js.prototype.isDigit)
1.  [function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>supplant (e)](#apidoc.element.mssql.map.0.js.prototype.supplant)

#### [module mssql.map.1](#apidoc.module.mssql.map.1)
1.  [function <span class="apidocSignatureSpan">mssql.map.1.</span>js ()](#apidoc.element.mssql.map.1.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.1.</span>sql ()](#apidoc.element.mssql.map.1.sql)

#### [module mssql.map.2](#apidoc.module.mssql.map.2)
1.  [function <span class="apidocSignatureSpan">mssql.map.2.</span>js ()](#apidoc.element.mssql.map.2.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.2.</span>sql ()](#apidoc.element.mssql.map.2.sql)

#### [module mssql.map.3](#apidoc.module.mssql.map.3)
1.  [function <span class="apidocSignatureSpan">mssql.map.3.</span>js ()](#apidoc.element.mssql.map.3.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.3.</span>sql ()](#apidoc.element.mssql.map.3.sql)

#### [module mssql.map.4](#apidoc.module.mssql.map.4)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.</span>js (arg, encodingOrOffset, length)](#apidoc.element.mssql.map.4.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.</span>sql (length)](#apidoc.element.mssql.map.4.sql)

#### [module mssql.map.4.js.prototype](#apidoc.module.mssql.map.4.js.prototype)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>asciiSlice ()](#apidoc.element.mssql.map.4.js.prototype.asciiSlice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>asciiWrite ()](#apidoc.element.mssql.map.4.js.prototype.asciiWrite)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>base64Slice ()](#apidoc.element.mssql.map.4.js.prototype.base64Slice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>base64Write ()](#apidoc.element.mssql.map.4.js.prototype.base64Write)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.mssql.map.4.js.prototype.compare)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>copy ()](#apidoc.element.mssql.map.4.js.prototype.copy)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>equals (other)](#apidoc.element.mssql.map.4.js.prototype.equals)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.mssql.map.4.js.prototype.fill)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>hexSlice ()](#apidoc.element.mssql.map.4.js.prototype.hexSlice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>hexWrite ()](#apidoc.element.mssql.map.4.js.prototype.hexWrite)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.includes)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>inspect ()](#apidoc.element.mssql.map.4.js.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>latin1Slice ()](#apidoc.element.mssql.map.4.js.prototype.latin1Slice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>latin1Write ()](#apidoc.element.mssql.map.4.js.prototype.latin1Write)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readDoubleBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readDoubleLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readFloatBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readFloatLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt16BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt16LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt32BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt32LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt8)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readIntBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readIntLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt16BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt16LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt32BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt32LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt8)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUIntBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUIntLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>slice (start, end)](#apidoc.element.mssql.map.4.js.prototype.slice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap16 ()](#apidoc.element.mssql.map.4.js.prototype.swap16)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap32 ()](#apidoc.element.mssql.map.4.js.prototype.swap32)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap64 ()](#apidoc.element.mssql.map.4.js.prototype.swap64)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toByteArray ()](#apidoc.element.mssql.map.4.js.prototype.toByteArray)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toJSON ()](#apidoc.element.mssql.map.4.js.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toString ()](#apidoc.element.mssql.map.4.js.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>ucs2Slice ()](#apidoc.element.mssql.map.4.js.prototype.ucs2Slice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>ucs2Write ()](#apidoc.element.mssql.map.4.js.prototype.ucs2Write)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>utf8Slice ()](#apidoc.element.mssql.map.4.js.prototype.utf8Slice)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>utf8Write ()](#apidoc.element.mssql.map.4.js.prototype.utf8Write)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.mssql.map.4.js.prototype.write)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeDoubleBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeDoubleLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeFloatBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeFloatLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt16BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt16LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt32BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt32LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt8)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeIntBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeIntLE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt16BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt16LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt32BE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt32LE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt8)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUIntBE)
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUIntLE)

#### [module mssql.map.5](#apidoc.module.mssql.map.5)
1.  [function <span class="apidocSignatureSpan">mssql.map.5.</span>js (name)](#apidoc.element.mssql.map.5.js)
1.  [function <span class="apidocSignatureSpan">mssql.map.5.</span>sql (tvpType)](#apidoc.element.mssql.map.5.sql)



# <a name="apidoc.module.mssql"></a>[module mssql](#apidoc.module.mssql)

#### <a name="apidoc.element.mssql.BIGINT"></a>[function <span class="apidocSignatureSpan">mssql.</span>BIGINT ()](#apidoc.element.mssql.BIGINT)
- description and source-code
```javascript
BIGINT = function () {
  return {
    type: TYPES.BigInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BINARY"></a>[function <span class="apidocSignatureSpan">mssql.</span>BINARY (length)](#apidoc.element.mssql.BINARY)
- description and source-code
```javascript
BINARY = function (length) {
  return {
    type: TYPES.Binary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BIT"></a>[function <span class="apidocSignatureSpan">mssql.</span>BIT ()](#apidoc.element.mssql.BIT)
- description and source-code
```javascript
BIT = function () {
  return {
    type: TYPES.Bit
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt)
- description and source-code
```javascript
BigInt = function () {
  return {
    type: TYPES.BigInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Binary"></a>[function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary)
- description and source-code
```javascript
Binary = function (length) {
  return {
    type: TYPES.Binary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Bit"></a>[function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit)
- description and source-code
```javascript
Bit = function () {
  return {
    type: TYPES.Bit
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.CHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>CHAR (length)](#apidoc.element.mssql.CHAR)
- description and source-code
```javascript
CHAR = function (length) {
  return {
    type: TYPES.Char,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Char"></a>[function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char)
- description and source-code
```javascript
Char = function (length) {
  return {
    type: TYPES.Char,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection"></a>[function <span class="apidocSignatureSpan">mssql.</span>Connection (config1, callback)](#apidoc.element.mssql.Connection)
- description and source-code
```javascript
function Connection(config1, callback) {
  var base, base1, base2, base3, base4, err, error, ex, ref1;
  this.config = config1;
  if ('string' === typeof this.config) {
    try {
      this.config = ConnectionString.resolve(this.config);
    } catch (error) {
      ex = error;
      if (callback) {
        return callback(ex);
      } else {
        throw ex;
      }
    }
  }
  if ((base = this.config).driver == null) {
    base.driver = 'tedious';
  }
  if ((base1 = this.config).port == null) {
    base1.port = 1433;
  }
  if ((base2 = this.config).options == null) {
    base2.options = {};
  }
  if ((base3 = this.config).stream == null) {
    base3.stream = false;
  }
  if ((base4 = this.config).parseJSON == null) {
    base4.parseJSON = false;
  }
  if (/^(.*)\\(.*)$/.exec(this.config.server)) {
    this.config.server = RegExp.$1;
    this.config.options.instanceName = RegExp.$2;
  }
  if (ref1 = this.config.driver, indexOf.call(DRIVERS, ref1) >= 0) {
    this.driver = this.initializeDriver(require("./" + this.config.driver));
    if (module.exports.fix) {
      this.driver.fix();
    }
  } else {
    err = new ConnectionError("Unknown driver " + this.config.driver + "!", 'EDRIVER');
    if (callback) {
      return callback(err);
    } else {
      throw err;
    }
  }
  if (callback) {
    this.connect(callback);
  }
}
```
- example usage
```shell
...
database: '...',

options: {
    encrypt: true // Use this if you're on Windows Azure
}
}

var connection1 = new sql.Connection(config, function(err) {
// ... error checks

// Query

var request = new sql.Request(connection1); // or: var request = connection1.request();
request.query('select 1 as number', function(err, recordset) {
    // ... error checks
...
```

#### <a name="apidoc.element.mssql.ConnectionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, code) {
  var err;
  if (!(this instanceof ConnectionError)) {
    if (message instanceof Error) {
      err = new ConnectionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new ConnectionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  ConnectionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATE"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATE ()](#apidoc.element.mssql.DATE)
- description and source-code
```javascript
DATE = function () {
  return {
    type: TYPES.Date
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIME ()](#apidoc.element.mssql.DATETIME)
- description and source-code
```javascript
DATETIME = function () {
  return {
    type: TYPES.DateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIME2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIME2 (scale)](#apidoc.element.mssql.DATETIME2)
- description and source-code
```javascript
DATETIME2 = function (scale) {
  return {
    type: TYPES.DateTime2,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIMEOFFSET"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIMEOFFSET (scale)](#apidoc.element.mssql.DATETIMEOFFSET)
- description and source-code
```javascript
DATETIMEOFFSET = function (scale) {
  return {
    type: TYPES.DateTimeOffset,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DECIMAL"></a>[function <span class="apidocSignatureSpan">mssql.</span>DECIMAL (precision, scale)](#apidoc.element.mssql.DECIMAL)
- description and source-code
```javascript
DECIMAL = function (precision, scale) {
  return {
    type: TYPES.Decimal,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Date"></a>[function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date)
- description and source-code
```javascript
Date = function () {
  return {
    type: TYPES.Date
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime)
- description and source-code
```javascript
DateTime = function () {
  return {
    type: TYPES.DateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2)
- description and source-code
```javascript
DateTime2 = function (scale) {
  return {
    type: TYPES.DateTime2,
    scale: scale
  };
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:

'''
sql.Bit
sql.BigInt
...
```

#### <a name="apidoc.element.mssql.DateTimeOffset"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTimeOffset (scale)](#apidoc.element.mssql.DateTimeOffset)
- description and source-code
```javascript
DateTimeOffset = function (scale) {
  return {
    type: TYPES.DateTimeOffset,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal)
- description and source-code
```javascript
Decimal = function (precision, scale) {
  return {
    type: TYPES.Decimal,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc");               // varchar(3)
request.input("name", sql.VarChar(50), "abc");           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc");      // varchar(MAX)
request.output("name", sql.VarChar);                     // varchar(8000)
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.FLOAT"></a>[function <span class="apidocSignatureSpan">mssql.</span>FLOAT ()](#apidoc.element.mssql.FLOAT)
- description and source-code
```javascript
FLOAT = function () {
  return {
    type: TYPES.Float
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Float"></a>[function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float)
- description and source-code
```javascript
Float = function () {
  return {
    type: TYPES.Float
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.GEOGRAPHY"></a>[function <span class="apidocSignatureSpan">mssql.</span>GEOGRAPHY ()](#apidoc.element.mssql.GEOGRAPHY)
- description and source-code
```javascript
GEOGRAPHY = function () {
  return {
    type: TYPES.Geography
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.GEOMETRY"></a>[function <span class="apidocSignatureSpan">mssql.</span>GEOMETRY ()](#apidoc.element.mssql.GEOMETRY)
- description and source-code
```javascript
GEOMETRY = function () {
  return {
    type: TYPES.Geometry
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geography"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography)
- description and source-code
```javascript
Geography = function () {
  return {
    type: TYPES.Geography
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry)
- description and source-code
```javascript
Geometry = function () {
  return {
    type: TYPES.Geometry
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.IMAGE"></a>[function <span class="apidocSignatureSpan">mssql.</span>IMAGE ()](#apidoc.element.mssql.IMAGE)
- description and source-code
```javascript
IMAGE = function () {
  return {
    type: TYPES.Image
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.INT"></a>[function <span class="apidocSignatureSpan">mssql.</span>INT ()](#apidoc.element.mssql.INT)
- description and source-code
```javascript
INT = function () {
  return {
    type: TYPES.Int
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Image"></a>[function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image)
- description and source-code
```javascript
Image = function () {
  return {
    type: TYPES.Image
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Int"></a>[function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int)
- description and source-code
```javascript
Int = function () {
  return {
    type: TYPES.Int
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.MONEY"></a>[function <span class="apidocSignatureSpan">mssql.</span>MONEY ()](#apidoc.element.mssql.MONEY)
- description and source-code
```javascript
MONEY = function () {
  return {
    type: TYPES.Money
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Money"></a>[function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money)
- description and source-code
```javascript
Money = function () {
  return {
    type: TYPES.Money
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>NCHAR (length)](#apidoc.element.mssql.NCHAR)
- description and source-code
```javascript
NCHAR = function (length) {
  return {
    type: TYPES.NChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar)
- description and source-code
```javascript
NChar = function (length) {
  return {
    type: TYPES.NChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NTEXT"></a>[function <span class="apidocSignatureSpan">mssql.</span>NTEXT ()](#apidoc.element.mssql.NTEXT)
- description and source-code
```javascript
NTEXT = function () {
  return {
    type: TYPES.NText
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NText"></a>[function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText)
- description and source-code
```javascript
NText = function () {
  return {
    type: TYPES.NText
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NUMERIC"></a>[function <span class="apidocSignatureSpan">mssql.</span>NUMERIC (precision, scale)](#apidoc.element.mssql.NUMERIC)
- description and source-code
```javascript
NUMERIC = function (precision, scale) {
  return {
    type: TYPES.Numeric,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVARCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVARCHAR (length)](#apidoc.element.mssql.NVARCHAR)
- description and source-code
```javascript
NVARCHAR = function (length) {
  return {
    type: TYPES.NVarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar)
- description and source-code
```javascript
NVarChar = function (length) {
  return {
    type: TYPES.NVarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric)
- description and source-code
```javascript
Numeric = function (precision, scale) {
  return {
    type: TYPES.Numeric,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (connection)](#apidoc.element.mssql.PreparedStatement)
- description and source-code
```javascript
function PreparedStatement(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this._queue = [];
  this.parameters = {};
}
```
- example usage
```shell
...
- EREQINPROG ('TransactionError') - Can't rollback transaction. There is a request in progress.

## Prepared Statement

**IMPORTANT:** always use 'PreparedStatement' class to create prepared statements - it ensures that all your executions of prepared
 statement are executed on one connection. Once you call 'prepare', a single connection is acquired from the connection pool and
 all subsequent executions are executed exclusively on this connection. Prepared Statement also contains a queue to make sure your
 executions are executed in series. After you call 'unprepare', the connection is then released back to the connection pool.

'''javascript
var ps = new sql.PreparedStatement(/* [connection] */);
'''

If you omit the connection argument, the global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.PreparedStatementError"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError)
- description and source-code
```javascript
function PreparedStatementError(message, code) {
  var err;
  if (!(this instanceof PreparedStatementError)) {
    if (message instanceof Error) {
      err = new PreparedStatementError(message.message, message.code);
      err.originalError = message;
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new PreparedStatementError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  this.code = code;
  PreparedStatementError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Promise"></a>[function <span class="apidocSignatureSpan">mssql.</span>Promise ()](#apidoc.element.mssql.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.REAL"></a>[function <span class="apidocSignatureSpan">mssql.</span>REAL ()](#apidoc.element.mssql.REAL)
- description and source-code
```javascript
REAL = function () {
  return {
    type: TYPES.Real
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Real"></a>[function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real)
- description and source-code
```javascript
Real = function () {
  return {
    type: TYPES.Real
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request"></a>[function <span class="apidocSignatureSpan">mssql.</span>Request (connection)](#apidoc.element.mssql.Request)
- description and source-code
```javascript
function Request(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof PreparedStatement) {
    this.pstatement = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this.parameters = {};
}
```
- example usage
```shell
...

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
// Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});

// Stored Procedure
...
```

#### <a name="apidoc.element.mssql.RequestError"></a>[function <span class="apidocSignatureSpan">mssql.</span>RequestError (message, code)](#apidoc.element.mssql.RequestError)
- description and source-code
```javascript
function RequestError(message, code) {
  var err, ref1, ref10, ref11, ref2, ref3, ref4, ref5, ref6, ref7, ref8, ref9;
  if (!(this instanceof RequestError)) {
    if (message instanceof Error) {
      err = new RequestError(message.message, (ref1 = message.code) != null ? ref1 : code);
      err.number = (ref2 = (ref3 = message.info) != null ? ref3.number : void 0) != null ? ref2 : message.code;
      err.lineNumber = (ref4 = message.info) != null ? ref4.lineNumber : void 0;
      err.state = (ref5 = (ref6 = message.info) != null ? ref6.state : void 0) != null ? ref5 : message.sqlstate;
      err["class"] = (ref7 = (ref8 = message.info) != null ? ref8["class"] : void 0) != null ? ref7 : (ref9 = message.info) != null
 ? ref9.severity : void 0;
      err.serverName = (ref10 = message.info) != null ? ref10.serverName : void 0;
      err.procName = (ref11 = message.info) != null ? ref11.procName : void 0;
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new RequestError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  RequestError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLDATETIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLDATETIME ()](#apidoc.element.mssql.SMALLDATETIME)
- description and source-code
```javascript
SMALLDATETIME = function () {
  return {
    type: TYPES.SmallDateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLINT"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLINT ()](#apidoc.element.mssql.SMALLINT)
- description and source-code
```javascript
SMALLINT = function () {
  return {
    type: TYPES.SmallInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLMONEY"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLMONEY ()](#apidoc.element.mssql.SMALLMONEY)
- description and source-code
```javascript
SMALLMONEY = function () {
  return {
    type: TYPES.SmallMoney
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime)
- description and source-code
```javascript
SmallDateTime = function () {
  return {
    type: TYPES.SmallDateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt)
- description and source-code
```javascript
SmallInt = function () {
  return {
    type: TYPES.SmallInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney)
- description and source-code
```javascript
SmallMoney = function () {
  return {
    type: TYPES.SmallMoney
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TEXT"></a>[function <span class="apidocSignatureSpan">mssql.</span>TEXT ()](#apidoc.element.mssql.TEXT)
- description and source-code
```javascript
TEXT = function () {
  return {
    type: TYPES.Text
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>TIME (scale)](#apidoc.element.mssql.TIME)
- description and source-code
```javascript
TIME = function (scale) {
  return {
    type: TYPES.Time,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TINYINT"></a>[function <span class="apidocSignatureSpan">mssql.</span>TINYINT ()](#apidoc.element.mssql.TINYINT)
- description and source-code
```javascript
TINYINT = function () {
  return {
    type: TYPES.TinyInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TVP"></a>[function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP)
- description and source-code
```javascript
TVP = function (tvpType) {
  return {
    type: TYPES.TVP,
    tvpType: tvpType
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Table"></a>[function <span class="apidocSignatureSpan">mssql.</span>Table (name)](#apidoc.element.mssql.Table)
- description and source-code
```javascript
function Table(name) {
  var ref1;
  if (name) {
    ref1 = Table.parseName(name), this.name = ref1.name, this.schema = ref1.schema, this.database = ref1.database;
    this.path = "" + (this.database ? "[" + this.database + "]." : "") + (this.schema ? "[" + this.schema + "]." : "") + "[" + this
.name + "]";
    this.temporary = this.name.charAt(0) === '#';
  }
  this.columns = [];
  this.rows = [];
  Object.defineProperty(this.columns, "add", {
    value: function(name, column, options) {
      if (options == null) {
        options = {};
      }
      if (column == null) {
        throw new Error("Column data type is not defined.");
      }
      if (column instanceof Function) {
        column = column();
      }
      column.name = name;
      column.nullable = options.nullable;
      column.primary = options.primary;
      return this.push(column);
    }
  });
  Object.defineProperty(this.rows, "add", {
    value: function() {
      var values;
      values = 1 <= arguments.length ? slice.call(arguments, 0) : [];
      return this.push(values);
    }
  });
}
```
- example usage
```shell
...

- **table** - 'sql.Table' instance.
- **callback(err, rowCount)** - A callback which is called after bulk insert has completed, or an error has occurred. Optional.
If omitted, returns [Promise](#promises).

__Example__

'''javascript
var table = new sql.Table('table_name'); // or temporary table, e.g. #temptable
table.create = true;
table.columns.add('a', sql.Int, {nullable: true, primary: true});
table.columns.add('b', sql.VarChar(50), {nullable: false});
table.rows.add(777, 'test');

var request = new sql.Request();
request.bulk(table, function(err, rowCount) {
...
```

#### <a name="apidoc.element.mssql.Text"></a>[function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text)
- description and source-code
```javascript
Text = function () {
  return {
    type: TYPES.Text
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Time"></a>[function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time)
- description and source-code
```javascript
Time = function (scale) {
  return {
    type: TYPES.Time,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt)
- description and source-code
```javascript
TinyInt = function () {
  return {
    type: TYPES.TinyInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction"></a>[function <span class="apidocSignatureSpan">mssql.</span>Transaction (connection)](#apidoc.element.mssql.Transaction)
- description and source-code
```javascript
function Transaction(connection) {
  this._abort = bind(this._abort, this);
  this.connection = connection != null ? connection : global_connection;
  this._queue = [];
}
```
- example usage
```shell
...
'''

## Transaction

**IMPORTANT:** always use 'Transaction' class to create transactions - it ensures that all your requests are executed on one connection
. Once you call 'begin', a single connection is acquired from the connection pool and all subsequent requests (initialized with
the 'Transaction' object) are executed exclusively on this connection. Transaction also contains a queue to make sure your requests
 are executed in series. After you call 'commit' or 'rollback', connection is then released back to the connection pool.

'''javascript
var transaction = new sql.Transaction(/* [connection] */);
'''

If you omit connection argument, global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.TransactionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>TransactionError (message, code)](#apidoc.element.mssql.TransactionError)
- description and source-code
```javascript
function TransactionError(message, code) {
  var err;
  if (!(this instanceof TransactionError)) {
    if (message instanceof Error) {
      err = new TransactionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new TransactionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  TransactionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UDT"></a>[function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT)
- description and source-code
```javascript
UDT = function () {
  return {
    type: TYPES.UDT
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UNIQUEIDENTIFIER"></a>[function <span class="apidocSignatureSpan">mssql.</span>UNIQUEIDENTIFIER ()](#apidoc.element.mssql.UNIQUEIDENTIFIER)
- description and source-code
```javascript
UNIQUEIDENTIFIER = function () {
  return {
    type: TYPES.UniqueIdentifier
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier = function () {
  return {
    type: TYPES.UniqueIdentifier
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARBINARY"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARBINARY (length)](#apidoc.element.mssql.VARBINARY)
- description and source-code
```javascript
VARBINARY = function (length) {
  return {
    type: TYPES.VarBinary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARCHAR (length)](#apidoc.element.mssql.VARCHAR)
- description and source-code
```javascript
VARCHAR = function (length) {
  return {
    type: TYPES.VarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARIANT"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARIANT ()](#apidoc.element.mssql.VARIANT)
- description and source-code
```javascript
VARIANT = function () {
  return {
    type: TYPES.Variant
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary)
- description and source-code
```javascript
VarBinary = function (length) {
  return {
    type: TYPES.VarBinary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar)
- description and source-code
```javascript
VarChar = function (length) {
  return {
    type: TYPES.VarChar,
    length: length
  };
}
```
- example usage
```shell
...
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.Variant"></a>[function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant)
- description and source-code
```javascript
Variant = function () {
  return {
    type: TYPES.Variant
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.XML"></a>[function <span class="apidocSignatureSpan">mssql.</span>XML ()](#apidoc.element.mssql.XML)
- description and source-code
```javascript
XML = function () {
  return {
    type: TYPES.Xml
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Xml"></a>[function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml)
- description and source-code
```javascript
Xml = function () {
  return {
    type: TYPES.Xml
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.batch"></a>[function <span class="apidocSignatureSpan">mssql.</span>batch ()](#apidoc.element.mssql.batch)
- description and source-code
```javascript
batch = function () {
  var strings, values;
  strings = arguments[0], values = 2 <= arguments.length ? slice.call(arguments, 1) : [];
  return new Request()._template('batch', strings, values);
}
```
- example usage
```shell
...
- **batch** - T-SQL command to be executed.
- **callback(err, recordset)** - A callback which is called after execution has completed, or an error has occurred. Optional. If
 omitted, returns [Promise](#promises).

__Example__

'''javascript
var request = new sql.Request();
request.batch('create procedure #temporary as select * from table', function(err, recordset) {
    // ... error checks
});
'''

__Errors__
- ETIMEOUT ('RequestError') - Request timeout.
- EREQUEST ('RequestError') - *Message from SQL Server*
...
```

#### <a name="apidoc.element.mssql.close"></a>[function <span class="apidocSignatureSpan">mssql.</span>close (callback)](#apidoc.element.mssql.close)
- description and source-code
```javascript
close = function (callback) {
  return global_connection != null ? global_connection.close(callback) : void 0;
}
```
- example usage
```shell
...
### close()

Close all active connections in the pool.

__Example__

'''javascript
connection.close();
'''

## Request

'''javascript
var request = new sql.Request(/* [connection] */);
'''
...
```

#### <a name="apidoc.element.mssql.connect"></a>[function <span class="apidocSignatureSpan">mssql.</span>connect (config, callback)](#apidoc.element.mssql.connect)
- description and source-code
```javascript
connect = function (config, callback) {
  global_connection = new Connection(config);
  return global_connection.connect(callback);
}
```
- example usage
```shell
...
    npm install mssql

## Quick Example

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
    // Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});
...
```

#### <a name="apidoc.element.mssql.init"></a>[function <span class="apidocSignatureSpan">mssql.</span>init ()](#apidoc.element.mssql.init)
- description and source-code
```javascript
init = function () {
  return module.exports.connect({
    user: module.exports.connection.userName,
    password: module.exports.connection.password,
    server: module.exports.connection.server,
    options: module.exports.connection.options,
    driver: 'tedious',
    pool: module.exports.pool
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.on"></a>[function <span class="apidocSignatureSpan">mssql.</span>on (event, handler)](#apidoc.element.mssql.on)
- description and source-code
```javascript
on = function (event, handler) {
  return global_connection != null ? global_connection.on(event, handler) : void 0;
}
```
- example usage
```shell
...
    .execute('procedure_name', function(err, recordsets, returnValue) {
        // ... error checks

        console.dir(recordsets);
    });
});

sql.on('error', function(err) {
	// ... error handler
});
'''

### Streaming

If you plan to work with large amount of rows, you should always use streaming. Once you enable this, you must listen for events
 to receive data.
...
```

#### <a name="apidoc.element.mssql.query"></a>[function <span class="apidocSignatureSpan">mssql.</span>query ()](#apidoc.element.mssql.query)
- description and source-code
```javascript
query = function () {
  var strings, values;
  strings = arguments[0], values = 2 <= arguments.length ? slice.call(arguments, 1) : [];
  return new Request()._template('query', strings, values);
}
```
- example usage
```shell
...

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
// Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});

// Stored Procedure
...
```



# <a name="apidoc.module.mssql.BigInt"></a>[module mssql.BigInt](#apidoc.module.mssql.BigInt)

#### <a name="apidoc.element.mssql.BigInt.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt.BigInt)
- description and source-code
```javascript
BigInt = function () {
  return {
    type: TYPES.BigInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BigInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.BigInt.</span>inspect ()](#apidoc.element.mssql.BigInt.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Binary"></a>[module mssql.Binary](#apidoc.module.mssql.Binary)

#### <a name="apidoc.element.mssql.Binary.Binary"></a>[function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary.Binary)
- description and source-code
```javascript
Binary = function (length) {
  return {
    type: TYPES.Binary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Binary.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Binary.</span>inspect ()](#apidoc.element.mssql.Binary.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Bit"></a>[module mssql.Bit](#apidoc.module.mssql.Bit)

#### <a name="apidoc.element.mssql.Bit.Bit"></a>[function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit.Bit)
- description and source-code
```javascript
Bit = function () {
  return {
    type: TYPES.Bit
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Bit.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Bit.</span>inspect ()](#apidoc.element.mssql.Bit.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Char"></a>[module mssql.Char](#apidoc.module.mssql.Char)

#### <a name="apidoc.element.mssql.Char.Char"></a>[function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char.Char)
- description and source-code
```javascript
Char = function (length) {
  return {
    type: TYPES.Char,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Char.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Char.</span>inspect ()](#apidoc.element.mssql.Char.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Connection"></a>[module mssql.Connection](#apidoc.module.mssql.Connection)

#### <a name="apidoc.element.mssql.Connection.Connection"></a>[function <span class="apidocSignatureSpan">mssql.</span>Connection (config1, callback)](#apidoc.element.mssql.Connection.Connection)
- description and source-code
```javascript
function Connection(config1, callback) {
  var base, base1, base2, base3, base4, err, error, ex, ref1;
  this.config = config1;
  if ('string' === typeof this.config) {
    try {
      this.config = ConnectionString.resolve(this.config);
    } catch (error) {
      ex = error;
      if (callback) {
        return callback(ex);
      } else {
        throw ex;
      }
    }
  }
  if ((base = this.config).driver == null) {
    base.driver = 'tedious';
  }
  if ((base1 = this.config).port == null) {
    base1.port = 1433;
  }
  if ((base2 = this.config).options == null) {
    base2.options = {};
  }
  if ((base3 = this.config).stream == null) {
    base3.stream = false;
  }
  if ((base4 = this.config).parseJSON == null) {
    base4.parseJSON = false;
  }
  if (/^(.*)\\(.*)$/.exec(this.config.server)) {
    this.config.server = RegExp.$1;
    this.config.options.instanceName = RegExp.$2;
  }
  if (ref1 = this.config.driver, indexOf.call(DRIVERS, ref1) >= 0) {
    this.driver = this.initializeDriver(require("./" + this.config.driver));
    if (module.exports.fix) {
      this.driver.fix();
    }
  } else {
    err = new ConnectionError("Unknown driver " + this.config.driver + "!", 'EDRIVER');
    if (callback) {
      return callback(err);
    } else {
      throw err;
    }
  }
  if (callback) {
    this.connect(callback);
  }
}
```
- example usage
```shell
...
database: '...',

options: {
    encrypt: true // Use this if you're on Windows Azure
}
}

var connection1 = new sql.Connection(config, function(err) {
// ... error checks

// Query

var request = new sql.Request(connection1); // or: var request = connection1.request();
request.query('select 1 as number', function(err, recordset) {
    // ... error checks
...
```

#### <a name="apidoc.element.mssql.Connection.EventEmitter"></a>[function <span class="apidocSignatureSpan">mssql.Connection.</span>EventEmitter ()](#apidoc.element.mssql.Connection.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.init"></a>[function <span class="apidocSignatureSpan">mssql.Connection.</span>init ()](#apidoc.element.mssql.Connection.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.listenerCount"></a>[function <span class="apidocSignatureSpan">mssql.Connection.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Connection.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Connection.prototype"></a>[module mssql.Connection.prototype](#apidoc.module.mssql.Connection.prototype)

#### <a name="apidoc.element.mssql.Connection.prototype._close"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_close (callback)](#apidoc.element.mssql.Connection.prototype._close)
- description and source-code
```javascript
_close = function (callback) {
  if (this._debugStream) {
    this._debugStream.removeAllListeners();
    this._debugStream.end();
    this._debugStream = null;
  }
  if (this.connecting) {
    this.connecting = false;
    this.driver.Connection.prototype.close.call(this, (function(_this) {
      return function(err) {
        return callback(err);
      };
    })(this));
    this.driver = null;
  } else if (this.connected) {
    this.connected = false;
    this.driver.Connection.prototype.close.call(this, (function(_this) {
      return function(err) {
        if (!err) {
          _this.connected = false;
          _this.emit('close');
        }
        return callback(err);
      };
    })(this));
    this.driver = null;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.prototype._connect"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_connect (callback)](#apidoc.element.mssql.Connection.prototype._connect)
- description and source-code
```javascript
_connect = function (callback) {
  var go;
  if (!this.driver) {
    return callback(new ConnectionError("Connection was closed. Create a new instance."));
  }
  if (this.connected) {
    return callback(new ConnectionError("Database is already connected! Call close before connecting to different database.", 'EALREADYCONNECTED
'));
  }
  if (this.connecting) {
    return callback(new ConnectionError("Already connecting to database! Call close before connecting to different database.", '
EALREADYCONNECTING'));
  }
  go = (function(_this) {
    return function() {
      _this.connecting = true;
      return _this.driver.Connection.prototype.connect.call(_this, _this.config, function(err) {
        if (!_this.connecting) {
          return;
        }
        _this.connecting = false;
        if (err) {
          if (_this._debugStream) {
            _this._debugStream.removeAllListeners();
            _this._debugStream.end();
            _this._debugStream = null;
          }
        } else {
          _this.connected = true;
          _this.emit('connect');
        }
        return callback(err);
      });
    };
  })(this);
  if (this.config.debug) {
    this._debugStream = fs.createWriteStream("./mssql_debug_" + (Date.now()) + ".log");
    this._debugStream.once('open', go);
    this._debugStream.on('error', function(err) {
      if (this.connecting || this.connected) {
        return console.error(err.stack);
      } else {
        this._debugStream.removeListener('open', go);
        return callback(new ConnectionError("Failed to open debug stream. " + err.message, 'EDEBUG'));
      }
    });
  } else {
    go();
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.prototype._debug"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>_debug (msg)](#apidoc.element.mssql.Connection.prototype._debug)
- description and source-code
```javascript
_debug = function (msg) {
  var ref1;
  return (ref1 = this._debugStream) != null ? ref1.write((String(msg).replace(/\x1B\[[0-9;]*m/g, '')) + "\n") : void 0;
}
```
- example usage
```shell
...
        c.hasError = true;
        return;
      }
      return _this.emit('error', err);
    });
    if (config.debug) {
      return c.on('debug', function(msg) {
        return _this._debug(msg);
      });
    }
  };
})(this),
validate: function(c) {
  return (c != null) && !c.closed && !c.hasError;
},
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.batch"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>batch ()](#apidoc.element.mssql.Connection.prototype.batch)
- description and source-code
```javascript
batch = function () {
  var strings, values;
  strings = arguments[0], values = 2 <= arguments.length ? slice.call(arguments, 1) : [];
  return new Request(this)._template('batch', strings, values);
}
```
- example usage
```shell
...
- **batch** - T-SQL command to be executed.
- **callback(err, recordset)** - A callback which is called after execution has completed, or an error has occurred. Optional. If
 omitted, returns [Promise](#promises).

__Example__

'''javascript
var request = new sql.Request();
request.batch('create procedure #temporary as select * from table', function(err, recordset) {
    // ... error checks
});
'''

__Errors__
- ETIMEOUT ('RequestError') - Request timeout.
- EREQUEST ('RequestError') - *Message from SQL Server*
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.close"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>close (callback)](#apidoc.element.mssql.Connection.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  if (callback != null) {
    return this._close(callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._close(function(err) {
        if (err) {
          return reject(err);
        }
        return resolve();
      });
    };
  })(this));
}
```
- example usage
```shell
...
### close()

Close all active connections in the pool.

__Example__

'''javascript
connection.close();
'''

## Request

'''javascript
var request = new sql.Request(/* [connection] */);
'''
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.connect"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>connect (callback)](#apidoc.element.mssql.Connection.prototype.connect)
- description and source-code
```javascript
connect = function (callback) {
  if (callback != null) {
    return this._connect(callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._connect(function(err) {
        if (err) {
          return reject(err);
        }
        return resolve(_this);
      });
    };
  })(this));
}
```
- example usage
```shell
...
    npm install mssql

## Quick Example

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
    // Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>constructor (config1, callback)](#apidoc.element.mssql.Connection.prototype.constructor)
- description and source-code
```javascript
function Connection(config1, callback) {
  var base, base1, base2, base3, base4, err, error, ex, ref1;
  this.config = config1;
  if ('string' === typeof this.config) {
    try {
      this.config = ConnectionString.resolve(this.config);
    } catch (error) {
      ex = error;
      if (callback) {
        return callback(ex);
      } else {
        throw ex;
      }
    }
  }
  if ((base = this.config).driver == null) {
    base.driver = 'tedious';
  }
  if ((base1 = this.config).port == null) {
    base1.port = 1433;
  }
  if ((base2 = this.config).options == null) {
    base2.options = {};
  }
  if ((base3 = this.config).stream == null) {
    base3.stream = false;
  }
  if ((base4 = this.config).parseJSON == null) {
    base4.parseJSON = false;
  }
  if (/^(.*)\\(.*)$/.exec(this.config.server)) {
    this.config.server = RegExp.$1;
    this.config.options.instanceName = RegExp.$2;
  }
  if (ref1 = this.config.driver, indexOf.call(DRIVERS, ref1) >= 0) {
    this.driver = this.initializeDriver(require("./" + this.config.driver));
    if (module.exports.fix) {
      this.driver.fix();
    }
  } else {
    err = new ConnectionError("Unknown driver " + this.config.driver + "!", 'EDRIVER');
    if (callback) {
      return callback(err);
    } else {
      throw err;
    }
  }
  if (callback) {
    this.connect(callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.prototype.initializeDriver"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>initializeDriver (driver)](#apidoc.element.mssql.Connection.prototype.initializeDriver)
- description and source-code
```javascript
initializeDriver = function (driver) {
  return driver(Connection, Transaction, Request, ConnectionError, TransactionError, RequestError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Connection.prototype.query"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>query ()](#apidoc.element.mssql.Connection.prototype.query)
- description and source-code
```javascript
query = function () {
  var strings, values;
  strings = arguments[0], values = 2 <= arguments.length ? slice.call(arguments, 1) : [];
  return new Request(this)._template('query', strings, values);
}
```
- example usage
```shell
...

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
// Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});

// Stored Procedure
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.request"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>request ()](#apidoc.element.mssql.Connection.prototype.request)
- description and source-code
```javascript
request = function () {
  return new Request(this);
}
```
- example usage
```shell
...
}

var connection1 = new sql.Connection(config, function(err) {
    // ... error checks

    // Query

    var request = new sql.Request(connection1); // or: var request = connection1.request();
    request.query('select 1 as number', function(err, recordset) {
        // ... error checks

        console.dir(recordset);
    });

});
...
```

#### <a name="apidoc.element.mssql.Connection.prototype.transaction"></a>[function <span class="apidocSignatureSpan">mssql.Connection.prototype.</span>transaction ()](#apidoc.element.mssql.Connection.prototype.transaction)
- description and source-code
```javascript
transaction = function () {
  return new Transaction(this);
}
```
- example usage
```shell
...

            console.log("Transaction committed.");
        });
    });
});
'''

Transaction can also be created by 'var transaction = connection.transaction();'. Requests can also be created by 'var request =
transaction.request();'.

__Aborted transactions__

This example shows how you should correctly handle transaction errors when 'abortTransactionOnError' ('XACT_ABORT') is enabled.
Added in 2.0.

'''javascript
var transaction = new sql.Transaction(/* [connection] */);
...
```



# <a name="apidoc.module.mssql.ConnectionError"></a>[module mssql.ConnectionError](#apidoc.module.mssql.ConnectionError)

#### <a name="apidoc.element.mssql.ConnectionError.ConnectionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, code) {
  var err;
  if (!(this instanceof ConnectionError)) {
    if (message instanceof Error) {
      err = new ConnectionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new ConnectionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  ConnectionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.ConnectionError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">mssql.ConnectionError.</span>captureStackTrace ()](#apidoc.element.mssql.ConnectionError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.ConnectionError.prototype"></a>[module mssql.ConnectionError.prototype](#apidoc.module.mssql.ConnectionError.prototype)

#### <a name="apidoc.element.mssql.ConnectionError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.ConnectionError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.ConnectionError.prototype.constructor)
- description and source-code
```javascript
function ConnectionError(message, code) {
  var err;
  if (!(this instanceof ConnectionError)) {
    if (message instanceof Error) {
      err = new ConnectionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new ConnectionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  ConnectionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Date"></a>[module mssql.Date](#apidoc.module.mssql.Date)

#### <a name="apidoc.element.mssql.Date.Date"></a>[function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date.Date)
- description and source-code
```javascript
Date = function () {
  return {
    type: TYPES.Date
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Date.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Date.</span>inspect ()](#apidoc.element.mssql.Date.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.DateTime"></a>[module mssql.DateTime](#apidoc.module.mssql.DateTime)

#### <a name="apidoc.element.mssql.DateTime.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime.DateTime)
- description and source-code
```javascript
DateTime = function () {
  return {
    type: TYPES.DateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime.inspect"></a>[function <span class="apidocSignatureSpan">mssql.DateTime.</span>inspect ()](#apidoc.element.mssql.DateTime.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.DateTime2"></a>[module mssql.DateTime2](#apidoc.module.mssql.DateTime2)

#### <a name="apidoc.element.mssql.DateTime2.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2.DateTime2)
- description and source-code
```javascript
DateTime2 = function (scale) {
  return {
    type: TYPES.DateTime2,
    scale: scale
  };
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:

'''
sql.Bit
sql.BigInt
...
```

#### <a name="apidoc.element.mssql.DateTime2.inspect"></a>[function <span class="apidocSignatureSpan">mssql.DateTime2.</span>inspect ()](#apidoc.element.mssql.DateTime2.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.DateTimeOffset"></a>[module mssql.DateTimeOffset](#apidoc.module.mssql.DateTimeOffset)

#### <a name="apidoc.element.mssql.DateTimeOffset.DateTimeOffset"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTimeOffset (scale)](#apidoc.element.mssql.DateTimeOffset.DateTimeOffset)
- description and source-code
```javascript
DateTimeOffset = function (scale) {
  return {
    type: TYPES.DateTimeOffset,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTimeOffset.inspect"></a>[function <span class="apidocSignatureSpan">mssql.DateTimeOffset.</span>inspect ()](#apidoc.element.mssql.DateTimeOffset.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Decimal"></a>[module mssql.Decimal](#apidoc.module.mssql.Decimal)

#### <a name="apidoc.element.mssql.Decimal.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal.Decimal)
- description and source-code
```javascript
Decimal = function (precision, scale) {
  return {
    type: TYPES.Decimal,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc");               // varchar(3)
request.input("name", sql.VarChar(50), "abc");           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc");      // varchar(MAX)
request.output("name", sql.VarChar);                     // varchar(8000)
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.Decimal.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Decimal.</span>inspect ()](#apidoc.element.mssql.Decimal.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Float"></a>[module mssql.Float](#apidoc.module.mssql.Float)

#### <a name="apidoc.element.mssql.Float.Float"></a>[function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float.Float)
- description and source-code
```javascript
Float = function () {
  return {
    type: TYPES.Float
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Float.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Float.</span>inspect ()](#apidoc.element.mssql.Float.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Geography"></a>[module mssql.Geography](#apidoc.module.mssql.Geography)

#### <a name="apidoc.element.mssql.Geography.Geography"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography.Geography)
- description and source-code
```javascript
Geography = function () {
  return {
    type: TYPES.Geography
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geography.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Geography.</span>inspect ()](#apidoc.element.mssql.Geography.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Geometry"></a>[module mssql.Geometry](#apidoc.module.mssql.Geometry)

#### <a name="apidoc.element.mssql.Geometry.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry.Geometry)
- description and source-code
```javascript
Geometry = function () {
  return {
    type: TYPES.Geometry
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geometry.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Geometry.</span>inspect ()](#apidoc.element.mssql.Geometry.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Image"></a>[module mssql.Image](#apidoc.module.mssql.Image)

#### <a name="apidoc.element.mssql.Image.Image"></a>[function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image.Image)
- description and source-code
```javascript
Image = function () {
  return {
    type: TYPES.Image
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Image.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Image.</span>inspect ()](#apidoc.element.mssql.Image.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Int"></a>[module mssql.Int](#apidoc.module.mssql.Int)

#### <a name="apidoc.element.mssql.Int.Int"></a>[function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int.Int)
- description and source-code
```javascript
Int = function () {
  return {
    type: TYPES.Int
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Int.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Int.</span>inspect ()](#apidoc.element.mssql.Int.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Money"></a>[module mssql.Money](#apidoc.module.mssql.Money)

#### <a name="apidoc.element.mssql.Money.Money"></a>[function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money.Money)
- description and source-code
```javascript
Money = function () {
  return {
    type: TYPES.Money
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Money.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Money.</span>inspect ()](#apidoc.element.mssql.Money.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.NChar"></a>[module mssql.NChar](#apidoc.module.mssql.NChar)

#### <a name="apidoc.element.mssql.NChar.NChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar.NChar)
- description and source-code
```javascript
NChar = function (length) {
  return {
    type: TYPES.NChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NChar.</span>inspect ()](#apidoc.element.mssql.NChar.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.NText"></a>[module mssql.NText](#apidoc.module.mssql.NText)

#### <a name="apidoc.element.mssql.NText.NText"></a>[function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText.NText)
- description and source-code
```javascript
NText = function () {
  return {
    type: TYPES.NText
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NText.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NText.</span>inspect ()](#apidoc.element.mssql.NText.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.NVarChar"></a>[module mssql.NVarChar](#apidoc.module.mssql.NVarChar)

#### <a name="apidoc.element.mssql.NVarChar.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar.NVarChar)
- description and source-code
```javascript
NVarChar = function (length) {
  return {
    type: TYPES.NVarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVarChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NVarChar.</span>inspect ()](#apidoc.element.mssql.NVarChar.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Numeric"></a>[module mssql.Numeric](#apidoc.module.mssql.Numeric)

#### <a name="apidoc.element.mssql.Numeric.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric.Numeric)
- description and source-code
```javascript
Numeric = function (precision, scale) {
  return {
    type: TYPES.Numeric,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Numeric.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Numeric.</span>inspect ()](#apidoc.element.mssql.Numeric.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.PreparedStatement"></a>[module mssql.PreparedStatement](#apidoc.module.mssql.PreparedStatement)

#### <a name="apidoc.element.mssql.PreparedStatement.PreparedStatement"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (connection)](#apidoc.element.mssql.PreparedStatement.PreparedStatement)
- description and source-code
```javascript
function PreparedStatement(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this._queue = [];
  this.parameters = {};
}
```
- example usage
```shell
...
- EREQINPROG ('TransactionError') - Can't rollback transaction. There is a request in progress.

## Prepared Statement

**IMPORTANT:** always use 'PreparedStatement' class to create prepared statements - it ensures that all your executions of prepared
 statement are executed on one connection. Once you call 'prepare', a single connection is acquired from the connection pool and
 all subsequent executions are executed exclusively on this connection. Prepared Statement also contains a queue to make sure your
 executions are executed in series. After you call 'unprepare', the connection is then released back to the connection pool.

'''javascript
var ps = new sql.PreparedStatement(/* [connection] */);
'''

If you omit the connection argument, the global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.PreparedStatement.EventEmitter"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>EventEmitter ()](#apidoc.element.mssql.PreparedStatement.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.init"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>init ()](#apidoc.element.mssql.PreparedStatement.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.listenerCount"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.</span>listenerCount (emitter, type)](#apidoc.element.mssql.PreparedStatement.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.PreparedStatement.prototype"></a>[module mssql.PreparedStatement.prototype](#apidoc.module.mssql.PreparedStatement.prototype)

#### <a name="apidoc.element.mssql.PreparedStatement.prototype._execute"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_execute (values, callback)](#apidoc.element.mssql.PreparedStatement.prototype._execute)
- description and source-code
```javascript
_execute = function (values, callback) {
  var name, param, ref1, req;
  req = this.lastRequest = new Request(this);
  if (this.stream != null) {
    req.stream = this.stream;
  }
  req.input('handle', TYPES.Int, this._handle);
  ref1 = this.parameters;
  for (name in ref1) {
    param = ref1[name];
    req.parameters[name] = {
      name: name,
      type: param.type,
      io: param.io,
      value: values[name],
      length: param.length,
      scale: param.scale,
      precision: param.precision
    };
  }
  req.execute('sp_execute', (function(_this) {
    return function(err, recordsets, returnValue) {
      if (err) {
        return callback(err);
      }
      return callback(null, (_this.multiple ? recordsets : recordsets[0]), req.rowsAffected);
    };
  })(this));
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype._prepare"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_prepare (statement, callback)](#apidoc.element.mssql.PreparedStatement.prototype._prepare)
- description and source-code
```javascript
_prepare = function (statement, callback) {
  var done;
  if (this._pooledConnection) {
    callback(new PreparedStatementError("Statement is already prepared.", 'EALREADYPREPARED'));
    return this;
  }
  if (typeof statement === 'function') {
    callback = statement;
    statement = void 0;
  }
  if (statement != null) {
    this.statement = statement;
  }
  done = (function(_this) {
    return function(err, connection) {
      var name, param, req;
      if (err) {
        return callback(err);
      }
      _this._pooledConnection = connection;
      req = new Request(_this);
      req.stream = false;
      req.output('handle', TYPES.Int);
      req.input('params', TYPES.NVarChar, ((function() {
        var ref1, results;
        ref1 = this.parameters;
        results = [];
        for (name in ref1) {
          param = ref1[name];
          results.push("@" + name + " " + (declare(param.type, param)) + (param.io === 2 ? " output" : ""));
        }
        return results;
      }).call(_this)).join(','));
      req.input('stmt', TYPES.NVarChar, _this.statement);
      return req.execute('sp_prepare', function(err) {
        if (err) {
          if (_this.transaction) {
            _this.transaction.next();
          } else {
            _this.connection.pool.release(_this._pooledConnection);
            _this._pooledConnection = null;
          }
          return callback(err);
        }
        _this._handle = req.parameters.handle.value;
        return callback(null);
      });
    };
  })(this);
  if (this.transaction) {
    if (!this.transaction._pooledConnection) {
      callback(new TransactionError("Transaction has not begun. Call begin() first.", 'ENOTBEGUN'));
      return this;
    }
    this.transaction.queue(done);
  } else {
    this.connection.pool.acquire(done);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype._unprepare"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>_unprepare (callback)](#apidoc.element.mssql.PreparedStatement.prototype._unprepare)
- description and source-code
```javascript
_unprepare = function (callback) {
  var done, req;
  if (!this._pooledConnection) {
    callback(new PreparedStatementError("Statement is not prepared. Call prepare() first.", 'ENOTPREPARED'));
    return this;
  }
  done = (function(_this) {
    return function(err) {
      if (err) {
        return callback(err);
      }
      if (_this.transaction) {
        _this.transaction.next();
      } else {
        _this.connection.pool.release(_this._pooledConnection);
        _this._pooledConnection = null;
      }
      _this._handle = 0;
      return callback(null);
    };
  })(this);
  req = new Request(this);
  req.stream = false;
  req.input('handle', TYPES.Int, this._handle);
  req.execute('sp_unprepare', done);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>constructor (connection)](#apidoc.element.mssql.PreparedStatement.prototype.constructor)
- description and source-code
```javascript
function PreparedStatement(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this._queue = [];
  this.parameters = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.execute"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>execute (values, callback)](#apidoc.element.mssql.PreparedStatement.prototype.execute)
- description and source-code
```javascript
execute = function (values, callback) {
  if (callback != null) {
    return this._execute(values, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._execute(values, function(err, recordset) {
        if (err) {
          return reject(err);
        }
        return resolve(recordset);
      });
    };
  })(this));
}
```
- example usage
```shell
...
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.input"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>input (name, type)](#apidoc.element.mssql.PreparedStatement.prototype.input)
- description and source-code
```javascript
input = function (name, type) {
  if (/(--| |\/\*|\*\/|')/.test(name)) {
    throw new PreparedStatementError("SQL injection warning for param '" + name + "'", 'EINJECT');
  }
  if (arguments.length < 2) {
    throw new PreparedStatementError("Invalid number of arguments. 2 arguments expected.", 'EARGS');
  }
  if (type instanceof Function) {
    type = type();
  }
  this.parameters[name] = {
    name: name,
    type: type.type,
    io: 1,
    length: type.length,
    scale: type.scale,
    precision: type.precision,
    tvpType: type.tvpType
  };
  return this;
}
```
- example usage
```shell
...
	}).catch(function(err) {
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
...
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.next"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>next ()](#apidoc.element.mssql.PreparedStatement.prototype.next)
- description and source-code
```javascript
next = function () {
  if (this._queue.length) {
    process.nextTick((function(_this) {
      return function() {
        return _this._queue.shift()(null, _this._pooledConnection);
      };
    })(this));
  } else {
    this._working = false;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.output"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>output (name, type)](#apidoc.element.mssql.PreparedStatement.prototype.output)
- description and source-code
```javascript
output = function (name, type) {
  if (/(--| |\/\*|\*\/|')/.test(name)) {
    throw new PreparedStatementError("SQL injection warning for param '" + name + "'", 'EINJECT');
  }
  if (arguments.length < 2) {
    throw new PreparedStatementError("Invalid number of arguments. 2 arguments expected.", 'EARGS');
  }
  if (type instanceof Function) {
    type = type();
  }
  this.parameters[name] = {
    name: name,
    type: type.type,
    io: 2,
    length: type.length,
    scale: type.scale,
    precision: type.precision
  };
  return this;
}
```
- example usage
```shell
...
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.prepare"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>prepare (statement, callback)](#apidoc.element.mssql.PreparedStatement.prototype.prepare)
- description and source-code
```javascript
prepare = function (statement, callback) {
  if (callback != null) {
    return this._prepare(statement, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._prepare(statement, function(err) {
        if (err) {
          return reject(err);
        }
        return resolve(_this);
      });
    };
  })(this));
}
```
- example usage
```shell
...
If you omit the connection argument, the global connection is used instead.

__Example__

'''javascript
var ps = new sql.PreparedStatement(/* [connection] */);
ps.input('param', sql.Int);
ps.prepare('select @param as value', function(err) {
    // ... error checks

    ps.execute({param: 12345}, function(err, recordset) {
// ... error checks

ps.unprepare(function(err) {
    // ... error checks
...
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.queue"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>queue (callback)](#apidoc.element.mssql.PreparedStatement.prototype.queue)
- description and source-code
```javascript
queue = function (callback) {
  if (!this._pooledConnection) {
    callback(new PreparedStatementError("Statement is not prepared. Call prepare() first.", 'ENOTPREPARED'));
    return this;
  }
  if (this._working) {
    this._queue.push(callback);
  } else {
    this._working = true;
    callback(null, this._pooledConnection);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement.prototype.unprepare"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatement.prototype.</span>unprepare (callback)](#apidoc.element.mssql.PreparedStatement.prototype.unprepare)
- description and source-code
```javascript
unprepare = function (callback) {
  if (callback != null) {
    return this._unprepare(callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._unprepare(function(err) {
        if (err) {
          return reject(err);
        }
        return resolve();
      });
    };
  })(this));
}
```
- example usage
```shell
...
ps.input('param', sql.Int);
ps.prepare('select @param as value', function(err) {
    // ... error checks

    ps.execute({param: 12345}, function(err, recordset) {
        // ... error checks

        ps.unprepare(function(err) {
            // ... error checks

        });
    });
});
'''
...
```



# <a name="apidoc.module.mssql.PreparedStatementError"></a>[module mssql.PreparedStatementError](#apidoc.module.mssql.PreparedStatementError)

#### <a name="apidoc.element.mssql.PreparedStatementError.PreparedStatementError"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError.PreparedStatementError)
- description and source-code
```javascript
function PreparedStatementError(message, code) {
  var err;
  if (!(this instanceof PreparedStatementError)) {
    if (message instanceof Error) {
      err = new PreparedStatementError(message.message, message.code);
      err.originalError = message;
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new PreparedStatementError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  this.code = code;
  PreparedStatementError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatementError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatementError.</span>captureStackTrace ()](#apidoc.element.mssql.PreparedStatementError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.PreparedStatementError.prototype"></a>[module mssql.PreparedStatementError.prototype](#apidoc.module.mssql.PreparedStatementError.prototype)

#### <a name="apidoc.element.mssql.PreparedStatementError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.PreparedStatementError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.PreparedStatementError.prototype.constructor)
- description and source-code
```javascript
function PreparedStatementError(message, code) {
  var err;
  if (!(this instanceof PreparedStatementError)) {
    if (message instanceof Error) {
      err = new PreparedStatementError(message.message, message.code);
      err.originalError = message;
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new PreparedStatementError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  this.code = code;
  PreparedStatementError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Real"></a>[module mssql.Real](#apidoc.module.mssql.Real)

#### <a name="apidoc.element.mssql.Real.Real"></a>[function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real.Real)
- description and source-code
```javascript
Real = function () {
  return {
    type: TYPES.Real
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Real.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Real.</span>inspect ()](#apidoc.element.mssql.Real.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Request"></a>[module mssql.Request](#apidoc.module.mssql.Request)

#### <a name="apidoc.element.mssql.Request.Request"></a>[function <span class="apidocSignatureSpan">mssql.</span>Request (connection)](#apidoc.element.mssql.Request.Request)
- description and source-code
```javascript
function Request(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof PreparedStatement) {
    this.pstatement = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this.parameters = {};
}
```
- example usage
```shell
...

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
// Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});

// Stored Procedure
...
```

#### <a name="apidoc.element.mssql.Request.EventEmitter"></a>[function <span class="apidocSignatureSpan">mssql.Request.</span>EventEmitter ()](#apidoc.element.mssql.Request.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.init"></a>[function <span class="apidocSignatureSpan">mssql.Request.</span>init ()](#apidoc.element.mssql.Request.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.listenerCount"></a>[function <span class="apidocSignatureSpan">mssql.Request.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Request.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Request.prototype"></a>[module mssql.Request.prototype](#apidoc.module.mssql.Request.prototype)

#### <a name="apidoc.element.mssql.Request.prototype._acquire"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_acquire (callback)](#apidoc.element.mssql.Request.prototype._acquire)
- description and source-code
```javascript
_acquire = function (callback) {
  if (this.transaction) {
    return this.transaction.queue(callback);
  } else if (this.pstatement) {
    return this.pstatement.queue(callback);
  } else {
    if (!this.connection.pool) {
      return callback(new ConnectionError("Connection not yet open.", 'ENOTOPEN'));
    }
    return this.connection.pool.acquire(callback);
  }
}
```
- example usage
```shell
...
      "class": msg["class"],
      lineNumber: msg.lineNumber,
      serverName: msg.serverName,
      procName: msg.procName
    });
  };
})(this);
return this._acquire((function(_this) {
  return function(err, connection) {
    var bulk, col, done, i, j, len, len1, objectid, ref1, ref2, req, row;
    if (!err) {
      if (_this.verbose) {
        _this._log("-------- sql bulk load --------\n    table: " + table.name);
      }
      if (_this.canceled) {
...
```

#### <a name="apidoc.element.mssql.Request.prototype._batch"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_batch (batch, callback)](#apidoc.element.mssql.Request.prototype._batch)
- description and source-code
```javascript
_batch = function (batch, callback) {
  if (!this.connection) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new RequestError("No connection is specified for that request.", 'ENOCONN');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  if (!this.connection.connected) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new ConnectionError("Connection is closed.", 'ECONNCLOSED');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  this.canceled = false;
  this.connection.driver.Request.prototype.batch.call(this, batch, (function(_this) {
    return function(err, recordsets) {
      if (_this.stream) {
        if (err) {
          _this.emit('error', err);
        }
        return _this.emit('done', _this.rowsAffected);
      } else {
        return callback(err, recordsets, _this.rowsAffected);
      }
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype._bulk"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_bulk (table, callback)](#apidoc.element.mssql.Request.prototype._bulk)
- description and source-code
```javascript
_bulk = function (table, callback) {
  if (!this.connection) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new RequestError("No connection is specified for that request.", 'ENOCONN');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  if (!this.connection.connected) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new ConnectionError("Connection is closed.", 'ECONNCLOSED');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  this.canceled = false;
  this.connection.driver.Request.prototype.bulk.call(this, table, (function(_this) {
    return function(err, rowCount) {
      if (_this.stream) {
        if (err) {
          _this.emit('error', err);
        }
        return _this.emit('done');
      } else {
        return callback(err, rowCount);
      }
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype._dedicated"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_dedicated (connection)](#apidoc.element.mssql.Request.prototype._dedicated)
- description and source-code
```javascript
_dedicated = function (connection) {
  this._acquire = function(callback) {
    return callback(null, connection);
  };
  this._release = function() {};
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype._execute"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_execute (procedure, callback)](#apidoc.element.mssql.Request.prototype._execute)
- description and source-code
```javascript
_execute = function (procedure, callback) {
  if (!this.connection) {
    return process.nextTick(function() {
      var e;
      e = new RequestError("No connection is specified for that request.", 'ENOCONN');
      if (this.stream) {
        this.emit('error', e);
        return this.emit('done');
      } else {
        return callback(e);
      }
    });
  }
  if (!this.connection.connected) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new ConnectionError("Connection is closed.", 'ECONNCLOSED');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  this.canceled = false;
  this.connection.driver.Request.prototype.execute.call(this, procedure, (function(_this) {
    return function(err, recordsets, returnValue) {
      if (_this.stream) {
        if (err) {
          _this.emit('error', err);
        }
        return _this.emit('done', returnValue, _this.rowsAffected);
      } else {
        return callback(err, recordsets, returnValue, _this.rowsAffected);
      }
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype._log"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_log (out)](#apidoc.element.mssql.Request.prototype._log)
- description and source-code
```javascript
_log = function (out) {
  if (typeof this.logger === "function") {
    return this.logger(out);
  } else {
    return console.log(out);
  }
}
```
- example usage
```shell
...
  };
})(this);
return this._acquire((function(_this) {
  return function(err, connection) {
    var bulk, col, done, i, j, len, len1, objectid, ref1, ref2, req, row;
    if (!err) {
      if (_this.verbose) {
        _this._log("-------- sql bulk load --------\n    table: " + table.name);
      }
      if (_this.canceled) {
        if (_this.verbose) {
          _this._log("---------- canceling ----------");
        }
        _this._release(connection);
        return typeof callback === "function" ? callback(new RequestError("Canceled.", 'ECANCEL')) : void 0;
...
```

#### <a name="apidoc.element.mssql.Request.prototype._query"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_query (command, callback)](#apidoc.element.mssql.Request.prototype._query)
- description and source-code
```javascript
_query = function (command, callback) {
  if (!this.connection) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new RequestError("No connection is specified for that request.", 'ENOCONN');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  if (!this.connection.connected) {
    return process.nextTick((function(_this) {
      return function() {
        var e;
        e = new ConnectionError("Connection is closed.", 'ECONNCLOSED');
        if (_this.stream) {
          _this.emit('error', e);
          return _this.emit('done');
        } else {
          return callback(e);
        }
      };
    })(this));
  }
  this.canceled = false;
  this.connection.driver.Request.prototype.query.call(this, command, (function(_this) {
    return function(err, recordsets) {
      if (_this.stream) {
        if (err) {
          _this.emit('error', err);
        }
        return _this.emit('done', _this.rowsAffected);
      } else {
        return callback(err, recordsets, _this.rowsAffected);
      }
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype._release"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_release (connection)](#apidoc.element.mssql.Request.prototype._release)
- description and source-code
```javascript
_release = function (connection) {
  if (this.transaction) {
    return this.transaction.next();
  } else if (this.pstatement) {
    return this.pstatement.next();
  } else {
    return this.connection.pool.release(connection);
  }
}
```
- example usage
```shell
...
} else {
  if (doReturn && !hasReturned) {
    if (connection != null) {
      for (event in errorHandlers) {
        handler = errorHandlers[event];
        connection.removeListener(event, handler);
      }
      _this._release(connection);
    }
    hasReturned = true;
    if (typeof callback === "function") {
      callback(e);
    }
  }
}
...
```

#### <a name="apidoc.element.mssql.Request.prototype._template"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>_template (method, strings, values)](#apidoc.element.mssql.Request.prototype._template)
- description and source-code
```javascript
_template = function (method, strings, values) {
  var command, i, index, len, value;
  command = [strings[0]];
  for (index = i = 0, len = values.length; i < len; index = ++i) {
    value = values[index];
    this.input("param" + (index + 1), value);
    command.push("@param" + (index + 1), strings[index + 1]);
  }
  return this[method](command.join(''));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype.batch"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>batch (batch, callback)](#apidoc.element.mssql.Request.prototype.batch)
- description and source-code
```javascript
batch = function (batch, callback) {
  var ref1;
  if (this.stream == null) {
    this.stream = (ref1 = this.connection) != null ? ref1.config.stream : void 0;
  }
  this.rowsAffected = 0;
  if (this.stream || (callback != null)) {
    return this._batch(batch, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._batch(batch, function(err, recordset) {
        if (err) {
          return reject(err);
        }
        return resolve(recordset);
      });
    };
  })(this));
}
```
- example usage
```shell
...
- **batch** - T-SQL command to be executed.
- **callback(err, recordset)** - A callback which is called after execution has completed, or an error has occurred. Optional. If
 omitted, returns [Promise](#promises).

__Example__

'''javascript
var request = new sql.Request();
request.batch('create procedure #temporary as select * from table', function(err, recordset) {
    // ... error checks
});
'''

__Errors__
- ETIMEOUT ('RequestError') - Request timeout.
- EREQUEST ('RequestError') - *Message from SQL Server*
...
```

#### <a name="apidoc.element.mssql.Request.prototype.bulk"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>bulk (table, callback)](#apidoc.element.mssql.Request.prototype.bulk)
- description and source-code
```javascript
bulk = function (table, callback) {
  var ref1;
  if (this.stream == null) {
    this.stream = (ref1 = this.connection) != null ? ref1.config.stream : void 0;
  }
  if (this.stream || (callback != null)) {
    return this._bulk(table, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._bulk(table, function(err, rowCount) {
        if (err) {
          return reject(err);
        }
        return resolve(rowCount);
      });
    };
  })(this));
}
```
- example usage
```shell
...
var table = new sql.Table('table_name'); // or temporary table, e.g. #temptable
table.create = true;
table.columns.add('a', sql.Int, {nullable: true, primary: true});
table.columns.add('b', sql.VarChar(50), {nullable: false});
table.rows.add(777, 'test');

var request = new sql.Request();
request.bulk(table, function(err, rowCount) {
    // ... error checks
});
'''

**IMPORTANT**: Always indicate whether the column is nullable or not!

**TIP**: If you set 'table.create' to 'true', module will check if the table exists before it start sending data. If it doesn't,
it will automatically create it. You can specify primary key columns by setting 'primary: true' to column's options. Primary key
 constraint on multiple columns is supported.
...
```

#### <a name="apidoc.element.mssql.Request.prototype.cancel"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>cancel ()](#apidoc.element.mssql.Request.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  this.canceled = true;
  this.connection.driver.Request.prototype.cancel.call(this);
  return this;
}
```
- example usage
```shell
...
    console.log(err instanceof sql.RequestError);  // true
    console.log(err.message);                      // Cancelled.
    console.log(err.code);                         // ECANCEL

    // ...
});

request.cancel();
'''

## Transaction

**IMPORTANT:** always use 'Transaction' class to create transactions - it ensures that all your requests are executed on one connection
. Once you call 'begin', a single connection is acquired from the connection pool and all subsequent requests (initialized with
the 'Transaction' object) are executed exclusively on this connection. Transaction also contains a queue to make sure your requests
 are executed in series. After you call 'commit' or 'rollback', connection is then released back to the connection pool.

'''javascript
...
```

#### <a name="apidoc.element.mssql.Request.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>constructor (connection)](#apidoc.element.mssql.Request.prototype.constructor)
- description and source-code
```javascript
function Request(connection) {
  if (connection instanceof Transaction) {
    this.transaction = connection;
    this.connection = connection.connection;
  } else if (connection instanceof PreparedStatement) {
    this.pstatement = connection;
    this.connection = connection.connection;
  } else if (connection instanceof Connection) {
    this.connection = connection;
  } else {
    this.connection = global_connection;
  }
  this.parameters = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request.prototype.execute"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>execute (command, callback)](#apidoc.element.mssql.Request.prototype.execute)
- description and source-code
```javascript
execute = function (command, callback) {
  var ref1;
  if (this.stream == null) {
    this.stream = (ref1 = this.connection) != null ? ref1.config.stream : void 0;
  }
  this.rowsAffected = 0;
  if (this.stream || (callback != null)) {
    return this._execute(command, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._execute(command, function(err, recordset) {
        if (err) {
          return reject(err);
        }
        return resolve(recordset);
      });
    };
  })(this));
}
```
- example usage
```shell
...
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.Request.prototype.input"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>input (name, type, value)](#apidoc.element.mssql.Request.prototype.input)
- description and source-code
```javascript
input = function (name, type, value) {
  if (/(--| |\/\*|\*\/|')/.test(name)) {
    throw new RequestError("SQL injection warning for param '" + name + "'", 'EINJECT');
  }
  if (arguments.length === 1) {
    throw new RequestError("Invalid number of arguments. At least 2 arguments expected.", 'EARGS');
  } else if (arguments.length === 2) {
    value = type;
    type = getTypeByValue(value);
  }
  if ((value != null ? value.valueOf : void 0) && !(value instanceof Date)) {
    value = value.valueOf();
  }
  if (value === void 0) {
    value = null;
  }
  if (value !== value) {
    value = null;
  }
  if (type instanceof Function) {
    type = type();
  }
  this.parameters[name] = {
    name: name,
    type: type.type,
    io: 1,
    value: value,
    length: type.length,
    scale: type.scale,
    precision: type.precision,
    tvpType: type.tvpType
  };
  return this;
}
```
- example usage
```shell
...
	}).catch(function(err) {
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
...
```

#### <a name="apidoc.element.mssql.Request.prototype.output"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>output (name, type, value)](#apidoc.element.mssql.Request.prototype.output)
- description and source-code
```javascript
output = function (name, type, value) {
  if (!type) {
    type = TYPES.NVarChar;
  }
  if (/(--| |\/\*|\*\/|')/.test(name)) {
    throw new RequestError("SQL injection warning for param '" + name + "'", 'EINJECT');
  }
  if (type === TYPES.Text || type === TYPES.NText || type === TYPES.Image) {
    throw new RequestError("Deprecated types (Text, NText, Image) are not supported as OUTPUT parameters.", 'EDEPRECATED');
  }
  if ((value != null ? value.valueOf : void 0) && !(value instanceof Date)) {
    value = value.valueOf();
  }
  if (value === void 0) {
    value = null;
  }
  if (value !== value) {
    value = null;
  }
  if (type instanceof Function) {
    type = type();
  }
  this.parameters[name] = {
    name: name,
    type: type.type,
    io: 2,
    value: value,
    length: type.length,
    scale: type.scale,
    precision: type.precision
  };
  return this;
}
```
- example usage
```shell
...
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.Request.prototype.pipe"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>pipe (stream)](#apidoc.element.mssql.Request.prototype.pipe)
- description and source-code
```javascript
pipe = function (stream) {
  this.stream = true;
  this.on('row', stream.write.bind(stream));
  this.on('error', stream.emit.bind(stream, 'error'));
  this.on('done', function() {
    return setImmediate(function() {
      return stream.end();
    });
  });
  stream.emit('pipe', this);
  return stream;
}
```
- example usage
```shell
...

- **stream** - Writable stream in object mode.

__Example__

'''javascript
var request = new sql.Request();
request.pipe(stream);
request.query('select * from mytable');
stream.on('error', function(err) {
    // ...
});
stream.on('finish', function() {
    // ...
});
...
```

#### <a name="apidoc.element.mssql.Request.prototype.query"></a>[function <span class="apidocSignatureSpan">mssql.Request.prototype.</span>query (command, callback)](#apidoc.element.mssql.Request.prototype.query)
- description and source-code
```javascript
query = function (command, callback) {
  var ref1;
  if (this.stream == null) {
    this.stream = (ref1 = this.connection) != null ? ref1.config.stream : void 0;
  }
  this.rowsAffected = 0;
  if (this.stream || (callback != null)) {
    return this._query(command, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._query(command, function(err, recordsets) {
        if (err) {
          return reject(err);
        }
        return resolve(recordsets);
      });
    };
  })(this));
}
```
- example usage
```shell
...

'''javascript
var sql = require('mssql');

sql.connect("mssql://username:password@localhost/database").then(function() {
// Query

	new sql.Request().query('select * from mytable').then(function(recordset) {
		console.dir(recordset);
	}).catch(function(err) {
		// ... query error checks
	});

// Stored Procedure
...
```



# <a name="apidoc.module.mssql.RequestError"></a>[module mssql.RequestError](#apidoc.module.mssql.RequestError)

#### <a name="apidoc.element.mssql.RequestError.RequestError"></a>[function <span class="apidocSignatureSpan">mssql.</span>RequestError (message, code)](#apidoc.element.mssql.RequestError.RequestError)
- description and source-code
```javascript
function RequestError(message, code) {
  var err, ref1, ref10, ref11, ref2, ref3, ref4, ref5, ref6, ref7, ref8, ref9;
  if (!(this instanceof RequestError)) {
    if (message instanceof Error) {
      err = new RequestError(message.message, (ref1 = message.code) != null ? ref1 : code);
      err.number = (ref2 = (ref3 = message.info) != null ? ref3.number : void 0) != null ? ref2 : message.code;
      err.lineNumber = (ref4 = message.info) != null ? ref4.lineNumber : void 0;
      err.state = (ref5 = (ref6 = message.info) != null ? ref6.state : void 0) != null ? ref5 : message.sqlstate;
      err["class"] = (ref7 = (ref8 = message.info) != null ? ref8["class"] : void 0) != null ? ref7 : (ref9 = message.info) != null
 ? ref9.severity : void 0;
      err.serverName = (ref10 = message.info) != null ? ref10.serverName : void 0;
      err.procName = (ref11 = message.info) != null ? ref11.procName : void 0;
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new RequestError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  RequestError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.RequestError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">mssql.RequestError.</span>captureStackTrace ()](#apidoc.element.mssql.RequestError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.RequestError.prototype"></a>[module mssql.RequestError.prototype](#apidoc.module.mssql.RequestError.prototype)

#### <a name="apidoc.element.mssql.RequestError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.RequestError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.RequestError.prototype.constructor)
- description and source-code
```javascript
function RequestError(message, code) {
  var err, ref1, ref10, ref11, ref2, ref3, ref4, ref5, ref6, ref7, ref8, ref9;
  if (!(this instanceof RequestError)) {
    if (message instanceof Error) {
      err = new RequestError(message.message, (ref1 = message.code) != null ? ref1 : code);
      err.number = (ref2 = (ref3 = message.info) != null ? ref3.number : void 0) != null ? ref2 : message.code;
      err.lineNumber = (ref4 = message.info) != null ? ref4.lineNumber : void 0;
      err.state = (ref5 = (ref6 = message.info) != null ? ref6.state : void 0) != null ? ref5 : message.sqlstate;
      err["class"] = (ref7 = (ref8 = message.info) != null ? ref8["class"] : void 0) != null ? ref7 : (ref9 = message.info) != null
 ? ref9.severity : void 0;
      err.serverName = (ref10 = message.info) != null ? ref10.serverName : void 0;
      err.procName = (ref11 = message.info) != null ? ref11.procName : void 0;
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new RequestError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  RequestError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.SmallDateTime"></a>[module mssql.SmallDateTime](#apidoc.module.mssql.SmallDateTime)

#### <a name="apidoc.element.mssql.SmallDateTime.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime.SmallDateTime)
- description and source-code
```javascript
SmallDateTime = function () {
  return {
    type: TYPES.SmallDateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallDateTime.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallDateTime.</span>inspect ()](#apidoc.element.mssql.SmallDateTime.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.SmallInt"></a>[module mssql.SmallInt](#apidoc.module.mssql.SmallInt)

#### <a name="apidoc.element.mssql.SmallInt.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt.SmallInt)
- description and source-code
```javascript
SmallInt = function () {
  return {
    type: TYPES.SmallInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallInt.</span>inspect ()](#apidoc.element.mssql.SmallInt.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.SmallMoney"></a>[module mssql.SmallMoney](#apidoc.module.mssql.SmallMoney)

#### <a name="apidoc.element.mssql.SmallMoney.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney.SmallMoney)
- description and source-code
```javascript
SmallMoney = function () {
  return {
    type: TYPES.SmallMoney
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallMoney.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallMoney.</span>inspect ()](#apidoc.element.mssql.SmallMoney.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.TVP"></a>[module mssql.TVP](#apidoc.module.mssql.TVP)

#### <a name="apidoc.element.mssql.TVP.TVP"></a>[function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP.TVP)
- description and source-code
```javascript
TVP = function (tvpType) {
  return {
    type: TYPES.TVP,
    tvpType: tvpType
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TVP.inspect"></a>[function <span class="apidocSignatureSpan">mssql.TVP.</span>inspect ()](#apidoc.element.mssql.TVP.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.TYPES"></a>[module mssql.TYPES](#apidoc.module.mssql.TYPES)

#### <a name="apidoc.element.mssql.TYPES.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>BigInt ()](#apidoc.element.mssql.TYPES.BigInt)
- description and source-code
```javascript
BigInt = function () {
  return {
    type: TYPES.BigInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Binary"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Binary (length)](#apidoc.element.mssql.TYPES.Binary)
- description and source-code
```javascript
Binary = function (length) {
  return {
    type: TYPES.Binary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Bit"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Bit ()](#apidoc.element.mssql.TYPES.Bit)
- description and source-code
```javascript
Bit = function () {
  return {
    type: TYPES.Bit
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Char"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Char (length)](#apidoc.element.mssql.TYPES.Char)
- description and source-code
```javascript
Char = function (length) {
  return {
    type: TYPES.Char,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Date"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Date ()](#apidoc.element.mssql.TYPES.Date)
- description and source-code
```javascript
Date = function () {
  return {
    type: TYPES.Date
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime ()](#apidoc.element.mssql.TYPES.DateTime)
- description and source-code
```javascript
DateTime = function () {
  return {
    type: TYPES.DateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime2 (scale)](#apidoc.element.mssql.TYPES.DateTime2)
- description and source-code
```javascript
DateTime2 = function (scale) {
  return {
    type: TYPES.DateTime2,
    scale: scale
  };
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:

'''
sql.Bit
sql.BigInt
...
```

#### <a name="apidoc.element.mssql.TYPES.DateTimeOffset"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTimeOffset (scale)](#apidoc.element.mssql.TYPES.DateTimeOffset)
- description and source-code
```javascript
DateTimeOffset = function (scale) {
  return {
    type: TYPES.DateTimeOffset,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Decimal (precision, scale)](#apidoc.element.mssql.TYPES.Decimal)
- description and source-code
```javascript
Decimal = function (precision, scale) {
  return {
    type: TYPES.Decimal,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc");               // varchar(3)
request.input("name", sql.VarChar(50), "abc");           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc");      // varchar(MAX)
request.output("name", sql.VarChar);                     // varchar(8000)
request.output("name", sql.VarChar, "abc");              // varchar(3)

request.input("name", sql.Decimal, 155.33);              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33);          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33);       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date());        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date());     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.TYPES.Float"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Float ()](#apidoc.element.mssql.TYPES.Float)
- description and source-code
```javascript
Float = function () {
  return {
    type: TYPES.Float
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Geography"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geography ()](#apidoc.element.mssql.TYPES.Geography)
- description and source-code
```javascript
Geography = function () {
  return {
    type: TYPES.Geography
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geometry ()](#apidoc.element.mssql.TYPES.Geometry)
- description and source-code
```javascript
Geometry = function () {
  return {
    type: TYPES.Geometry
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Image"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Image ()](#apidoc.element.mssql.TYPES.Image)
- description and source-code
```javascript
Image = function () {
  return {
    type: TYPES.Image
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Int"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Int ()](#apidoc.element.mssql.TYPES.Int)
- description and source-code
```javascript
Int = function () {
  return {
    type: TYPES.Int
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Money"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Money ()](#apidoc.element.mssql.TYPES.Money)
- description and source-code
```javascript
Money = function () {
  return {
    type: TYPES.Money
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NChar (length)](#apidoc.element.mssql.TYPES.NChar)
- description and source-code
```javascript
NChar = function (length) {
  return {
    type: TYPES.NChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NText"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NText ()](#apidoc.element.mssql.TYPES.NText)
- description and source-code
```javascript
NText = function () {
  return {
    type: TYPES.NText
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NVarChar (length)](#apidoc.element.mssql.TYPES.NVarChar)
- description and source-code
```javascript
NVarChar = function (length) {
  return {
    type: TYPES.NVarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Numeric (precision, scale)](#apidoc.element.mssql.TYPES.Numeric)
- description and source-code
```javascript
Numeric = function (precision, scale) {
  return {
    type: TYPES.Numeric,
    precision: precision,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Real"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Real ()](#apidoc.element.mssql.TYPES.Real)
- description and source-code
```javascript
Real = function () {
  return {
    type: TYPES.Real
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallDateTime ()](#apidoc.element.mssql.TYPES.SmallDateTime)
- description and source-code
```javascript
SmallDateTime = function () {
  return {
    type: TYPES.SmallDateTime
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallInt ()](#apidoc.element.mssql.TYPES.SmallInt)
- description and source-code
```javascript
SmallInt = function () {
  return {
    type: TYPES.SmallInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallMoney ()](#apidoc.element.mssql.TYPES.SmallMoney)
- description and source-code
```javascript
SmallMoney = function () {
  return {
    type: TYPES.SmallMoney
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.TVP"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>TVP (tvpType)](#apidoc.element.mssql.TYPES.TVP)
- description and source-code
```javascript
TVP = function (tvpType) {
  return {
    type: TYPES.TVP,
    tvpType: tvpType
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Text"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Text ()](#apidoc.element.mssql.TYPES.Text)
- description and source-code
```javascript
Text = function () {
  return {
    type: TYPES.Text
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Time"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Time (scale)](#apidoc.element.mssql.TYPES.Time)
- description and source-code
```javascript
Time = function (scale) {
  return {
    type: TYPES.Time,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>TinyInt ()](#apidoc.element.mssql.TYPES.TinyInt)
- description and source-code
```javascript
TinyInt = function () {
  return {
    type: TYPES.TinyInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.UDT"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>UDT ()](#apidoc.element.mssql.TYPES.UDT)
- description and source-code
```javascript
UDT = function () {
  return {
    type: TYPES.UDT
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>UniqueIdentifier ()](#apidoc.element.mssql.TYPES.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier = function () {
  return {
    type: TYPES.UniqueIdentifier
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarBinary (length)](#apidoc.element.mssql.TYPES.VarBinary)
- description and source-code
```javascript
VarBinary = function (length) {
  return {
    type: TYPES.VarBinary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarChar (length)](#apidoc.element.mssql.TYPES.VarChar)
- description and source-code
```javascript
VarChar = function (length) {
  return {
    type: TYPES.VarChar,
    length: length
  };
}
```
- example usage
```shell
...
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.TYPES.Variant"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Variant ()](#apidoc.element.mssql.TYPES.Variant)
- description and source-code
```javascript
Variant = function () {
  return {
    type: TYPES.Variant
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Xml"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Xml ()](#apidoc.element.mssql.TYPES.Xml)
- description and source-code
```javascript
Xml = function () {
  return {
    type: TYPES.Xml
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Table"></a>[module mssql.Table](#apidoc.module.mssql.Table)

#### <a name="apidoc.element.mssql.Table.Table"></a>[function <span class="apidocSignatureSpan">mssql.</span>Table (name)](#apidoc.element.mssql.Table.Table)
- description and source-code
```javascript
function Table(name) {
  var ref1;
  if (name) {
    ref1 = Table.parseName(name), this.name = ref1.name, this.schema = ref1.schema, this.database = ref1.database;
    this.path = "" + (this.database ? "[" + this.database + "]." : "") + (this.schema ? "[" + this.schema + "]." : "") + "[" + this
.name + "]";
    this.temporary = this.name.charAt(0) === '#';
  }
  this.columns = [];
  this.rows = [];
  Object.defineProperty(this.columns, "add", {
    value: function(name, column, options) {
      if (options == null) {
        options = {};
      }
      if (column == null) {
        throw new Error("Column data type is not defined.");
      }
      if (column instanceof Function) {
        column = column();
      }
      column.name = name;
      column.nullable = options.nullable;
      column.primary = options.primary;
      return this.push(column);
    }
  });
  Object.defineProperty(this.rows, "add", {
    value: function() {
      var values;
      values = 1 <= arguments.length ? slice.call(arguments, 0) : [];
      return this.push(values);
    }
  });
}
```
- example usage
```shell
...

- **table** - 'sql.Table' instance.
- **callback(err, rowCount)** - A callback which is called after bulk insert has completed, or an error has occurred. Optional.
If omitted, returns [Promise](#promises).

__Example__

'''javascript
var table = new sql.Table('table_name'); // or temporary table, e.g. #temptable
table.create = true;
table.columns.add('a', sql.Int, {nullable: true, primary: true});
table.columns.add('b', sql.VarChar(50), {nullable: false});
table.rows.add(777, 'test');

var request = new sql.Request();
request.bulk(table, function(err, rowCount) {
...
```

#### <a name="apidoc.element.mssql.Table.fromRecordset"></a>[function <span class="apidocSignatureSpan">mssql.Table.</span>fromRecordset (recordset, name)](#apidoc.element.mssql.Table.fromRecordset)
- description and source-code
```javascript
fromRecordset = function (recordset, name) {
  var col, i, j, len, len1, ref1, ref2, row, t;
  t = new this(name);
  ref1 = recordset.columns;
  for (name in ref1) {
    col = ref1[name];
    t.columns.add(name, {
      type: col.type,
      length: col.length,
      scale: col.scale,
      precision: col.precision
    }, {
      nullable: col.nullable
    });
  }
  if (t.columns.length === 1 && t.columns[0].name === JSON_COLUMN_ID) {
    for (i = 0, len = recordset.length; i < len; i++) {
      row = recordset[i];
      t.rows.add(JSON.stringify(row));
    }
  } else {
    for (j = 0, len1 = recordset.length; j < len1; j++) {
      row = recordset[j];
      (ref2 = t.rows).add.apply(ref2, (function() {
        var k, len2, ref2, results;
        ref2 = t.columns;
        results = [];
        for (k = 0, len2 = ref2.length; k < len2; k++) {
          col = ref2[k];
          results.push(row[col.name]);
        }
        return results;
      })());
    }
  }
  return t;
}
```
- example usage
```shell
...
    Object.defineProperty(recordset, 'columns', {
      enumerable: false,
      value: columns
    });
    Object.defineProperty(recordset, 'toTable', {
      enumerable: false,
      value: function() {
        return Table.fromRecordset(this);
      }
    });
    recordsets.push(recordset);
  }
  recordset = [];
  return columns = {};
};
...
```

#### <a name="apidoc.element.mssql.Table.parseName"></a>[function <span class="apidocSignatureSpan">mssql.Table.</span>parseName (name)](#apidoc.element.mssql.Table.parseName)
- description and source-code
```javascript
parseName = function (name) {
  var buffer, char, cursor, escaped, length, path;
  length = name.length;
  cursor = -1;
  buffer = '';
  escaped = false;
  path = [];
  while (++cursor < length) {
    char = name.charAt(cursor);
    if (char === '[') {
      if (escaped) {
        buffer += char;
      } else {
        escaped = true;
      }
    } else if (char === ']') {
      if (escaped) {
        escaped = false;
      } else {
        throw new Error("Invalid table name.");
      }
    } else if (char === '.') {
      if (escaped) {
        buffer += char;
      } else {
        path.push(buffer);
        buffer = '';
      }
    } else {
      buffer += char;
    }
  }
  if (buffer) {
    path.push(buffer);
  }
  switch (path.length) {
    case 1:
      return {
        name: path[0],
        schema: null,
        database: null
      };
    case 2:
      return {
        name: path[1],
        schema: path[0],
        database: null
      };
    case 3:
      return {
        name: path[2],
        schema: path[1],
        database: path[0]
      };
    default:
      throw new Error("Invalid table name.");
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Table.prototype"></a>[module mssql.Table.prototype](#apidoc.module.mssql.Table.prototype)

#### <a name="apidoc.element.mssql.Table.prototype._makeBulk"></a>[function <span class="apidocSignatureSpan">mssql.Table.prototype.</span>_makeBulk ()](#apidoc.element.mssql.Table.prototype._makeBulk)
- description and source-code
```javascript
_makeBulk = function () {
  var col, i, len, ref1;
  ref1 = this.columns;
  for (i = 0, len = ref1.length; i < len; i++) {
    col = ref1[i];
    switch (col.type) {
      case TYPES.Xml:
        col.type = TYPES.NVarChar(MAX).type;
        break;
      case TYPES.UDT:
      case TYPES.Geography:
      case TYPES.Geometry:
        col.type = TYPES.VarBinary(MAX).type;
    }
  }
  return this;
}
```
- example usage
```shell
...

/*
		Bulk load.
 */

TediousRequest.prototype.bulk = function(table, callback) {
  var errorHandlers, errors, handleError, handleInfo, hasReturned, started;
  table._makeBulk();
  if (!table.name) {
    process.nextTick(function() {
      return callback(RequestError("Table name must be specified for bulk insert.", "ENAME"));
    });
  }
  if (table.name.charAt(0) === '@') {
    process.nextTick(function() {
...
```

#### <a name="apidoc.element.mssql.Table.prototype.declare"></a>[function <span class="apidocSignatureSpan">mssql.Table.prototype.</span>declare ()](#apidoc.element.mssql.Table.prototype.declare)
- description and source-code
```javascript
declare = function () {
  var cols, pkey;
  pkey = this.columns.filter(function(col) {
    return col.primary === true;
  }).map(function(col) {
    return col.name;
  });
  cols = this.columns.map(function(col) {
    var def;
    def = ["[" + col.name + "] " + (declare(col.type, col))];
    if (col.nullable === true) {
      def.push("null");
    } else if (col.nullable === false) {
      def.push("not null");
    }
    if (col.primary === true && pkey.length === 1) {
      def.push("primary key");
    }
    return def.join(' ');
  });
  return "create table " + this.path + " (" + (cols.join(', ')) + (pkey.length > 1 ? ", constraint PK_" + (this.temporary ? this
.name.substr(1) : this.name) + " primary key (" + (pkey.join(', ')) + ")" : "") + ")";
}
```
- example usage
```shell
...
}
if (table.create) {
  if (table.temporary) {
    objectid = "tempdb..[" + table.name + "]";
  } else {
    objectid = table.path;
  }
  req = new tds.Request("if object_id('" + (objectid.replace(/'/g, '\'\'')) + "') is null " + (table.declare()), function(err) {
    if (err) {
      return done(err);
    }
    return connection.execBulkLoad(bulk);
  });
  return connection.execSqlBatch(req);
} else {
...
```



# <a name="apidoc.module.mssql.Text"></a>[module mssql.Text](#apidoc.module.mssql.Text)

#### <a name="apidoc.element.mssql.Text.Text"></a>[function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text.Text)
- description and source-code
```javascript
Text = function () {
  return {
    type: TYPES.Text
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Text.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Text.</span>inspect ()](#apidoc.element.mssql.Text.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Time"></a>[module mssql.Time](#apidoc.module.mssql.Time)

#### <a name="apidoc.element.mssql.Time.Time"></a>[function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time.Time)
- description and source-code
```javascript
Time = function (scale) {
  return {
    type: TYPES.Time,
    scale: scale
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Time.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Time.</span>inspect ()](#apidoc.element.mssql.Time.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.TinyInt"></a>[module mssql.TinyInt](#apidoc.module.mssql.TinyInt)

#### <a name="apidoc.element.mssql.TinyInt.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt.TinyInt)
- description and source-code
```javascript
TinyInt = function () {
  return {
    type: TYPES.TinyInt
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TinyInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.TinyInt.</span>inspect ()](#apidoc.element.mssql.TinyInt.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Transaction"></a>[module mssql.Transaction](#apidoc.module.mssql.Transaction)

#### <a name="apidoc.element.mssql.Transaction.Transaction"></a>[function <span class="apidocSignatureSpan">mssql.</span>Transaction (connection)](#apidoc.element.mssql.Transaction.Transaction)
- description and source-code
```javascript
function Transaction(connection) {
  this._abort = bind(this._abort, this);
  this.connection = connection != null ? connection : global_connection;
  this._queue = [];
}
```
- example usage
```shell
...
'''

## Transaction

**IMPORTANT:** always use 'Transaction' class to create transactions - it ensures that all your requests are executed on one connection
. Once you call 'begin', a single connection is acquired from the connection pool and all subsequent requests (initialized with
the 'Transaction' object) are executed exclusively on this connection. Transaction also contains a queue to make sure your requests
 are executed in series. After you call 'commit' or 'rollback', connection is then released back to the connection pool.

'''javascript
var transaction = new sql.Transaction(/* [connection] */);
'''

If you omit connection argument, global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.Transaction.EventEmitter"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.</span>EventEmitter ()](#apidoc.element.mssql.Transaction.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.init"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.</span>init ()](#apidoc.element.mssql.Transaction.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.listenerCount"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.</span>listenerCount (emitter, type)](#apidoc.element.mssql.Transaction.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Transaction.prototype"></a>[module mssql.Transaction.prototype](#apidoc.module.mssql.Transaction.prototype)

#### <a name="apidoc.element.mssql.Transaction.prototype._abort"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_abort ()](#apidoc.element.mssql.Transaction.prototype._abort)
- description and source-code
```javascript
_abort = function () {
  return this.connection.driver.Transaction.prototype._abort.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype._begin"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_begin (isolationLevel, callback)](#apidoc.element.mssql.Transaction.prototype._begin)
- description and source-code
```javascript
_begin = function (isolationLevel, callback) {
  if (isolationLevel != null) {
    this.isolationLevel = isolationLevel;
  }
  if (this._pooledConnection) {
    callback(new TransactionError("Transaction has already begun.", 'EALREADYBEGUN'));
    return this;
  }
  this.connection.driver.Transaction.prototype.begin.call(this, (function(_this) {
    return function(err) {
      if (!err) {
        _this.emit('begin');
      }
      return callback(err);
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype._commit"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_commit (callback)](#apidoc.element.mssql.Transaction.prototype._commit)
- description and source-code
```javascript
_commit = function (callback) {
  if (!this._pooledConnection) {
    callback(new TransactionError("Transaction has not begun. Call begin() first.", 'ENOTBEGUN'));
    return this;
  }
  if (this._working) {
    callback(new TransactionError("Can't commit transaction. There is a request in progress.", 'EREQINPROG'));
    return this;
  }
  if (this._queue.length) {
    callback(new TransactionError("Can't commit transaction. There are request in queue.", 'EREQINPROG'));
    return this;
  }
  this.connection.driver.Transaction.prototype.commit.call(this, (function(_this) {
    return function(err) {
      if (!err) {
        _this.emit('commit');
      }
      return callback(err);
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype._rollback"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>_rollback (callback)](#apidoc.element.mssql.Transaction.prototype._rollback)
- description and source-code
```javascript
_rollback = function (callback) {
  if (this._aborted) {
    callback(new TransactionError("Transaction has been aborted.", 'EABORT'));
    return this;
  }
  if (!this._pooledConnection) {
    callback(new TransactionError("Transaction has not begun. Call begin() first.", 'ENOTBEGUN'));
    return this;
  }
  if (this._working) {
    callback(new TransactionError("Can't rollback transaction. There is a request in progress.", 'EREQINPROG'));
    return this;
  }
  if (this._queue.length) {
    this._aborted = true;
  }
  this.connection.driver.Transaction.prototype.rollback.call(this, (function(_this) {
    return function(err) {
      if (!err) {
        _this.emit('rollback', _this._aborted);
      }
      return callback(err);
    };
  })(this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype.begin"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>begin (isolationLevel, callback)](#apidoc.element.mssql.Transaction.prototype.begin)
- description and source-code
```javascript
begin = function (isolationLevel, callback) {
  if (isolationLevel instanceof Function) {
    callback = isolationLevel;
    isolationLevel = void 0;
  }
  if (callback != null) {
    return this._begin(isolationLevel, callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._begin(isolationLevel, function(err) {
        if (err) {
          return reject(err);
        }
        return resolve(_this);
      });
    };
  })(this));
}
```
- example usage
```shell
...

If you omit connection argument, global connection is used instead.

__Example__

'''javascript
var transaction = new sql.Transaction(/* [connection] */);
transaction.begin(function(err) {
    // ... error checks

    var request = new sql.Request(transaction);
    request.query('insert into mytable (mycolumn) values (12345)', function(err, recordset) {
// ... error checks

transaction.commit(function(err, recordset) {
...
```

#### <a name="apidoc.element.mssql.Transaction.prototype.commit"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>commit (callback)](#apidoc.element.mssql.Transaction.prototype.commit)
- description and source-code
```javascript
commit = function (callback) {
  if (callback != null) {
    return this._commit(callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._commit(function(err) {
        if (err) {
          return reject(err);
        }
        return resolve();
      });
    };
  })(this));
}
```
- example usage
```shell
...
transaction.begin(function(err) {
    // ... error checks

    var request = new sql.Request(transaction);
    request.query('insert into mytable (mycolumn) values (12345)', function(err, recordset) {
        // ... error checks

        transaction.commit(function(err, recordset) {
            // ... error checks

            console.log("Transaction committed.");
        });
    });
});
'''
...
```

#### <a name="apidoc.element.mssql.Transaction.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>constructor (connection)](#apidoc.element.mssql.Transaction.prototype.constructor)
- description and source-code
```javascript
function Transaction(connection) {
  this._abort = bind(this._abort, this);
  this.connection = connection != null ? connection : global_connection;
  this._queue = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype.next"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>next ()](#apidoc.element.mssql.Transaction.prototype.next)
- description and source-code
```javascript
next = function () {
  var toAbort;
  if (this._aborted) {
    toAbort = this._queue;
    this._queue = [];
    process.nextTick((function(_this) {
      return function() {
        var results;
        results = [];
        while (toAbort.length) {
          results.push(toAbort.shift()(new TransactionError("Transaction aborted.", "EABORT")));
        }
        return results;
      };
    })(this));
  }
  this._working = false;
  if (this._queue.length) {
    process.nextTick((function(_this) {
      return function() {
        if (_this._aborted) {
          return _this.next();
        }
        _this._working = true;
        return _this._queue.shift()(null, _this._pooledConnection);
      };
    })(this));
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype.queue"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>queue (callback)](#apidoc.element.mssql.Transaction.prototype.queue)
- description and source-code
```javascript
queue = function (callback) {
  if (!this._pooledConnection) {
    callback(new TransactionError("Transaction has not begun. Call begin() first.", 'ENOTBEGUN'));
    return this;
  }
  if (this._working || this._queue.length) {
    this._queue.push(callback);
  } else {
    this._working = true;
    callback(null, this._pooledConnection);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction.prototype.request"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>request ()](#apidoc.element.mssql.Transaction.prototype.request)
- description and source-code
```javascript
request = function () {
  return new Request(this);
}
```
- example usage
```shell
...
}

var connection1 = new sql.Connection(config, function(err) {
    // ... error checks

    // Query

    var request = new sql.Request(connection1); // or: var request = connection1.request();
    request.query('select 1 as number', function(err, recordset) {
        // ... error checks

        console.dir(recordset);
    });

});
...
```

#### <a name="apidoc.element.mssql.Transaction.prototype.rollback"></a>[function <span class="apidocSignatureSpan">mssql.Transaction.prototype.</span>rollback (callback)](#apidoc.element.mssql.Transaction.prototype.rollback)
- description and source-code
```javascript
rollback = function (callback) {
  if (callback != null) {
    return this._rollback(callback);
  }
  return new module.exports.Promise((function(_this) {
    return function(resolve, reject) {
      return _this._rollback(function(err) {
        if (err) {
          return reject(err);
        }
        return resolve();
      });
    };
  })(this));
}
```
- example usage
```shell
...

    var request = new sql.Request(transaction);
    request.query('insert into mytable (bitcolumn) values (2)', function(err, recordset) {
        // insert should fail because of invalid value

		if (err) {
			if (!rolledBack) {
		        transaction.rollback(function(err) {
		            // ... error checks
		        });
		    }
		} else {
			transaction.commit(function(err) {
	            // ... error checks
	        });
...
```



# <a name="apidoc.module.mssql.TransactionError"></a>[module mssql.TransactionError](#apidoc.module.mssql.TransactionError)

#### <a name="apidoc.element.mssql.TransactionError.TransactionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>TransactionError (message, code)](#apidoc.element.mssql.TransactionError.TransactionError)
- description and source-code
```javascript
function TransactionError(message, code) {
  var err;
  if (!(this instanceof TransactionError)) {
    if (message instanceof Error) {
      err = new TransactionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new TransactionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  TransactionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TransactionError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">mssql.TransactionError.</span>captureStackTrace ()](#apidoc.element.mssql.TransactionError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.TransactionError.prototype"></a>[module mssql.TransactionError.prototype](#apidoc.module.mssql.TransactionError.prototype)

#### <a name="apidoc.element.mssql.TransactionError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">mssql.TransactionError.prototype.</span>constructor (message, code)](#apidoc.element.mssql.TransactionError.prototype.constructor)
- description and source-code
```javascript
function TransactionError(message, code) {
  var err;
  if (!(this instanceof TransactionError)) {
    if (message instanceof Error) {
      err = new TransactionError(message.message, message.code);
      Object.defineProperty(err, 'originalError', {
        value: message
      });
      Error.captureStackTrace(err, arguments.callee);
      return err;
    } else {
      err = new TransactionError(message);
      Error.captureStackTrace(err, arguments.callee);
      return err;
    }
  }
  this.name = this.constructor.name;
  this.message = message;
  if (code != null) {
    this.code = code;
  }
  TransactionError.__super__.constructor.call(this);
  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.UDT"></a>[module mssql.UDT](#apidoc.module.mssql.UDT)

#### <a name="apidoc.element.mssql.UDT.UDT"></a>[function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT.UDT)
- description and source-code
```javascript
UDT = function () {
  return {
    type: TYPES.UDT
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UDT.inspect"></a>[function <span class="apidocSignatureSpan">mssql.UDT.</span>inspect ()](#apidoc.element.mssql.UDT.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.UniqueIdentifier"></a>[module mssql.UniqueIdentifier](#apidoc.module.mssql.UniqueIdentifier)

#### <a name="apidoc.element.mssql.UniqueIdentifier.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier = function () {
  return {
    type: TYPES.UniqueIdentifier
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UniqueIdentifier.inspect"></a>[function <span class="apidocSignatureSpan">mssql.UniqueIdentifier.</span>inspect ()](#apidoc.element.mssql.UniqueIdentifier.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.VarBinary"></a>[module mssql.VarBinary](#apidoc.module.mssql.VarBinary)

#### <a name="apidoc.element.mssql.VarBinary.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary.VarBinary)
- description and source-code
```javascript
VarBinary = function (length) {
  return {
    type: TYPES.VarBinary,
    length: length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarBinary.inspect"></a>[function <span class="apidocSignatureSpan">mssql.VarBinary.</span>inspect ()](#apidoc.element.mssql.VarBinary.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.VarChar"></a>[module mssql.VarChar](#apidoc.module.mssql.VarChar)

#### <a name="apidoc.element.mssql.VarChar.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar.VarChar)
- description and source-code
```javascript
VarChar = function (length) {
  return {
    type: TYPES.VarChar,
    length: length
  };
}
```
- example usage
```shell
...
		// ... query error checks
	});

    // Stored Procedure
	
	new sql.Request()
	.input('input_parameter', sql.Int, value)
    .output('output_parameter', sql.VarChar(50))
	.execute('procedure_name').then(function(recordsets) {
		console.dir(recordsets);
	}).catch(function(err) {
		// ... execute error checks
	});
	
	// ES6 Tagged template literals (experimental)
...
```

#### <a name="apidoc.element.mssql.VarChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.VarChar.</span>inspect ()](#apidoc.element.mssql.VarChar.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Variant"></a>[module mssql.Variant](#apidoc.module.mssql.Variant)

#### <a name="apidoc.element.mssql.Variant.Variant"></a>[function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant.Variant)
- description and source-code
```javascript
Variant = function () {
  return {
    type: TYPES.Variant
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Variant.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Variant.</span>inspect ()](#apidoc.element.mssql.Variant.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.Xml"></a>[module mssql.Xml](#apidoc.module.mssql.Xml)

#### <a name="apidoc.element.mssql.Xml.Xml"></a>[function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml.Xml)
- description and source-code
```javascript
Xml = function () {
  return {
    type: TYPES.Xml
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Xml.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Xml.</span>inspect ()](#apidoc.element.mssql.Xml.inspect)
- description and source-code
```javascript
inspect = function () {
  return "[sql." + key + "]";
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```



# <a name="apidoc.module.mssql.connectionstring"></a>[module mssql.connectionstring](#apidoc.module.mssql.connectionstring)

#### <a name="apidoc.element.mssql.connectionstring.parse"></a>[function <span class="apidocSignatureSpan">mssql.connectionstring.</span>parse (string)](#apidoc.element.mssql.connectionstring.parse)
- description and source-code
```javascript
parse = function (string) {
  var buffer, char, cursor, original, param, parsed, parsing, quotes;
  cursor = 0;
  parsing = 'name';
  param = null;
  buffer = '';
  quotes = null;
  parsed = {};
  original = {};
  Object.defineProperty(parsed, '__original__', {
    value: original
  });
  Object.defineProperty(parsed, 'toString', {
    value: function() {
      var key, value;
      return ((function() {
        var ref, ref1, ref2, ref3, results;
        results = [];
        for (key in this) {
          value = this[key];
          if (indexOf.call(IGNORE_KEYS, key) < 0) {
            results.push(original[key].name + "=" + ((ref = (ref1 = original[key].escape) != null ? ref1[0] : void 0) != null ?
ref : '') + value + ((ref2 = (ref3 = original[key].escape) != null ? ref3[1] : void 0) != null ? ref2 : ''));
          }
        }
        return results;
      }).call(this)).join(';');
    }
  });
  while (cursor < string.length) {
    char = string.charAt(cursor);
    switch (char) {
      case '=':
        if (parsing === 'name') {
          buffer = buffer.trim();
          param = buffer.toLowerCase();
          original[param] = {
            name: buffer
          };
          parsing = 'value';
          buffer = '';
        } else {
          buffer += char;
        }
        break;
      case '\'':
      case '"':
        if (parsing === 'value') {
          if (!buffer.trim().length) {
            original[param].escape = [char, char];
            quotes = char;
            buffer = '';
          } else {
            if (quotes) {
              if (char === quotes) {
                if (char === string.charAt(cursor + 1)) {
                  buffer += char;
                  cursor++;
                } else {
                  parsed[param] = buffer;
                  param = null;
                  parsing = null;
                  buffer = '';
                  quotes = null;
                }
              } else {
                buffer += char;
              }
            } else {
              buffer += char;
            }
          }
        } else {
          throw new Error("Invalid connection string.");
        }
        break;
      case '{':
        if (parsing === 'value') {
          if (!buffer.trim().length) {
            original[param].escape = ['{', '}'];
            quotes = '{}';
            buffer = '';
          } else {
            buffer += char;
          }
        } else {
          throw new Error("Invalid connection string.");
        }
        break;
      case '}':
        if (parsing === 'value') {
          if (quotes === '{}') {
            parsed[param] = buffer;
            param = null;
            parsing = null;
            buffer = '';
            quotes = null;
          } else {
            buffer += char;
          }
        } else {
          throw new Error("Invalid connection string.");
        }
        break;
      case ';':
        if (parsing === 'value') {
          if (quotes) {
            buffer += char;
          } else {
            parsed[param] = buffer;
            param = null;
            parsing = 'name';
            buffer = '';
          }
        } else {
          buffer = '';
          parsing = 'name';
        }
        break;
      default:
        buffer += char;
    }
    cursor++;
  }
  if (parsing === 'value') {
    parsed[param] = buffer;
  }
  return parsed;
}
```
- example usage
```shell
...
} catch (error) {
  ex = error;
  console.error("Failed to load config file. " + ex.message);
  process.exit(1);
}

try {
  config = JSON.parse(config);
} catch (error1) {
  ex = error1;
  console.error("Failed to parse config file. " + ex.message);
  process.exit(1);
}

buffer = [];
...
```

#### <a name="apidoc.element.mssql.connectionstring.resolve"></a>[function <span class="apidocSignatureSpan">mssql.connectionstring.</span>resolve (string)](#apidoc.element.mssql.connectionstring.resolve)
- description and source-code
```javascript
resolve = function (string) {
  var config, parsed, ref, ref1, ref10, ref11, ref12, ref13, ref14, ref15, ref16, ref17, ref2, ref3, ref4, ref5, ref6, ref7, ref8
, ref9, server, user;
  if (/^(mssql|tedious|msnodesql|tds)\:\/\//i.test(string)) {
    parsed = parseConnectionURI(string);
  } else {
    parsed = parseConnectionString(string);
  }
  if (parsed.driver === 'msnodesql') {
    parsed.driver = 'SQL Server Native Client 11.0';
    if ((ref = parsed.__original__) != null) {
      ref.driver = {
        name: 'Driver',
        escape: ['{', '}']
      };
    }
    return {
      driver: 'msnodesql',
      connectionString: parsed.toString()
    };
  }
  user = (ref1 = parsed.uid) != null ? ref1 : parsed['user id'];
  server = (ref2 = (ref3 = (ref4 = (ref5 = parsed.server) != null ? ref5 : parsed.address) != null ? ref4 : parsed.addr) != null
 ? ref3 : parsed['data source']) != null ? ref2 : parsed['network address'];
  config = {
    driver: parsed.driver,
    password: (ref6 = parsed.pwd) != null ? ref6 : parsed.password,
    database: (ref7 = parsed.database) != null ? ref7 : parsed['initial catalog'],
    connectionTimeout: (ref8 = (ref9 = (ref10 = parsed.connectionTimeout) != null ? ref10 : parsed.timeout) != null ? ref9 : parsed
['connect timeout']) != null ? ref8 : parsed['connection timeout'],
    requestTimeout: (ref11 = parsed.requestTimeout) != null ? ref11 : parsed['request timeout'],
    stream: (ref12 = (ref13 = parsed.stream) != null ? ref13.toLowerCase() : void 0) === 'true' || ref12 === 'yes' || ref12 === '
1',
    options: {
      encrypt: (ref14 = (ref15 = parsed.encrypt) != null ? ref15.toLowerCase() : void 0) === 'true' || ref14 === 'yes' || ref14 === '
1'
    }
  };
  if (parsed.useUTC != null) {
    config.options.useUTC = (ref16 = parsed.useUTC.toLowerCase()) === 'true' || ref16 === 'yes' || ref16 === '1';
  }
  if (config.connectionTimeout != null) {
    config.connectionTimeout = parseInt(config.connectionTimeout);
  }
  if (config.requestTimeout != null) {
    config.requestTimeout = parseInt(config.requestTimeout);
  }
  if (/^(.*)\\(.*)$/.exec(user)) {
    config.domain = RegExp.$1;
    user = RegExp.$2;
  }
  if (server) {
    server = server.trim();
    if (/^np\:/i.test(server)) {
      throw new Error("Connection via Named Pipes is not supported.");
    }
    if (/^tcp\:/i.test(server)) {
      server = server.substr(4);
    }
    if (/^(.*)\\(.*)$/.exec(server)) {
      server = RegExp.$1;
      config.options.instanceName = RegExp.$2;
    }
    if (/^(.*),(.*)$/.exec(server)) {
      server = RegExp.$1.trim();
      config.port = parseInt(RegExp.$2.trim());
    }
    if ((ref17 = server.toLowerCase()) === '.' || ref17 === '(.)' || ref17 === '(localdb)' || ref17 === '(local)') {
      server = 'localhost';
    }
  }
  config.user = user;
  config.server = server;
  return config;
}
```
- example usage
```shell
...

cfgPath = process.argv[2];

if (!cfgPath) {
  cfgPath = process.cwd();
}

cfgPath = path.resolve(cfgPath);

if (fs.lstatSync(cfgPath).isDirectory()) {
  cfgPath = path.resolve(cfgPath, './.mssql.json');
}

if (!fs.existsSync(cfgPath)) {
  console.error("Config file not found.");
...
```



# <a name="apidoc.module.mssql.datatypes"></a>[module mssql.datatypes](#apidoc.module.mssql.datatypes)

#### <a name="apidoc.element.mssql.datatypes.cast"></a>[function <span class="apidocSignatureSpan">mssql.datatypes.</span>cast (value, type, options)](#apidoc.element.mssql.datatypes.cast)
- description and source-code
```javascript
cast = function (value, type, options) {
  var ns, ref, scale;
  if (value == null) {
    return null;
  }
  switch (typeof value) {
    case 'string':
      return "N'" + (value.replace(/'/g, '\'\'')) + "'";
    case 'number':
      return value;
    case 'boolean':
      if (value) {
        return 1;
      } else {
        return 0;
      }
    case 'object':
      if (value instanceof Date) {
        ns = value.getUTCMilliseconds() / 1000;
        if (value.nanosecondDelta != null) {
          ns += value.nanosecondDelta;
        }
        scale = (ref = options.scale) != null ? ref : 7;
        if (scale > 0) {
          ns = String(ns).substr(1, scale + 1);
        } else {
          ns = "";
        }
        return "N'" + (value.getUTCFullYear()) + "-" + (zero(value.getUTCMonth() + 1)) + "-" + (zero(value.getUTCDate())) + " " + (
zero(value.getUTCHours())) + ":" + (zero(value.getUTCMinutes())) + ":" + (zero(value.getUTCSeconds())) + ns + "'";
      } else if (Buffer.isBuffer(value)) {
        return "0x" + (value.toString('hex'));
      } else {
        return null;
      }
      break;
    default:
      return null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.datatypes.declare"></a>[function <span class="apidocSignatureSpan">mssql.datatypes.</span>declare (type, options)](#apidoc.element.mssql.datatypes.declare)
- description and source-code
```javascript
declare = function (type, options) {
  var ref, ref1, ref2, ref3, ref4, ref5;
  switch (type) {
    case TYPES.VarChar:
    case TYPES.NVarChar:
    case TYPES.VarBinary:
      return type.declaration + " (" + (options.length > 8000 ? 'MAX' : (ref = options.length) != null ? ref : 'MAX') + ")";
    case TYPES.NVarChar:
      return type.declaration + " (" + (options.length > 4000 ? 'MAX' : (ref1 = options.length) != null ? ref1 : 'MAX') + ")";
    case TYPES.Char:
    case TYPES.NChar:
    case TYPES.Binary:
      return type.declaration + " (" + ((ref2 = options.length) != null ? ref2 : 1) + ")";
    case TYPES.Decimal:
    case TYPES.Numeric:
      return type.declaration + " (" + ((ref3 = options.precision) != null ? ref3 : 18) + ", " + ((ref4 = options.scale) != null
 ? ref4 : 0) + ")";
    case TYPES.Time:
    case TYPES.DateTime2:
    case TYPES.DateTimeOffset:
      return type.declaration + " (" + ((ref5 = options.scale) != null ? ref5 : 7) + ")";
    case TYPES.TVP:
      return options.tvpType + " readonly";
    default:
      return type.declaration;
  }
}
```
- example usage
```shell
...
}
if (table.create) {
  if (table.temporary) {
    objectid = "tempdb..[" + table.name + "]";
  } else {
    objectid = table.path;
  }
  req = new tds.Request("if object_id('" + (objectid.replace(/'/g, '\'\'')) + "') is null " + (table.declare()), function(err) {
    if (err) {
      return done(err);
    }
    return connection.execBulkLoad(bulk);
  });
  return connection.execSqlBatch(req);
} else {
...
```



# <a name="apidoc.module.mssql.map"></a>[module mssql.map](#apidoc.module.mssql.map)

#### <a name="apidoc.element.mssql.map.register"></a>[function <span class="apidocSignatureSpan">mssql.map.</span>register (jstype, sqltype)](#apidoc.element.mssql.map.register)
- description and source-code
```javascript
register = function (jstype, sqltype) {
  var i, index, item, len;
  for (index = i = 0, len = this.length; i < len; index = ++i) {
    item = this[index];
    if (!(item.js === jstype)) {
      continue;
    }
    this.splice(index, 1);
    break;
  }
  this.push({
    js: jstype,
    sql: sqltype
  });
  return null;
}
```
- example usage
```shell
...
- 'sql.Table' -> 'sql.TVP'

Default data type for unknown object is 'sql.NVarChar'.

You can define your own type map.

'''javascript
sql.map.register(MyClass, sql.Text);
'''

You can also overwrite the default type map.

'''javascript
sql.map.register(Number, sql.BigInt);
'''
...
```



# <a name="apidoc.module.mssql.map.0"></a>[module mssql.map.0](#apidoc.module.mssql.map.0)

#### <a name="apidoc.element.mssql.map.0.js"></a>[function <span class="apidocSignatureSpan">mssql.map.0.</span>js ()](#apidoc.element.mssql.map.0.js)
- description and source-code
```javascript
function String() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.0.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.0.</span>sql (length)](#apidoc.element.mssql.map.0.sql)
- description and source-code
```javascript
sql = function (length) {
  return {
    type: TYPES.NVarChar,
    length: length
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.0.js.prototype"></a>[module mssql.map.0.js.prototype](#apidoc.module.mssql.map.0.js.prototype)

#### <a name="apidoc.element.mssql.map.0.js.prototype.entityify"></a>[function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>entityify ()](#apidoc.element.mssql.map.0.js.prototype.entityify)
- description and source-code
```javascript
entityify = function (){return this.replace(/&/g,"&amp;").replace(/</g,"&lt;").replace(/>/g,"&gt;"
)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.0.js.prototype.isAlpha"></a>[function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>isAlpha ( )](#apidoc.element.mssql.map.0.js.prototype.isAlpha)
- description and source-code
```javascript
isAlpha = function ( ){return this>="a"&&this<="z\uffff"||this>="A"&&this<="Z\uffff"}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.0.js.prototype.isDigit"></a>[function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>isDigit ()](#apidoc.element.mssql.map.0.js.prototype.isDigit)
- description and source-code
```javascript
isDigit = function (){return this>="0"&&
this<="9"}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.0.js.prototype.supplant"></a>[function <span class="apidocSignatureSpan">mssql.map.0.js.prototype.</span>supplant (e)](#apidoc.element.mssql.map.0.js.prototype.supplant)
- description and source-code
```javascript
supplant = function (e){return this.replace(/\{([^{}]*)\}/g,function(t,n){var r=e[n];return typeof
r=="string"||typeof r=="number"?r:t})}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.1"></a>[module mssql.map.1](#apidoc.module.mssql.map.1)

#### <a name="apidoc.element.mssql.map.1.js"></a>[function <span class="apidocSignatureSpan">mssql.map.1.</span>js ()](#apidoc.element.mssql.map.1.js)
- description and source-code
```javascript
function Number() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.1.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.1.</span>sql ()](#apidoc.element.mssql.map.1.sql)
- description and source-code
```javascript
sql = function () {
  return {
    type: TYPES.Int
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.2"></a>[module mssql.map.2](#apidoc.module.mssql.map.2)

#### <a name="apidoc.element.mssql.map.2.js"></a>[function <span class="apidocSignatureSpan">mssql.map.2.</span>js ()](#apidoc.element.mssql.map.2.js)
- description and source-code
```javascript
function Boolean() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.2.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.2.</span>sql ()](#apidoc.element.mssql.map.2.sql)
- description and source-code
```javascript
sql = function () {
  return {
    type: TYPES.Bit
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.3"></a>[module mssql.map.3](#apidoc.module.mssql.map.3)

#### <a name="apidoc.element.mssql.map.3.js"></a>[function <span class="apidocSignatureSpan">mssql.map.3.</span>js ()](#apidoc.element.mssql.map.3.js)
- description and source-code
```javascript
function Date() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.3.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.3.</span>sql ()](#apidoc.element.mssql.map.3.sql)
- description and source-code
```javascript
sql = function () {
  return {
    type: TYPES.DateTime
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.4"></a>[module mssql.map.4](#apidoc.module.mssql.map.4)

#### <a name="apidoc.element.mssql.map.4.js"></a>[function <span class="apidocSignatureSpan">mssql.map.4.</span>js (arg, encodingOrOffset, length)](#apidoc.element.mssql.map.4.js)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.4.</span>sql (length)](#apidoc.element.mssql.map.4.sql)
- description and source-code
```javascript
sql = function (length) {
  return {
    type: TYPES.VarBinary,
    length: length
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.4.js.prototype"></a>[module mssql.map.4.js.prototype](#apidoc.module.mssql.map.4.js.prototype)

#### <a name="apidoc.element.mssql.map.4.js.prototype.asciiSlice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>asciiSlice ()](#apidoc.element.mssql.map.4.js.prototype.asciiSlice)
- description and source-code
```javascript
function asciiSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.asciiWrite"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>asciiWrite ()](#apidoc.element.mssql.map.4.js.prototype.asciiWrite)
- description and source-code
```javascript
function asciiWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.base64Slice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>base64Slice ()](#apidoc.element.mssql.map.4.js.prototype.base64Slice)
- description and source-code
```javascript
function base64Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.base64Write"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>base64Write ()](#apidoc.element.mssql.map.4.js.prototype.base64Write)
- description and source-code
```javascript
function base64Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.compare"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.mssql.map.4.js.prototype.compare)
- description and source-code
```javascript
function compare(target, start, end, thisStart, thisEnd) {

  if (!(target instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');
  if (arguments.length === 1)
    return compare_(this, target);

  if (start === undefined)
    start = 0;
  else if (start < 0)
    throw new RangeError('out of range index');
  else
    start >>>= 0;

  if (end === undefined)
    end = target.length;
  else if (end > target.length)
    throw new RangeError('out of range index');
  else
    end >>>= 0;

  if (thisStart === undefined)
    thisStart = 0;
  else if (thisStart < 0)
    throw new RangeError('out of range index');
  else
    thisStart >>>= 0;

  if (thisEnd === undefined)
    thisEnd = this.length;
  else if (thisEnd > this.length)
    throw new RangeError('out of range index');
  else
    thisEnd >>>= 0;

  if (thisStart >= thisEnd)
    return (start >= end ? 0 : -1);
  else if (start >= end)
    return 1;

  return compareOffset(this, target, start, thisStart, end, thisEnd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.copy"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>copy ()](#apidoc.element.mssql.map.4.js.prototype.copy)
- description and source-code
```javascript
function copy() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.equals"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>equals (other)](#apidoc.element.mssql.map.4.js.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  if (this.length !== other.length) {
    return false;
  }

  for (var i = 0, len = this.length; i < len; i++) {
    if (this[i] !== other[i]) {
      return false;
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.fill"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.mssql.map.4.js.prototype.fill)
- description and source-code
```javascript
function fill(val, start, end, encoding) {
  // Handle string cases:
  if (typeof val === 'string') {
    if (typeof start === 'string') {
      encoding = start;
      start = 0;
      end = this.length;
    } else if (typeof end === 'string') {
      encoding = end;
      end = this.length;
    }

    if (encoding !== undefined && typeof encoding !== 'string') {
      throw new TypeError('encoding must be a string');
    }
    var normalizedEncoding = internalUtil.normalizeEncoding(encoding);
    if (normalizedEncoding === undefined) {
      throw new TypeError('Unknown encoding: ' + encoding);
    }

    if (val.length === 0) {
      // Previously, if val === '', the Buffer would not fill,
      // which is rather surprising.
      val = 0;
    } else if (val.length === 1) {
      var code = val.charCodeAt(0);
      if ((normalizedEncoding === 'utf8' && code < 128) ||
          normalizedEncoding === 'latin1') {
        // Fast path: If 'val' fits into a single byte, use that numeric value.
        val = code;
      }
    }
  } else if (typeof val === 'number') {
    val = val & 255;
  }

  // Invalid ranges are not set to a default, so can range check early.
  if (start < 0 || end > this.length)
    throw new RangeError('Out of range index');

  if (end <= start)
    return this;

  start = start >>> 0;
  end = end === undefined ? this.length : end >>> 0;

  binding.fill(this, val, start, end, encoding);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.hexSlice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>hexSlice ()](#apidoc.element.mssql.map.4.js.prototype.hexSlice)
- description and source-code
```javascript
function hexSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.hexWrite"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>hexWrite ()](#apidoc.element.mssql.map.4.js.prototype.hexWrite)
- description and source-code
```javascript
function hexWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.includes"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.includes)
- description and source-code
```javascript
function includes(val, byteOffset, encoding) {
  return this.indexOf(val, byteOffset, encoding) !== -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.indexOf)
- description and source-code
```javascript
function indexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.inspect"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>inspect ()](#apidoc.element.mssql.map.4.js.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var str = '';
  var max = exports.INSPECT_MAX_BYTES;
  if (this.length > 0) {
    str = this.toString('hex', 0, max).match(/.{2}/g).join(' ');
    if (this.length > max)
      str += ' ... ';
  }
  return '<' + this.constructor.name + ' ' + str + '>';
}
```
- example usage
```shell
...
  }
} else {
  row = {};
  row[Object.keys(columns)[0]] = chunksBuffer.join('');
}
chunksBuffer = null;
if (_this.verbose) {
  _this._log(util.inspect(row));
  _this._log("---------- --------------------");
}
if (_this.stream) {
  _this.emit('row', row);
} else {
  recordset.push(row);
}
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.mssql.map.4.js.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.latin1Slice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>latin1Slice ()](#apidoc.element.mssql.map.4.js.prototype.latin1Slice)
- description and source-code
```javascript
function latin1Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.latin1Write"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>latin1Write ()](#apidoc.element.mssql.map.4.js.prototype.latin1Write)
- description and source-code
```javascript
function latin1Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readDoubleBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readDoubleBE)
- description and source-code
```javascript
function readDoubleBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readDoubleLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readDoubleLE)
- description and source-code
```javascript
function readDoubleLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleLE(this, offset);
}
```
- example usage
```shell
...
  var i, j, point, points, ref;
  points = [];
  if (count < 1) {
    return points;
  }
  for (i = j = 1, ref = count; 1 <= ref ? j <= ref : j >= ref; i = 1 <= ref ? ++j : --j) {
    points.push((point = new Point));
    point.x = buffer.readDoubleLE(buffer.position);
    point.y = buffer.readDoubleLE(buffer.position + 8);
    buffer.position += 16;
  }
  return points;
};

parseZ = function(buffer, points) {
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readFloatBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readFloatBE)
- description and source-code
```javascript
function readFloatBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readFloatLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readFloatLE)
- description and source-code
```javascript
function readFloatLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readInt16BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt16BE)
- description and source-code
```javascript
readInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset + 1] | (this[offset] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readInt16LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt16LE)
- description and source-code
```javascript
readInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset] | (this[offset + 1] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readInt32BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt32BE)
- description and source-code
```javascript
readInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] << 24) |
      (this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      (this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readInt32LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt32LE)
- description and source-code
```javascript
readInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16) |
      (this[offset + 3] << 24);
}
```
- example usage
```shell
...
})();

parseGeography = function(buffer, geometry) {
  var flags, numberOfFigures, numberOfPoints, numberOfSegments, numberOfShapes, properties, srid, value;
  if (geometry == null) {
    geometry = false;
  }
  srid = buffer.readInt32LE(0);
  if (srid === -1) {
    return null;
  }
  value = {
    srid: srid,
    version: buffer.readUInt8(4)
  };
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readInt8"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readInt8)
- description and source-code
```javascript
readInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  var val = this[offset];
  return !(val & 0x80) ? val : (0xff - val + 1) * -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readIntBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readIntBE)
- description and source-code
```javascript
readIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var i = byteLength;
  var mul = 1;
  var val = this[offset + --i];
  while (i > 0 && (mul *= 0x100))
    val += this[offset + --i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readIntLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readIntLE)
- description and source-code
```javascript
readIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUInt16BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt16BE)
- description and source-code
```javascript
readUInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return (this[offset] << 8) | this[offset + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUInt16LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt16LE)
- description and source-code
```javascript
readUInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return this[offset] | (this[offset + 1] << 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUInt32BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt32BE)
- description and source-code
```javascript
readUInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] * 0x1000000) +
      ((this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUInt32LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt32LE)
- description and source-code
```javascript
readUInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return ((this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16)) +
      (this[offset + 3] * 0x1000000);
}
```
- example usage
```shell
...
  properties.H = flags & (1 << 3) ? true : false;
}
if (properties.P) {
  numberOfPoints = 1;
} else if (properties.L) {
  numberOfPoints = 2;
} else {
  numberOfPoints = buffer.readUInt32LE(buffer.position);
  buffer.position += 4;
}
value.points = parsePoints(buffer, numberOfPoints);
if (properties.Z) {
  parseZ(buffer, value.points);
}
if (properties.M) {
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUInt8"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUInt8)
- description and source-code
```javascript
readUInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  return this[offset];
}
```
- example usage
```shell
...
}
srid = buffer.readInt32LE(0);
if (srid === -1) {
  return null;
}
value = {
  srid: srid,
  version: buffer.readUInt8(4)
};
flags = buffer.readUInt8(5);
buffer.position = 6;
properties = {
  Z: flags & (1 << 0) ? true : false,
  M: flags & (1 << 1) ? true : false,
  V: flags & (1 << 2) ? true : false,
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUIntBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUIntBE)
- description and source-code
```javascript
readUIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset + --byteLength];
  var mul = 1;
  while (byteLength > 0 && (mul *= 0x100))
    val += this[offset + --byteLength] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.readUIntLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.readUIntLE)
- description and source-code
```javascript
readUIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.slice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>slice (start, end)](#apidoc.element.mssql.map.4.js.prototype.slice)
- description and source-code
```javascript
function slice(start, end) {
  const srcLength = this.length;
  start = adjustOffset(start, srcLength);
  end = end !== undefined ? adjustOffset(end, srcLength) : srcLength;
  const newLength = end > start ? end - start : 0;
  return new FastBuffer(this.buffer, this.byteOffset + start, newLength);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.swap16"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap16 ()](#apidoc.element.mssql.map.4.js.prototype.swap16)
- description and source-code
```javascript
function swap16() {
  // For Buffer.length < 128, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 2 !== 0)
    throw new RangeError('Buffer size must be a multiple of 16-bits');
  if (len < 128) {
    for (var i = 0; i < len; i += 2)
      swap(this, i, i + 1);
    return this;
  }
  return swap16n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.swap32"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap32 ()](#apidoc.element.mssql.map.4.js.prototype.swap32)
- description and source-code
```javascript
function swap32() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 4 !== 0)
    throw new RangeError('Buffer size must be a multiple of 32-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 4) {
      swap(this, i, i + 3);
      swap(this, i + 1, i + 2);
    }
    return this;
  }
  return swap32n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.swap64"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>swap64 ()](#apidoc.element.mssql.map.4.js.prototype.swap64)
- description and source-code
```javascript
function swap64() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 8 !== 0)
    throw new RangeError('Buffer size must be a multiple of 64-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 8) {
      swap(this, i, i + 7);
      swap(this, i + 1, i + 6);
      swap(this, i + 2, i + 5);
      swap(this, i + 3, i + 4);
    }
    return this;
  }
  return swap64n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.toByteArray"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toByteArray ()](#apidoc.element.mssql.map.4.js.prototype.toByteArray)
- description and source-code
```javascript
toByteArray = function () {
  return Array.prototype.slice.call(this, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toJSON ()](#apidoc.element.mssql.map.4.js.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return "0x" + (this.toString('hex'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.toString"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toString ()](#apidoc.element.mssql.map.4.js.prototype.toString)
- description and source-code
```javascript
toString = function () {
  let result;
  if (arguments.length === 0) {
    result = this.utf8Slice(0, this.length);
  } else {
    result = slowToString.apply(this, arguments);
  }
  if (result === undefined)
    throw new Error('"toString()" failed');
  return result;
}
```
- example usage
```shell
...
sql = require('./main');

write = function(text) {
  return process.stdout.write(text);
};

Buffer.prototype.toJSON = function() {
  return "0x" + (this.toString('hex'));
};

cfgPath = process.argv[2];

if (!cfgPath) {
  cfgPath = process.cwd();
}
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.ucs2Slice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>ucs2Slice ()](#apidoc.element.mssql.map.4.js.prototype.ucs2Slice)
- description and source-code
```javascript
function ucs2Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.ucs2Write"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>ucs2Write ()](#apidoc.element.mssql.map.4.js.prototype.ucs2Write)
- description and source-code
```javascript
function ucs2Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.utf8Slice"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>utf8Slice ()](#apidoc.element.mssql.map.4.js.prototype.utf8Slice)
- description and source-code
```javascript
function utf8Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.utf8Write"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>utf8Write ()](#apidoc.element.mssql.map.4.js.prototype.utf8Write)
- description and source-code
```javascript
function utf8Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.write"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.mssql.map.4.js.prototype.write)
- description and source-code
```javascript
write = function (string, offset, length, encoding) {
  // Buffer#write(string);
  if (offset === undefined) {
    encoding = 'utf8';
    length = this.length;
    offset = 0;

  // Buffer#write(string, encoding)
  } else if (length === undefined && typeof offset === 'string') {
    encoding = offset;
    length = this.length;
    offset = 0;

  // Buffer#write(string, offset[, length][, encoding])
  } else if (isFinite(offset)) {
    offset = offset >>> 0;
    if (isFinite(length)) {
      length = length >>> 0;
      if (encoding === undefined)
        encoding = 'utf8';
    } else {
      encoding = length;
      length = undefined;
    }
  } else {
    // if someone is still calling the obsolete form of write(), tell them.
    // we don't want eg buf.write("foo", "utf8", 10) to silently turn into
    // buf.write("foo", "utf8"), so we can't ignore extra args
    throw new Error('Buffer.write(string, encoding, offset[, length]) ' +
                    'is no longer supported');
  }

  var remaining = this.length - offset;
  if (length === undefined || length > remaining)
    length = remaining;

  if (string.length > 0 && (length < 0 || offset < 0))
    throw new RangeError('Attempt to write outside buffer bounds');

  if (!encoding)
    encoding = 'utf8';

  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'hex':
        return this.hexWrite(string, offset, length);

      case 'utf8':
      case 'utf-8':
        return this.utf8Write(string, offset, length);

      case 'ascii':
        return this.asciiWrite(string, offset, length);

      case 'latin1':
      case 'binary':
        return this.latin1Write(string, offset, length);

      case 'base64':
        // Warning: maxLength not taken into account in base64Write
        return this.base64Write(string, offset, length);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return this.ucs2Write(string, offset, length);

      default:
        if (loweredCase)
          throw new TypeError('Unknown encoding: ' + encoding);
        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
...
fs = require('fs');

path = require('path');

sql = require('./main');

write = function(text) {
  return process.stdout.write(text);
};

Buffer.prototype.toJSON = function() {
  return "0x" + (this.toString('hex'));
};

cfgPath = process.argv[2];
...
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeDoubleBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeDoubleBE)
- description and source-code
```javascript
function writeDoubleBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleBE(this, val, offset);
  else
    binding.writeDoubleBE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeDoubleLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeDoubleLE)
- description and source-code
```javascript
function writeDoubleLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleLE(this, val, offset);
  else
    binding.writeDoubleLE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeFloatBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeFloatBE)
- description and source-code
```javascript
function writeFloatBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatBE(this, val, offset);
  else
    binding.writeFloatBE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeFloatLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeFloatLE)
- description and source-code
```javascript
function writeFloatLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatLE(this, val, offset);
  else
    binding.writeFloatLE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeInt16BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt16BE)
- description and source-code
```javascript
writeInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeInt16LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt16LE)
- description and source-code
```javascript
writeInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeInt32BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt32BE)
- description and source-code
```javascript
writeInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeInt32LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt32LE)
- description and source-code
```javascript
writeInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  this[offset + 2] = (value >>> 16);
  this[offset + 3] = (value >>> 24);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeInt8"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeInt8)
- description and source-code
```javascript
writeInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0x7f, -0x80);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeIntBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeIntBE)
- description and source-code
```javascript
writeIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = byteLength - 1;
  var mul = 1;
  var sub = 0;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i + 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeIntLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeIntLE)
- description and source-code
```javascript
writeIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = 0;
  var mul = 1;
  var sub = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i - 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUInt16BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt16BE)
- description and source-code
```javascript
writeUInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUInt16LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt16LE)
- description and source-code
```javascript
writeUInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUInt32BE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt32BE)
- description and source-code
```javascript
writeUInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUInt32LE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt32LE)
- description and source-code
```javascript
writeUInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset + 3] = (value >>> 24);
  this[offset + 2] = (value >>> 16);
  this[offset + 1] = (value >>> 8);
  this[offset] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUInt8"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUInt8)
- description and source-code
```javascript
writeUInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0xff, 0);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUIntBE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUIntBE)
- description and source-code
```javascript
writeUIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var i = byteLength - 1;
  var mul = 1;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.4.js.prototype.writeUIntLE"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.mssql.map.4.js.prototype.writeUIntLE)
- description and source-code
```javascript
writeUIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var mul = 1;
  var i = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map.5"></a>[module mssql.map.5](#apidoc.module.mssql.map.5)

#### <a name="apidoc.element.mssql.map.5.js"></a>[function <span class="apidocSignatureSpan">mssql.map.5.</span>js (name)](#apidoc.element.mssql.map.5.js)
- description and source-code
```javascript
function Table(name) {
  var ref1;
  if (name) {
    ref1 = Table.parseName(name), this.name = ref1.name, this.schema = ref1.schema, this.database = ref1.database;
    this.path = "" + (this.database ? "[" + this.database + "]." : "") + (this.schema ? "[" + this.schema + "]." : "") + "[" + this
.name + "]";
    this.temporary = this.name.charAt(0) === '#';
  }
  this.columns = [];
  this.rows = [];
  Object.defineProperty(this.columns, "add", {
    value: function(name, column, options) {
      if (options == null) {
        options = {};
      }
      if (column == null) {
        throw new Error("Column data type is not defined.");
      }
      if (column instanceof Function) {
        column = column();
      }
      column.name = name;
      column.nullable = options.nullable;
      column.primary = options.primary;
      return this.push(column);
    }
  });
  Object.defineProperty(this.rows, "add", {
    value: function() {
      var values;
      values = 1 <= arguments.length ? slice.call(arguments, 0) : [];
      return this.push(values);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.5.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.5.</span>sql (tvpType)](#apidoc.element.mssql.map.5.sql)
- description and source-code
```javascript
sql = function (tvpType) {
  return {
    type: TYPES.TVP,
    tvpType: tvpType
  };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
