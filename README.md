# api documentation for  [mssql (v4.0.1)](https://github.com/patriksimek/node-mssql#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mssql.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mssql) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mssql.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mssql)
#### Microsoft SQL Server client for Node.js.

[![NPM](https://nodei.co/npm/mssql.png?downloads=true)](https://www.npmjs.com/package/mssql)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mssql/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mssql_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mssql/build/apidoc.html)

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
        "shasum": "5ac0028245f99a6bc8bd8dcd117c34244eba9f5b",
        "tarball": "https://registry.npmjs.org/mssql/-/mssql-4.0.1.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "e36e30aba611866b2095f8f7f1405911f9d273ca",
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
        "test": "standard && node_modules/.bin/mocha test/common/unit.js",
        "test-cli": "mocha test/common/cli.js",
        "test-msnodesqlv8": "mocha test/msnodesqlv8",
        "test-tedious": "mocha test/tedious"
    },
    "version": "4.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mssql](#apidoc.module.mssql)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BIGINT ()](#apidoc.element.mssql.BIGINT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BINARY (length)](#apidoc.element.mssql.BINARY)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BIT ()](#apidoc.element.mssql.BIT)
1.  [function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit)
1.  [function <span class="apidocSignatureSpan">mssql.</span>CHAR (length)](#apidoc.element.mssql.CHAR)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char)
1.  [function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>ConnectionPool ()](#apidoc.element.mssql.ConnectionPool)
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
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (parent)](#apidoc.element.mssql.PreparedStatement)
1.  [function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Promise ()](#apidoc.element.mssql.Promise)
1.  [function <span class="apidocSignatureSpan">mssql.</span>REAL ()](#apidoc.element.mssql.REAL)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Request (batch, callback)](#apidoc.element.mssql.Request)
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
1.  [function <span class="apidocSignatureSpan">mssql.</span>Transaction (parent)](#apidoc.element.mssql.Transaction)
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
1.  [function <span class="apidocSignatureSpan">mssql.</span>off (event, handler)](#apidoc.element.mssql.off)
1.  [function <span class="apidocSignatureSpan">mssql.</span>on (event, handler)](#apidoc.element.mssql.on)
1.  [function <span class="apidocSignatureSpan">mssql.</span>query ()](#apidoc.element.mssql.query)
1.  [function <span class="apidocSignatureSpan">mssql.</span>removeListener (event, handler)](#apidoc.element.mssql.removeListener)
1.  number <span class="apidocSignatureSpan">mssql.</span>MAX
1.  object <span class="apidocSignatureSpan">mssql.</span>ISOLATION_LEVEL
1.  object <span class="apidocSignatureSpan">mssql.</span>TYPES
1.  object <span class="apidocSignatureSpan">mssql.</span>Table.prototype
1.  object <span class="apidocSignatureSpan">mssql.</span>base
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

#### [module mssql.Real](#apidoc.module.mssql.Real)
1.  [function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real.Real)
1.  [function <span class="apidocSignatureSpan">mssql.Real.</span>inspect ()](#apidoc.element.mssql.Real.inspect)
1.  string <span class="apidocSignatureSpan">mssql.Real.</span>declaration

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

#### [module mssql.base](#apidoc.module.mssql.base)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>ConnectionError (message, code)](#apidoc.element.mssql.base.ConnectionError)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>ConnectionPool (config, callback)](#apidoc.element.mssql.base.ConnectionPool)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>PreparedStatement (parent)](#apidoc.element.mssql.base.PreparedStatement)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.base.PreparedStatementError)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>Request (parent)](#apidoc.element.mssql.base.Request)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>RequestError (message, code)](#apidoc.element.mssql.base.RequestError)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>Transaction (parent)](#apidoc.element.mssql.base.Transaction)
1.  [function <span class="apidocSignatureSpan">mssql.base.</span>TransactionError (message, code)](#apidoc.element.mssql.base.TransactionError)
1.  object <span class="apidocSignatureSpan">mssql.base.</span>driver
1.  object <span class="apidocSignatureSpan">mssql.base.</span>exports

#### [module mssql.connectionstring](#apidoc.module.mssql.connectionstring)
1.  [function <span class="apidocSignatureSpan">mssql.connectionstring.</span>parse (string)](#apidoc.element.mssql.connectionstring.parse)
1.  [function <span class="apidocSignatureSpan">mssql.connectionstring.</span>resolve (string, driver)](#apidoc.element.mssql.connectionstring.resolve)

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
1.  [function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>equals (b)](#apidoc.element.mssql.map.4.js.prototype.equals)
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
BigInt() {
  return {type: TYPES.BigInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BINARY"></a>[function <span class="apidocSignatureSpan">mssql.</span>BINARY (length)](#apidoc.element.mssql.BINARY)
- description and source-code
```javascript
Binary(length) {
  return {type: TYPES.Binary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BIT"></a>[function <span class="apidocSignatureSpan">mssql.</span>BIT ()](#apidoc.element.mssql.BIT)
- description and source-code
```javascript
Bit() {
  return {type: TYPES.Bit}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt)
- description and source-code
```javascript
BigInt() {
  return {type: TYPES.BigInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Binary"></a>[function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary)
- description and source-code
```javascript
Binary(length) {
  return {type: TYPES.Binary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Bit"></a>[function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit)
- description and source-code
```javascript
Bit() {
  return {type: TYPES.Bit}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.CHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>CHAR (length)](#apidoc.element.mssql.CHAR)
- description and source-code
```javascript
Char(length) {
  return {type: TYPES.Char, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Char"></a>[function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char)
- description and source-code
```javascript
Char(length) {
  return {type: TYPES.Char, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.ConnectionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>ConnectionError (message, code)](#apidoc.element.mssql.ConnectionError)
- description and source-code
```javascript
class ConnectionError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new ConnectionError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'ConnectionError'
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.ConnectionPool"></a>[function <span class="apidocSignatureSpan">mssql.</span>ConnectionPool ()](#apidoc.element.mssql.ConnectionPool)
- description and source-code
```javascript
class ConnectionPool extends base.ConnectionPool {
  _poolCreate () {
    return new base.Promise((resolve, reject) => {
      const cfg = {
        userName: this.config.user,
        password: this.config.password,
        server: this.config.server,
        options: Object.assign({}, this.config.options),
        domain: this.config.domain
      }

      cfg.options.database = this.config.database
      cfg.options.port = this.config.port
      cfg.options.connectTimeout = this.config.connectionTimeout || this.config.timeout || 15000
      cfg.options.requestTimeout = this.config.requestTimeout != null ? this.config.requestTimeout : 15000
      cfg.options.tdsVersion = cfg.options.tdsVersion || '7_4'
      cfg.options.rowCollectionOnDone = false
      cfg.options.rowCollectionOnRequestCompletion = false
      cfg.options.useColumnNames = false
      cfg.options.appName = cfg.options.appName || 'node-mssql'

      // tedious always connect via tcp when port is specified
      if (cfg.options.instanceName) delete cfg.options.port

      if (isNaN(cfg.options.requestTimeout)) cfg.options.requestTimeout = 15000
      if (cfg.options.requestTimeout === Infinity) cfg.options.requestTimeout = 0
      if (cfg.options.requestTimeout < 0) cfg.options.requestTimeout = 0

      if (this.config.debug) {
        cfg.options.debug = {
          packet: true,
          token: true,
          data: true,
          payload: true
        }
      }

      const tedious = new tds.Connection(cfg)

      tedious.once('connect', err => {
        if (err) {
          err = new base.ConnectionError(err)
          return reject(err)
        }

        resolve(tedious)
      })

      tedious.on('error', err => {
        if (err.code === 'ESOCKET') {
          tedious.hasError = true
          return
        }

        this.emit('error', err)
      })

      if (this.config.debug) {
        tedious.on('debug', msg => this._debug(msg))
      }
    })
  }

  _poolValidate (tedious) {
    return new base.Promise((resolve, reject) => {
      resolve(!tedious.closed && !tedious.hasError)
    })
  }

  _poolDestroy (tedious) {
    return new base.Promise((resolve, reject) => {
      tedious.once('end', () => {
        resolve()
      })

      tedious.close()
    })
  }
}
```
- example usage
```shell
...
'''

## Connection Pools

'''javascript
const sql = require('mssql')

const pool1 = new sql.ConnectionPool(config, err => {
// ... error checks

// Query

pool1.request() // or: new sql.Request(pool1)
.query('select 1 as number', (err, result) => {
    // ... error checks
...
```

#### <a name="apidoc.element.mssql.DATE"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATE ()](#apidoc.element.mssql.DATE)
- description and source-code
```javascript
Date() {
  return {type: TYPES.Date}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIME ()](#apidoc.element.mssql.DATETIME)
- description and source-code
```javascript
DateTime() {
  return {type: TYPES.DateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIME2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIME2 (scale)](#apidoc.element.mssql.DATETIME2)
- description and source-code
```javascript
DateTime2(scale) {
  return {type: TYPES.DateTime2, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DATETIMEOFFSET"></a>[function <span class="apidocSignatureSpan">mssql.</span>DATETIMEOFFSET (scale)](#apidoc.element.mssql.DATETIMEOFFSET)
- description and source-code
```javascript
DateTimeOffset(scale) {
  return {type: TYPES.DateTimeOffset, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DECIMAL"></a>[function <span class="apidocSignatureSpan">mssql.</span>DECIMAL (precision, scale)](#apidoc.element.mssql.DECIMAL)
- description and source-code
```javascript
Decimal(precision, scale) {
  return {type: TYPES.Decimal, precision, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Date"></a>[function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date)
- description and source-code
```javascript
Date() {
  return {type: TYPES.Date}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime)
- description and source-code
```javascript
DateTime() {
  return {type: TYPES.DateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2)
- description and source-code
```javascript
DateTime2(scale) {
  return {type: TYPES.DateTime2, scale}
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
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
DateTimeOffset(scale) {
  return {type: TYPES.DateTimeOffset, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal)
- description and source-code
```javascript
Decimal(precision, scale) {
  return {type: TYPES.Decimal, precision, scale}
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc")               // varchar(3)
request.input("name", sql.VarChar(50), "abc")           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc")      // varchar(MAX)
request.output("name", sql.VarChar)                     // varchar(8000)
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.FLOAT"></a>[function <span class="apidocSignatureSpan">mssql.</span>FLOAT ()](#apidoc.element.mssql.FLOAT)
- description and source-code
```javascript
Float() {
  return {type: TYPES.Float}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Float"></a>[function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float)
- description and source-code
```javascript
Float() {
  return {type: TYPES.Float}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.GEOGRAPHY"></a>[function <span class="apidocSignatureSpan">mssql.</span>GEOGRAPHY ()](#apidoc.element.mssql.GEOGRAPHY)
- description and source-code
```javascript
Geography() {
  return {type: TYPES.Geography}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.GEOMETRY"></a>[function <span class="apidocSignatureSpan">mssql.</span>GEOMETRY ()](#apidoc.element.mssql.GEOMETRY)
- description and source-code
```javascript
Geometry() {
  return {type: TYPES.Geometry}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geography"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography)
- description and source-code
```javascript
Geography() {
  return {type: TYPES.Geography}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry)
- description and source-code
```javascript
Geometry() {
  return {type: TYPES.Geometry}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.IMAGE"></a>[function <span class="apidocSignatureSpan">mssql.</span>IMAGE ()](#apidoc.element.mssql.IMAGE)
- description and source-code
```javascript
Image() {
  return {type: TYPES.Image}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.INT"></a>[function <span class="apidocSignatureSpan">mssql.</span>INT ()](#apidoc.element.mssql.INT)
- description and source-code
```javascript
Int() {
  return {type: TYPES.Int}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Image"></a>[function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image)
- description and source-code
```javascript
Image() {
  return {type: TYPES.Image}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Int"></a>[function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int)
- description and source-code
```javascript
Int() {
  return {type: TYPES.Int}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.MONEY"></a>[function <span class="apidocSignatureSpan">mssql.</span>MONEY ()](#apidoc.element.mssql.MONEY)
- description and source-code
```javascript
Money() {
  return {type: TYPES.Money}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Money"></a>[function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money)
- description and source-code
```javascript
Money() {
  return {type: TYPES.Money}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>NCHAR (length)](#apidoc.element.mssql.NCHAR)
- description and source-code
```javascript
NChar(length) {
  return {type: TYPES.NChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar)
- description and source-code
```javascript
NChar(length) {
  return {type: TYPES.NChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NTEXT"></a>[function <span class="apidocSignatureSpan">mssql.</span>NTEXT ()](#apidoc.element.mssql.NTEXT)
- description and source-code
```javascript
NText() {
  return {type: TYPES.NText}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NText"></a>[function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText)
- description and source-code
```javascript
NText() {
  return {type: TYPES.NText}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NUMERIC"></a>[function <span class="apidocSignatureSpan">mssql.</span>NUMERIC (precision, scale)](#apidoc.element.mssql.NUMERIC)
- description and source-code
```javascript
Numeric(precision, scale) {
  return {type: TYPES.Numeric, precision, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVARCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVARCHAR (length)](#apidoc.element.mssql.NVARCHAR)
- description and source-code
```javascript
NVarChar(length) {
  return {type: TYPES.NVarChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar)
- description and source-code
```javascript
NVarChar(length) {
  return {type: TYPES.NVarChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric)
- description and source-code
```javascript
Numeric(precision, scale) {
  return {type: TYPES.Numeric, precision, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.PreparedStatement"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatement (parent)](#apidoc.element.mssql.PreparedStatement)
- description and source-code
```javascript
class PreparedStatement extends EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new Prepared Statement.
   *
   * @param {ConnectionPool|Transaction} [holder]
   */
</span>
  constructor (parent) {
    super()

    this.parent = parent || globalConnection
    this._handle = 0
    this.prepared = false
    this.parameters = {}
  }

  get connected () {
    return this.parent.connected
  }

  /**
   * Acquire connection from connection pool.
   *
   * @param {Request} request Request.
   * @param {ConnectionPool~acquireCallback} [callback] A callback which is called after connection has established, or an error
 has occurred. If omited, method returns Promise.
   * @return {PreparedStatement|Promise}
   */

  acquire (request, callback) {
    debug('ps: acquire')

    if (!this._acquiredConnection) {
      setImmediate(callback, new PreparedStatementError('Statement is not prepared. Call prepare() first.', 'ENOTPREPARED'))
      return this
    }

    if (this._activeRequest) {
      setImmediate(callback, new TransactionError("Can't acquire connection for the request. There is another request in progress
.", 'EREQINPROG'))
      return this
    }

    debug('ps: acquire ok')

    this._activeRequest = request
    setImmediate(callback, null, this._acquiredConnection)
    return this
  }

  /**
   * Release connection back to the pool.
   *
   * @param {Connection} connection Previously acquired connection.
   * @return {PreparedStatement}
   */

  release (connection) {
    debug('ps: release')

    if (connection === this._acquiredConnection) {
      this._activeRequest = null
      debug('ps: release ok')
    }

    return this
  }

  /**
   * Add an input parameter to the prepared statement.
   *
   * @param {String} name Name of the input parameter without @ char.
   * @param {*} type SQL data type of input parameter.
   * @return {PreparedStatement}
   */

  input (name, type) {
    if ((/(--| |\/\*|\*\/|')/).test(name)) {
      throw new PreparedStatementError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if (arguments.length < 2) {
      throw new PreparedStatementError('Invalid number of arguments. 2 arguments expected.', 'EARGS')
    }

    if (type instanceof Function) {
      type = type()
    }

    this.parameters[name] = {
      name,
      type: type.type,
      io: 1,
      length: type.length,
      scale: type.scale,
      precision: type.precision,
      tvpType: type.tvpType
    }

    return this
  }

  /**
   * Add an output parameter to the prepared statement.
   *
   * @param {String} name Name of the output parameter without @ char.
   * @param {*} type SQL data type of output parameter.
   * @return {PreparedStatement}
   */

  output (name, type) {
    if (/(--| |\/\*|\*\/|')/.test(name)) {
      throw new PreparedStatementError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if (arguments.length < 2) {
      throw new PreparedStatementError('Invalid number of arguments. 2 arguments expected.', 'EARGS')
    }

    if (type instanceof Function) type = type()

    this.parameters[name] = {
      name,
      type: type.type,
      io: 2,
      length: type.length,
      scale: type.scale,
      precision: type.precision
    }

    return this
  }

  /**
   * Prepare a statement.
   *
   * @param {String} statement SQL statement to prepare.
   * @param {basicCallback} [callback] A callback which is called after preparation has completed, or an error has occurred. If
omited, method returns Promise.
   * @return {PreparedStatement|Promise}
   */

  prepare (statement, callback) {
    if (typeof callback === 'function') {
      this._prepare(statement, callback)
      return this
    }

    return new PromiseLibrary((resolve, reject) => {
      this._prepare(statement, err => {
        if (err) return reject(err)
        resolve(this)
      })
    })
  }

  /**
   * @private
   * @param {String} statement
   * @param {basicCallback} callback
   */

  _prepare (statement, callback) {
    debug('ps: prepare')

    if (typeof statement === 'function') {
      callback = statement ...
```
- example usage
```shell
...
- EREQINPROG ('TransactionError') - Can't rollback transaction. There is a request in progress.

## Prepared Statement

**IMPORTANT:** always use 'PreparedStatement' class to create prepared statements - it ensures that all your executions of prepared
 statement are executed on one connection. Once you call 'prepare', a single connection is acquired from the connection pool and
 all subsequent executions are executed exclusively on this connection. After you call 'unprepare', the connection is then released
 back to the connection pool.

'''javascript
const ps = new sql.PreparedStatement(/* [pool] */)
'''

If you omit the connection argument, the global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.PreparedStatementError"></a>[function <span class="apidocSignatureSpan">mssql.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.PreparedStatementError)
- description and source-code
```javascript
class PreparedStatementError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new PreparedStatementError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'PreparedStatementError'
  }
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
Real() {
  return {type: TYPES.Real}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Real"></a>[function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real)
- description and source-code
```javascript
Real() {
  return {type: TYPES.Real}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Request"></a>[function <span class="apidocSignatureSpan">mssql.</span>Request (batch, callback)](#apidoc.element.mssql.Request)
- description and source-code
```javascript
class Request extends base.Request {
<span class="apidocCodeCommentSpan">  /*
  Execute specified sql batch.
  */
</span>
  _batch (batch, callback) {
    this._isBatch = true
    this._query(batch, callback)
  }

  /*
  Bulk load.
  */

  _bulk (table, callback) {
    super._bulk(table, err => {
      if (err) return callback(err)

      table._makeBulk()

      if (!table.name) {
        return callback(new base.RequestError('Table name must be specified for bulk insert.', 'ENAME'))
      }

      if (table.name.charAt(0) === '@') {
        return callback(new base.RequestError("You can't use table variables for bulk insert.", 'ENAME'))
      }

      const errors = []
      const errorHandlers = {}
      let hasReturned = false

      const handleError = (doReturn, connection, info) => {
        let err = new Error(info.message)
        err.info = info
        err = new base.RequestError(err, 'EREQUEST')

        if (this.stream) {
          this.emit('error', err)
        } else {
          if (doReturn && !hasReturned) {
            if (connection) {
              for (let event in errorHandlers) {
                connection.removeListener(event, errorHandlers[event])
              }

              this.parent.release(connection)
            }

            hasReturned = true
            callback(err)
          }
        }

        // we must collect errors even in stream mode
        errors.push(err)
      }

      const handleInfo = msg => {
        this.emit('info', {
          message: msg.message,
          number: msg.number,
          state: msg.state,
          class: msg.class,
          lineNumber: msg.lineNumber,
          serverName: msg.serverName,
          procName: msg.procName
        })
      }

      this.parent.acquire(this, (err, connection) => {
        if (err) return callback(err)

        if (this.canceled) {
          debug('req: canceled')
          this.parent.release(connection)
          return callback(new base.RequestError('Canceled.', 'ECANCEL'))
        }

        this._cancel = () => {
          debug('req: cancel')
          connection.cancel()
        }

        // attach handler to handle multiple error messages
        connection.on('infoMessage', errorHandlers.infoMessage = handleInfo)
        connection.on('errorMessage', errorHandlers.errorMessage = handleError.bind(null, false, connection))
        connection.on('error', errorHandlers.error = handleError.bind(null, true, connection))

        const done = (err, rowCount) => {
          // to make sure we handle no-sql errors as well
          if (err && (!errors.length || (errors.length && err.message !== errors[errors.length - 1].message))) {
            err = new base.RequestError(err, 'EREQUEST')
            if (this.stream) this.emit('error', err)
            errors.push(err)
          }

          this._cancel = null

          let error
          if (errors.length && !this.stream) {
            error = errors.pop()
            error.precedingErrors = errors
          }

          if (!hasReturned) {
            for (let event in errorHandlers) {
              connection.removeListener(event, errorHandlers[event])
            }

            this.parent.release(connection)
            hasReturned = true

            if (this.stream) {
              callback(null, rowCount)
            } else {
              callback(error, rowCount)
            }
          }
        }

        const bulk = connection.newBulkLoad(table.path, done)

        for (let col of table.columns) {
          bulk.addColumn(col.name, getTediousType(col.type), {nullable: col.nullable, length: col.length, scale: col.scale, precision
: col.precision})
        }

        for (let row of table.rows) {
          bulk.addRow(row)
        }

        if (table.create) {
          const objectid = table.temporary ? 'tempdb..[${table.name}]' : table.path
          const req = new tds.Request('if object_id('${objectid.replace(/'/g, '\'\'')}') is null ${table.declare()}', err => {
            if (err) return done(err)

            connection.execBulkLoad(bulk)
          })

          connection.execSqlBa ...
```
- example usage
```shell
...
const sql = require('mssql')

sql.connect(config, err => {
// ... error checks

// Query

new sql.Request().query('select 1 as number', (err, result) => {
    // ... error checks

    console.dir(result)
})

// Stored Procedure
...
```

#### <a name="apidoc.element.mssql.RequestError"></a>[function <span class="apidocSignatureSpan">mssql.</span>RequestError (message, code)](#apidoc.element.mssql.RequestError)
- description and source-code
```javascript
class RequestError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new RequestError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      if (message.info) {
        this.number = message.info.number || message.code // err.code is returned by msnodesql driver
        this.lineNumber = message.info.lineNumber
        this.state = message.info.state || message.sqlstate // err.sqlstate is returned by msnodesql driver
        this.class = message.info.class
        this.serverName = message.info.serverName
        this.procName = message.info.procName
      } else {
        this.number = message.code // err.code is returned by msnodesql driver
        this.state = message.sqlstate // err.sqlstate is returned by msnodesql driver
      }

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'RequestError'
    if ((/^\[Microsoft\]\[SQL Server Native Client 11\.0\](?:\[SQL Server\])?([\s\S]*)$/).exec(this.message)) {
      this.message = RegExp.$1
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLDATETIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLDATETIME ()](#apidoc.element.mssql.SMALLDATETIME)
- description and source-code
```javascript
SmallDateTime() {
  return {type: TYPES.SmallDateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLINT"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLINT ()](#apidoc.element.mssql.SMALLINT)
- description and source-code
```javascript
SmallInt() {
  return {type: TYPES.SmallInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SMALLMONEY"></a>[function <span class="apidocSignatureSpan">mssql.</span>SMALLMONEY ()](#apidoc.element.mssql.SMALLMONEY)
- description and source-code
```javascript
SmallMoney() {
  return {type: TYPES.SmallMoney}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime)
- description and source-code
```javascript
SmallDateTime() {
  return {type: TYPES.SmallDateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt)
- description and source-code
```javascript
SmallInt() {
  return {type: TYPES.SmallInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney)
- description and source-code
```javascript
SmallMoney() {
  return {type: TYPES.SmallMoney}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TEXT"></a>[function <span class="apidocSignatureSpan">mssql.</span>TEXT ()](#apidoc.element.mssql.TEXT)
- description and source-code
```javascript
Text() {
  return {type: TYPES.Text}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TIME"></a>[function <span class="apidocSignatureSpan">mssql.</span>TIME (scale)](#apidoc.element.mssql.TIME)
- description and source-code
```javascript
Time(scale) {
  return {type: TYPES.Time, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TINYINT"></a>[function <span class="apidocSignatureSpan">mssql.</span>TINYINT ()](#apidoc.element.mssql.TINYINT)
- description and source-code
```javascript
TinyInt() {
  return {type: TYPES.TinyInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TVP"></a>[function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP)
- description and source-code
```javascript
TVP(tvpType) {
  return {type: TYPES.TVP, tvpType}
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
  if (name) {
    const parsed = Table.parseName(name)
    this.name = parsed.name
    this.schema = parsed.schema
    this.database = parsed.database
    this.path = (this.database ? '[${this.database}].' : '') + (this.schema ? '[${this.schema}].' : '') + '[${this.name}]'
    this.temporary = this.name.charAt(0) === '#'
  }

  this.columns = []
  this.rows = []

  Object.defineProperty(this.columns, 'add', {
    value (name, column, options) {
      if (column == null) {
        throw new Error('Column data type is not defined.')
      }
      if (column instanceof Function) {
        column = column()
      }

      options = options || {}
      column.name = name
      column.nullable = options.nullable
      column.primary = options.primary

      return this.push(column)
    }
  }
  )

  Object.defineProperty(this.rows, 'add', {
    value () {
      return this.push(Array.prototype.slice.call(arguments))
    }
  }
  )
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
const table = new sql.Table('table_name') // or temporary table, e.g. #temptable
table.create = true
table.columns.add('a', sql.Int, {nullable: true, primary: true})
table.columns.add('b', sql.VarChar(50), {nullable: false})
table.rows.add(777, 'test')

const request = new sql.Request()
request.bulk(table, (err, result) => {
...
```

#### <a name="apidoc.element.mssql.Text"></a>[function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text)
- description and source-code
```javascript
Text() {
  return {type: TYPES.Text}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Time"></a>[function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time)
- description and source-code
```javascript
Time(scale) {
  return {type: TYPES.Time, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt)
- description and source-code
```javascript
TinyInt() {
  return {type: TYPES.TinyInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Transaction"></a>[function <span class="apidocSignatureSpan">mssql.</span>Transaction (parent)](#apidoc.element.mssql.Transaction)
- description and source-code
```javascript
class Transaction extends base.Transaction {
  constructor (parent) {
    super(parent)

    this._abort = () => {
      if (!this._rollbackRequested) {
        // transaction interrupted because of XACT_ABORT

        const pc = this._acquiredConnection

        // defer releasing so connection can switch from SentClientRequest to LoggedIn state
        setImmediate(this.parent.release.bind(this.parent), pc)

        this._acquiredConnection.removeListener('rollbackTransaction', this._abort)
        this._acquiredConnection = null
        this._aborted = true

        this.emit('rollback', true)
      }
    }
  }

  _begin (isolationLevel, callback) {
    super._begin(isolationLevel, err => {
      if (err) return callback(err)

      debug('tran: begin')

      this.parent.acquire(this, (err, connection) => {
        if (err) return callback(err)

        this._acquiredConnection = connection
        this._acquiredConnection.on('rollbackTransaction', this._abort)

        connection.beginTransaction(err => {
          if (err) err = new base.TransactionError(err)

          debug('tran: begin ok')

          callback(err)
        }, this.name, this.isolationLevel)
      })
    })
  }

  _commit (callback) {
    super._commit(err => {
      if (err) return callback(err)

      debug('tran: commit')

      this._acquiredConnection.commitTransaction(err => {
        if (err) err = new base.TransactionError(err)

        this._acquiredConnection.removeListener('rollbackTransaction', this._abort)
        this.parent.release(this._acquiredConnection)
        this._acquiredConnection = null

        if (!err) debug('tran: commit ok')

        callback(err)
      })
    })
  }

  _rollback (callback) {
    super._rollback(err => {
      if (err) return callback(err)

      debug('tran: rollback')

      this._acquiredConnection.rollbackTransaction(err => {
        if (err) err = new base.TransactionError(err)

        this._acquiredConnection.removeListener('rollbackTransaction', this._abort)
        this.parent.release(this._acquiredConnection)
        this._acquiredConnection = null

        if (!err) debug('tran: rollback ok')

        callback(err)
      })
    })
  }
}
```
- example usage
```shell
...
'''

## Transaction

**IMPORTANT:** always use 'Transaction' class to create transactions - it ensures that all your requests are executed on one connection
. Once you call 'begin', a single connection is acquired from the connection pool and all subsequent requests (initialized with
the 'Transaction' object) are executed exclusively on this connection. After you call 'commit' or 'rollback', connection is then
 released back to the connection pool.

'''javascript
const transaction = new sql.Transaction(/* [pool] */)
'''

If you omit connection argument, global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.TransactionError"></a>[function <span class="apidocSignatureSpan">mssql.</span>TransactionError (message, code)](#apidoc.element.mssql.TransactionError)
- description and source-code
```javascript
class TransactionError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new TransactionError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'TransactionError'
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UDT"></a>[function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT)
- description and source-code
```javascript
UDT() {
  return {type: TYPES.UDT}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UNIQUEIDENTIFIER"></a>[function <span class="apidocSignatureSpan">mssql.</span>UNIQUEIDENTIFIER ()](#apidoc.element.mssql.UNIQUEIDENTIFIER)
- description and source-code
```javascript
UniqueIdentifier() {
  return {type: TYPES.UniqueIdentifier}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier() {
  return {type: TYPES.UniqueIdentifier}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARBINARY"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARBINARY (length)](#apidoc.element.mssql.VARBINARY)
- description and source-code
```javascript
VarBinary(length) {
  return {type: TYPES.VarBinary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARCHAR"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARCHAR (length)](#apidoc.element.mssql.VARCHAR)
- description and source-code
```javascript
VarChar(length) {
  return {type: TYPES.VarChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VARIANT"></a>[function <span class="apidocSignatureSpan">mssql.</span>VARIANT ()](#apidoc.element.mssql.VARIANT)
- description and source-code
```javascript
Variant() {
  return {type: TYPES.Variant}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary)
- description and source-code
```javascript
VarBinary(length) {
  return {type: TYPES.VarBinary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar)
- description and source-code
```javascript
VarChar(length) {
  return {type: TYPES.VarChar, length}
}
```
- example usage
```shell
...

        console.dir(result1)

        // Stored procedure

        let result2 = await pool.request()
            .input('input_parameter', sql.Int, value)
            .output('output_parameter', sql.VarChar(50))
            .execute('procedure_name')

        console.dir(result2)
    } catch (err) {
        // ... error checks
    }
})()
...
```

#### <a name="apidoc.element.mssql.Variant"></a>[function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant)
- description and source-code
```javascript
Variant() {
  return {type: TYPES.Variant}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.XML"></a>[function <span class="apidocSignatureSpan">mssql.</span>XML ()](#apidoc.element.mssql.XML)
- description and source-code
```javascript
Xml() {
  return {type: TYPES.Xml}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Xml"></a>[function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml)
- description and source-code
```javascript
Xml() {
  return {type: TYPES.Xml}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.batch"></a>[function <span class="apidocSignatureSpan">mssql.</span>batch ()](#apidoc.element.mssql.batch)
- description and source-code
```javascript
function batch() {
  const values = Array.prototype.slice.call(arguments)
  const strings = values.shift()

  return new driver.Request()._template('batch', strings, values)
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
const request = new sql.Request()
request.batch('create procedure #temporary as select * from table', (err, result) => {
    // ... error checks
})
'''

__Errors__
- ETIMEOUT ('RequestError') - Request timeout.
- EREQUEST ('RequestError') - *Message from SQL Server*
...
```

#### <a name="apidoc.element.mssql.close"></a>[function <span class="apidocSignatureSpan">mssql.</span>close (callback)](#apidoc.element.mssql.close)
- description and source-code
```javascript
function close(callback) {
  if (globalConnection) {
    // remove event handlers from the global connection
    for (let event in globalConnectionHandlers) {
      for (let i = 0, l = globalConnectionHandlers[event].length; i < l; i++) {
        globalConnection.removeListener(event, globalConnectionHandlers[event][i])
      }
    }

    // attach error handler to prevent process crash in case of error
    globalConnection.on('error', err => {
      if (globalConnectionHandlers['error']) {
        for (let i = 0, l = globalConnectionHandlers['error'].length; i < l; i++) {
          globalConnectionHandlers['error'][i].call(globalConnection, err)
        }
      }
    })

    const gc = globalConnection
    globalConnection = null
    return gc.close(callback)
  }

  if (typeof callback === 'function') {
    setImmediate(callback)
    return null
  }

  return new PromiseLibrary((resolve, reject) => {
    resolve(globalConnection)
  })
}
```
- example usage
```shell
...
### close()

Close all active connections in the pool.

__Example__

'''javascript
pool.close()
'''

## Request

'''javascript
const request = new sql.Request(/* [pool or transaction] */)
'''
...
```

#### <a name="apidoc.element.mssql.connect"></a>[function <span class="apidocSignatureSpan">mssql.</span>connect (config, callback)](#apidoc.element.mssql.connect)
- description and source-code
```javascript
function connect(config, callback) {
  if (globalConnection) throw new Error('Global connection already exists. Call sql.close() first.')
  globalConnection = new driver.ConnectionPool(config)

  for (let event in globalConnectionHandlers) {
    for (let i = 0, l = globalConnectionHandlers[event].length; i < l; i++) {
      globalConnection.on(event, globalConnectionHandlers[event][i])
    }
  }

  return globalConnection.connect(callback)
}
```
- example usage
```shell
...
## Quick Example

'''javascript
const sql = require('mssql')

async () => {
    try {
        const pool = await sql.connect('mssql://username:password@localhost/database')
        const result = await sql.query'select * from mytable where id = ${value}'
        console.dir(result)
    } catch (err) {
        // ... error checks
    }
}
'''
...
```

#### <a name="apidoc.element.mssql.off"></a>[function <span class="apidocSignatureSpan">mssql.</span>off (event, handler)](#apidoc.element.mssql.off)
- description and source-code
```javascript
function removeListener(event, handler) {
  if (!globalConnectionHandlers[event]) return globalConnection
  const index = globalConnectionHandlers[event].indexOf(handler)
  if (index === -1) return globalConnection
  globalConnectionHandlers[event].splice(index, 1)
  if (globalConnectionHandlers[event].length === 0) globalConnectionHandlers[event] = undefined

  if (globalConnection) globalConnection.removeListener(event, handler)
  return globalConnection
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.on"></a>[function <span class="apidocSignatureSpan">mssql.</span>on (event, handler)](#apidoc.element.mssql.on)
- description and source-code
```javascript
function on(event, handler) {
  if (!globalConnectionHandlers[event]) globalConnectionHandlers[event] = []
  globalConnectionHandlers[event].push(handler)

  if (globalConnection) globalConnection.on(event, handler)
  return globalConnection
}
```
- example usage
```shell
...

        console.dir(result2)
    } catch (err) {
        // ... error checks
    }
})()

sql.on('error', err => {
    // ... error handler
})
'''

### Promises

'''javascript
...
```

#### <a name="apidoc.element.mssql.query"></a>[function <span class="apidocSignatureSpan">mssql.</span>query ()](#apidoc.element.mssql.query)
- description and source-code
```javascript
function query() {
  const values = Array.prototype.slice.call(arguments)
  const strings = values.shift()

  return new driver.Request()._template('query', strings, values)
}
```
- example usage
```shell
...
const sql = require('mssql')

(async function () {
try {
    let pool = await sql.connect(config)
    let result1 = await pool.request()
        .input('input_parameter', sql.Int, value)
        .query('select * from mytable where id = @input_parameter')

    console.dir(result1)

    // Stored procedure

    let result2 = await pool.request()
        .input('input_parameter', sql.Int, value)
...
```

#### <a name="apidoc.element.mssql.removeListener"></a>[function <span class="apidocSignatureSpan">mssql.</span>removeListener (event, handler)](#apidoc.element.mssql.removeListener)
- description and source-code
```javascript
function removeListener(event, handler) {
  if (!globalConnectionHandlers[event]) return globalConnection
  const index = globalConnectionHandlers[event].indexOf(handler)
  if (index === -1) return globalConnection
  globalConnectionHandlers[event].splice(index, 1)
  if (globalConnectionHandlers[event].length === 0) globalConnectionHandlers[event] = undefined

  if (globalConnection) globalConnection.removeListener(event, handler)
  return globalConnection
}
```
- example usage
```shell
...
 */

module.exports.exports.close = function close (callback) {
  if (globalConnection) {
// remove event handlers from the global connection
for (let event in globalConnectionHandlers) {
  for (let i = 0, l = globalConnectionHandlers[event].length; i < l; i++) {
    globalConnection.removeListener(event, globalConnectionHandlers[event][i])
  }
}

// attach error handler to prevent process crash in case of error
globalConnection.on('error', err => {
  if (globalConnectionHandlers['error']) {
    for (let i = 0, l = globalConnectionHandlers['error'].length; i < l; i++) {
...
```



# <a name="apidoc.module.mssql.BigInt"></a>[module mssql.BigInt](#apidoc.module.mssql.BigInt)

#### <a name="apidoc.element.mssql.BigInt.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>BigInt ()](#apidoc.element.mssql.BigInt.BigInt)
- description and source-code
```javascript
BigInt() {
  return {type: TYPES.BigInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.BigInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.BigInt.</span>inspect ()](#apidoc.element.mssql.BigInt.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Binary"></a>[module mssql.Binary](#apidoc.module.mssql.Binary)

#### <a name="apidoc.element.mssql.Binary.Binary"></a>[function <span class="apidocSignatureSpan">mssql.</span>Binary (length)](#apidoc.element.mssql.Binary.Binary)
- description and source-code
```javascript
Binary(length) {
  return {type: TYPES.Binary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Binary.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Binary.</span>inspect ()](#apidoc.element.mssql.Binary.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Bit"></a>[module mssql.Bit](#apidoc.module.mssql.Bit)

#### <a name="apidoc.element.mssql.Bit.Bit"></a>[function <span class="apidocSignatureSpan">mssql.</span>Bit ()](#apidoc.element.mssql.Bit.Bit)
- description and source-code
```javascript
Bit() {
  return {type: TYPES.Bit}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Bit.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Bit.</span>inspect ()](#apidoc.element.mssql.Bit.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Char"></a>[module mssql.Char](#apidoc.module.mssql.Char)

#### <a name="apidoc.element.mssql.Char.Char"></a>[function <span class="apidocSignatureSpan">mssql.</span>Char (length)](#apidoc.element.mssql.Char.Char)
- description and source-code
```javascript
Char(length) {
  return {type: TYPES.Char, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Char.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Char.</span>inspect ()](#apidoc.element.mssql.Char.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Date"></a>[module mssql.Date](#apidoc.module.mssql.Date)

#### <a name="apidoc.element.mssql.Date.Date"></a>[function <span class="apidocSignatureSpan">mssql.</span>Date ()](#apidoc.element.mssql.Date.Date)
- description and source-code
```javascript
Date() {
  return {type: TYPES.Date}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Date.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Date.</span>inspect ()](#apidoc.element.mssql.Date.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.DateTime"></a>[module mssql.DateTime](#apidoc.module.mssql.DateTime)

#### <a name="apidoc.element.mssql.DateTime.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime ()](#apidoc.element.mssql.DateTime.DateTime)
- description and source-code
```javascript
DateTime() {
  return {type: TYPES.DateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTime.inspect"></a>[function <span class="apidocSignatureSpan">mssql.DateTime.</span>inspect ()](#apidoc.element.mssql.DateTime.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.DateTime2"></a>[module mssql.DateTime2](#apidoc.module.mssql.DateTime2)

#### <a name="apidoc.element.mssql.DateTime2.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTime2 (scale)](#apidoc.element.mssql.DateTime2.DateTime2)
- description and source-code
```javascript
DateTime2(scale) {
  return {type: TYPES.DateTime2, scale}
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
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
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.DateTimeOffset"></a>[module mssql.DateTimeOffset](#apidoc.module.mssql.DateTimeOffset)

#### <a name="apidoc.element.mssql.DateTimeOffset.DateTimeOffset"></a>[function <span class="apidocSignatureSpan">mssql.</span>DateTimeOffset (scale)](#apidoc.element.mssql.DateTimeOffset.DateTimeOffset)
- description and source-code
```javascript
DateTimeOffset(scale) {
  return {type: TYPES.DateTimeOffset, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.DateTimeOffset.inspect"></a>[function <span class="apidocSignatureSpan">mssql.DateTimeOffset.</span>inspect ()](#apidoc.element.mssql.DateTimeOffset.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Decimal"></a>[module mssql.Decimal](#apidoc.module.mssql.Decimal)

#### <a name="apidoc.element.mssql.Decimal.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.</span>Decimal (precision, scale)](#apidoc.element.mssql.Decimal.Decimal)
- description and source-code
```javascript
Decimal(precision, scale) {
  return {type: TYPES.Decimal, precision, scale}
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc")               // varchar(3)
request.input("name", sql.VarChar(50), "abc")           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc")      // varchar(MAX)
request.output("name", sql.VarChar)                     // varchar(8000)
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.Decimal.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Decimal.</span>inspect ()](#apidoc.element.mssql.Decimal.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Float"></a>[module mssql.Float](#apidoc.module.mssql.Float)

#### <a name="apidoc.element.mssql.Float.Float"></a>[function <span class="apidocSignatureSpan">mssql.</span>Float ()](#apidoc.element.mssql.Float.Float)
- description and source-code
```javascript
Float() {
  return {type: TYPES.Float}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Float.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Float.</span>inspect ()](#apidoc.element.mssql.Float.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Geography"></a>[module mssql.Geography](#apidoc.module.mssql.Geography)

#### <a name="apidoc.element.mssql.Geography.Geography"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geography ()](#apidoc.element.mssql.Geography.Geography)
- description and source-code
```javascript
Geography() {
  return {type: TYPES.Geography}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geography.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Geography.</span>inspect ()](#apidoc.element.mssql.Geography.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Geometry"></a>[module mssql.Geometry](#apidoc.module.mssql.Geometry)

#### <a name="apidoc.element.mssql.Geometry.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.</span>Geometry ()](#apidoc.element.mssql.Geometry.Geometry)
- description and source-code
```javascript
Geometry() {
  return {type: TYPES.Geometry}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Geometry.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Geometry.</span>inspect ()](#apidoc.element.mssql.Geometry.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Image"></a>[module mssql.Image](#apidoc.module.mssql.Image)

#### <a name="apidoc.element.mssql.Image.Image"></a>[function <span class="apidocSignatureSpan">mssql.</span>Image ()](#apidoc.element.mssql.Image.Image)
- description and source-code
```javascript
Image() {
  return {type: TYPES.Image}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Image.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Image.</span>inspect ()](#apidoc.element.mssql.Image.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Int"></a>[module mssql.Int](#apidoc.module.mssql.Int)

#### <a name="apidoc.element.mssql.Int.Int"></a>[function <span class="apidocSignatureSpan">mssql.</span>Int ()](#apidoc.element.mssql.Int.Int)
- description and source-code
```javascript
Int() {
  return {type: TYPES.Int}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Int.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Int.</span>inspect ()](#apidoc.element.mssql.Int.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Money"></a>[module mssql.Money](#apidoc.module.mssql.Money)

#### <a name="apidoc.element.mssql.Money.Money"></a>[function <span class="apidocSignatureSpan">mssql.</span>Money ()](#apidoc.element.mssql.Money.Money)
- description and source-code
```javascript
Money() {
  return {type: TYPES.Money}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Money.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Money.</span>inspect ()](#apidoc.element.mssql.Money.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.NChar"></a>[module mssql.NChar](#apidoc.module.mssql.NChar)

#### <a name="apidoc.element.mssql.NChar.NChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NChar (length)](#apidoc.element.mssql.NChar.NChar)
- description and source-code
```javascript
NChar(length) {
  return {type: TYPES.NChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NChar.</span>inspect ()](#apidoc.element.mssql.NChar.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.NText"></a>[module mssql.NText](#apidoc.module.mssql.NText)

#### <a name="apidoc.element.mssql.NText.NText"></a>[function <span class="apidocSignatureSpan">mssql.</span>NText ()](#apidoc.element.mssql.NText.NText)
- description and source-code
```javascript
NText() {
  return {type: TYPES.NText}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NText.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NText.</span>inspect ()](#apidoc.element.mssql.NText.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.NVarChar"></a>[module mssql.NVarChar](#apidoc.module.mssql.NVarChar)

#### <a name="apidoc.element.mssql.NVarChar.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>NVarChar (length)](#apidoc.element.mssql.NVarChar.NVarChar)
- description and source-code
```javascript
NVarChar(length) {
  return {type: TYPES.NVarChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.NVarChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.NVarChar.</span>inspect ()](#apidoc.element.mssql.NVarChar.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Numeric"></a>[module mssql.Numeric](#apidoc.module.mssql.Numeric)

#### <a name="apidoc.element.mssql.Numeric.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.</span>Numeric (precision, scale)](#apidoc.element.mssql.Numeric.Numeric)
- description and source-code
```javascript
Numeric(precision, scale) {
  return {type: TYPES.Numeric, precision, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Numeric.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Numeric.</span>inspect ()](#apidoc.element.mssql.Numeric.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Real"></a>[module mssql.Real](#apidoc.module.mssql.Real)

#### <a name="apidoc.element.mssql.Real.Real"></a>[function <span class="apidocSignatureSpan">mssql.</span>Real ()](#apidoc.element.mssql.Real.Real)
- description and source-code
```javascript
Real() {
  return {type: TYPES.Real}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Real.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Real.</span>inspect ()](#apidoc.element.mssql.Real.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.SmallDateTime"></a>[module mssql.SmallDateTime](#apidoc.module.mssql.SmallDateTime)

#### <a name="apidoc.element.mssql.SmallDateTime.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallDateTime ()](#apidoc.element.mssql.SmallDateTime.SmallDateTime)
- description and source-code
```javascript
SmallDateTime() {
  return {type: TYPES.SmallDateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallDateTime.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallDateTime.</span>inspect ()](#apidoc.element.mssql.SmallDateTime.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.SmallInt"></a>[module mssql.SmallInt](#apidoc.module.mssql.SmallInt)

#### <a name="apidoc.element.mssql.SmallInt.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallInt ()](#apidoc.element.mssql.SmallInt.SmallInt)
- description and source-code
```javascript
SmallInt() {
  return {type: TYPES.SmallInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallInt.</span>inspect ()](#apidoc.element.mssql.SmallInt.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.SmallMoney"></a>[module mssql.SmallMoney](#apidoc.module.mssql.SmallMoney)

#### <a name="apidoc.element.mssql.SmallMoney.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.</span>SmallMoney ()](#apidoc.element.mssql.SmallMoney.SmallMoney)
- description and source-code
```javascript
SmallMoney() {
  return {type: TYPES.SmallMoney}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.SmallMoney.inspect"></a>[function <span class="apidocSignatureSpan">mssql.SmallMoney.</span>inspect ()](#apidoc.element.mssql.SmallMoney.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.TVP"></a>[module mssql.TVP](#apidoc.module.mssql.TVP)

#### <a name="apidoc.element.mssql.TVP.TVP"></a>[function <span class="apidocSignatureSpan">mssql.</span>TVP (tvpType)](#apidoc.element.mssql.TVP.TVP)
- description and source-code
```javascript
TVP(tvpType) {
  return {type: TYPES.TVP, tvpType}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TVP.inspect"></a>[function <span class="apidocSignatureSpan">mssql.TVP.</span>inspect ()](#apidoc.element.mssql.TVP.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.TYPES"></a>[module mssql.TYPES](#apidoc.module.mssql.TYPES)

#### <a name="apidoc.element.mssql.TYPES.BigInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>BigInt ()](#apidoc.element.mssql.TYPES.BigInt)
- description and source-code
```javascript
BigInt() {
  return {type: TYPES.BigInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Binary"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Binary (length)](#apidoc.element.mssql.TYPES.Binary)
- description and source-code
```javascript
Binary(length) {
  return {type: TYPES.Binary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Bit"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Bit ()](#apidoc.element.mssql.TYPES.Bit)
- description and source-code
```javascript
Bit() {
  return {type: TYPES.Bit}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Char"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Char (length)](#apidoc.element.mssql.TYPES.Char)
- description and source-code
```javascript
Char(length) {
  return {type: TYPES.Char, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Date"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Date ()](#apidoc.element.mssql.TYPES.Date)
- description and source-code
```javascript
Date() {
  return {type: TYPES.Date}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.DateTime"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime ()](#apidoc.element.mssql.TYPES.DateTime)
- description and source-code
```javascript
DateTime() {
  return {type: TYPES.DateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.DateTime2"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>DateTime2 (scale)](#apidoc.element.mssql.TYPES.DateTime2)
- description and source-code
```javascript
DateTime2(scale) {
  return {type: TYPES.DateTime2, scale}
}
```
- example usage
```shell
...
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
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
DateTimeOffset(scale) {
  return {type: TYPES.DateTimeOffset, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Decimal"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Decimal (precision, scale)](#apidoc.element.mssql.TYPES.Decimal)
- description and source-code
```javascript
Decimal(precision, scale) {
  return {type: TYPES.Decimal, precision, scale}
}
```
- example usage
```shell
...
request.input("name", sql.VarChar, "abc")               // varchar(3)
request.input("name", sql.VarChar(50), "abc")           // varchar(50)
request.input("name", sql.VarChar(sql.MAX), "abc")      // varchar(MAX)
request.output("name", sql.VarChar)                     // varchar(8000)
request.output("name", sql.VarChar, "abc")              // varchar(3)

request.input("name", sql.Decimal, 155.33)              // decimal(18, 0)
request.input("name", sql.Decimal(10), 155.33)          // decimal(10, 0)
request.input("name", sql.Decimal(10, 2), 155.33)       // decimal(10, 2)

request.input("name", sql.DateTime2, new Date())        // datetime2(7)
request.input("name", sql.DateTime2(5), new Date())     // datetime2(5)
'''

List of supported data types:
...
```

#### <a name="apidoc.element.mssql.TYPES.Float"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Float ()](#apidoc.element.mssql.TYPES.Float)
- description and source-code
```javascript
Float() {
  return {type: TYPES.Float}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Geography"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geography ()](#apidoc.element.mssql.TYPES.Geography)
- description and source-code
```javascript
Geography() {
  return {type: TYPES.Geography}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Geometry"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Geometry ()](#apidoc.element.mssql.TYPES.Geometry)
- description and source-code
```javascript
Geometry() {
  return {type: TYPES.Geometry}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Image"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Image ()](#apidoc.element.mssql.TYPES.Image)
- description and source-code
```javascript
Image() {
  return {type: TYPES.Image}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Int"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Int ()](#apidoc.element.mssql.TYPES.Int)
- description and source-code
```javascript
Int() {
  return {type: TYPES.Int}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Money"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Money ()](#apidoc.element.mssql.TYPES.Money)
- description and source-code
```javascript
Money() {
  return {type: TYPES.Money}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NChar (length)](#apidoc.element.mssql.TYPES.NChar)
- description and source-code
```javascript
NChar(length) {
  return {type: TYPES.NChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NText"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NText ()](#apidoc.element.mssql.TYPES.NText)
- description and source-code
```javascript
NText() {
  return {type: TYPES.NText}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.NVarChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>NVarChar (length)](#apidoc.element.mssql.TYPES.NVarChar)
- description and source-code
```javascript
NVarChar(length) {
  return {type: TYPES.NVarChar, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Numeric"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Numeric (precision, scale)](#apidoc.element.mssql.TYPES.Numeric)
- description and source-code
```javascript
Numeric(precision, scale) {
  return {type: TYPES.Numeric, precision, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Real"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Real ()](#apidoc.element.mssql.TYPES.Real)
- description and source-code
```javascript
Real() {
  return {type: TYPES.Real}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallDateTime"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallDateTime ()](#apidoc.element.mssql.TYPES.SmallDateTime)
- description and source-code
```javascript
SmallDateTime() {
  return {type: TYPES.SmallDateTime}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallInt ()](#apidoc.element.mssql.TYPES.SmallInt)
- description and source-code
```javascript
SmallInt() {
  return {type: TYPES.SmallInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.SmallMoney"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>SmallMoney ()](#apidoc.element.mssql.TYPES.SmallMoney)
- description and source-code
```javascript
SmallMoney() {
  return {type: TYPES.SmallMoney}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.TVP"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>TVP (tvpType)](#apidoc.element.mssql.TYPES.TVP)
- description and source-code
```javascript
TVP(tvpType) {
  return {type: TYPES.TVP, tvpType}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Text"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Text ()](#apidoc.element.mssql.TYPES.Text)
- description and source-code
```javascript
Text() {
  return {type: TYPES.Text}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Time"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Time (scale)](#apidoc.element.mssql.TYPES.Time)
- description and source-code
```javascript
Time(scale) {
  return {type: TYPES.Time, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>TinyInt ()](#apidoc.element.mssql.TYPES.TinyInt)
- description and source-code
```javascript
TinyInt() {
  return {type: TYPES.TinyInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.UDT"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>UDT ()](#apidoc.element.mssql.TYPES.UDT)
- description and source-code
```javascript
UDT() {
  return {type: TYPES.UDT}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>UniqueIdentifier ()](#apidoc.element.mssql.TYPES.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier() {
  return {type: TYPES.UniqueIdentifier}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarBinary (length)](#apidoc.element.mssql.TYPES.VarBinary)
- description and source-code
```javascript
VarBinary(length) {
  return {type: TYPES.VarBinary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>VarChar (length)](#apidoc.element.mssql.TYPES.VarChar)
- description and source-code
```javascript
VarChar(length) {
  return {type: TYPES.VarChar, length}
}
```
- example usage
```shell
...

        console.dir(result1)

        // Stored procedure

        let result2 = await pool.request()
            .input('input_parameter', sql.Int, value)
            .output('output_parameter', sql.VarChar(50))
            .execute('procedure_name')

        console.dir(result2)
    } catch (err) {
        // ... error checks
    }
})()
...
```

#### <a name="apidoc.element.mssql.TYPES.Variant"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Variant ()](#apidoc.element.mssql.TYPES.Variant)
- description and source-code
```javascript
Variant() {
  return {type: TYPES.Variant}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TYPES.Xml"></a>[function <span class="apidocSignatureSpan">mssql.TYPES.</span>Xml ()](#apidoc.element.mssql.TYPES.Xml)
- description and source-code
```javascript
Xml() {
  return {type: TYPES.Xml}
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
  if (name) {
    const parsed = Table.parseName(name)
    this.name = parsed.name
    this.schema = parsed.schema
    this.database = parsed.database
    this.path = (this.database ? '[${this.database}].' : '') + (this.schema ? '[${this.schema}].' : '') + '[${this.name}]'
    this.temporary = this.name.charAt(0) === '#'
  }

  this.columns = []
  this.rows = []

  Object.defineProperty(this.columns, 'add', {
    value (name, column, options) {
      if (column == null) {
        throw new Error('Column data type is not defined.')
      }
      if (column instanceof Function) {
        column = column()
      }

      options = options || {}
      column.name = name
      column.nullable = options.nullable
      column.primary = options.primary

      return this.push(column)
    }
  }
  )

  Object.defineProperty(this.rows, 'add', {
    value () {
      return this.push(Array.prototype.slice.call(arguments))
    }
  }
  )
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
const table = new sql.Table('table_name') // or temporary table, e.g. #temptable
table.create = true
table.columns.add('a', sql.Int, {nullable: true, primary: true})
table.columns.add('b', sql.VarChar(50), {nullable: false})
table.rows.add(777, 'test')

const request = new sql.Request()
request.bulk(table, (err, result) => {
...
```

#### <a name="apidoc.element.mssql.Table.fromRecordset"></a>[function <span class="apidocSignatureSpan">mssql.Table.</span>fromRecordset (recordset, name)](#apidoc.element.mssql.Table.fromRecordset)
- description and source-code
```javascript
function fromRecordset(recordset, name) {
  const t = new this(name)

  for (const colName in recordset.columns) {
    if (Object.prototype.hasOwnProperty.call(recordset.columns, colName)) {
      const col = recordset.columns[colName]

      t.columns.add(colName, {
        type: col.type,
        length: col.length,
        scale: col.scale,
        precision: col.precision
      }, {
        nullable: col.nullable
      })
    }
  }

  if (t.columns.length === 1 && t.columns[0].name === JSON_COLUMN_ID) {
    for (let i = 0; i < recordset.length; i++) {
      t.rows.add(JSON.stringify(recordset[i]))
    }
  } else {
    for (let i = 0; i < recordset.length; i++) {
      t.rows.add.apply(t.rows, t.columns.map(col => recordset[i][col.name]))
    }
  }

  return t
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Table.parseName"></a>[function <span class="apidocSignatureSpan">mssql.Table.</span>parseName (name)](#apidoc.element.mssql.Table.parseName)
- description and source-code
```javascript
function parseName(name) {
  const length = name.length
  let cursor = -1
  let buffer = ''
  let escaped = false
  const path = []

  while (++cursor < length) {
    const char = name.charAt(cursor)
    if (char === '[') {
      if (escaped) {
        buffer += char
      } else {
        escaped = true
      }
    } else if (char === ']') {
      if (escaped) {
        escaped = false
      } else {
        throw new Error('Invalid table name.')
      }
    } else if (char === '.') {
      if (escaped) {
        buffer += char
      } else {
        path.push(buffer)
        buffer = ''
      }
    } else {
      buffer += char
    }
  }

  if (buffer) {
    path.push(buffer)
  }

  switch (path.length) {
    case 1:
      return {
        name: path[0],
        schema: null,
        database: null
      }

    case 2:
      return {
        name: path[1],
        schema: path[0],
        database: null
      }

    case 3:
      return {
        name: path[2],
        schema: path[1],
        database: path[0]
      }

    default:
      throw new Error('Invalid table name.')
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
function _makeBulk() {
  for (let i = 0; i < this.columns.length; i++) {
    const col = this.columns[i]
    switch (col.type) {
      case TYPES.Xml:
        col.type = TYPES.NVarChar(MAX).type
        break

      case TYPES.UDT:
      case TYPES.Geography:
      case TYPES.Geometry:
        col.type = TYPES.VarBinary(MAX).type
        break

      default:
        break
    }
  }

  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Table.prototype.declare"></a>[function <span class="apidocSignatureSpan">mssql.Table.prototype.</span>declare ()](#apidoc.element.mssql.Table.prototype.declare)
- description and source-code
```javascript
function declare() {
  const pkey = this.columns.filter(col => col.primary === true).map(col => col.name)
  const cols = this.columns.map(col => {
    const def = ['[${col.name}] ${declareType(col.type, col)}']

    if (col.nullable === true) {
      def.push('null')
    } else if (col.nullable === false) {
      def.push('not null')
    }

    if (col.primary === true && pkey.length === 1) {
      def.push('primary key')
    }

    return def.join(' ')
  })

  const constraint = pkey.length > 1 ? ', constraint PK_${this.temporary ? this.name.substr(1) : this.name} primary key (${pkey.
join(', ')})' : ''
  return 'create table ${this.path} (${cols.join(', ')}${constraint})'
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Text"></a>[module mssql.Text](#apidoc.module.mssql.Text)

#### <a name="apidoc.element.mssql.Text.Text"></a>[function <span class="apidocSignatureSpan">mssql.</span>Text ()](#apidoc.element.mssql.Text.Text)
- description and source-code
```javascript
Text() {
  return {type: TYPES.Text}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Text.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Text.</span>inspect ()](#apidoc.element.mssql.Text.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Time"></a>[module mssql.Time](#apidoc.module.mssql.Time)

#### <a name="apidoc.element.mssql.Time.Time"></a>[function <span class="apidocSignatureSpan">mssql.</span>Time (scale)](#apidoc.element.mssql.Time.Time)
- description and source-code
```javascript
Time(scale) {
  return {type: TYPES.Time, scale}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Time.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Time.</span>inspect ()](#apidoc.element.mssql.Time.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.TinyInt"></a>[module mssql.TinyInt](#apidoc.module.mssql.TinyInt)

#### <a name="apidoc.element.mssql.TinyInt.TinyInt"></a>[function <span class="apidocSignatureSpan">mssql.</span>TinyInt ()](#apidoc.element.mssql.TinyInt.TinyInt)
- description and source-code
```javascript
TinyInt() {
  return {type: TYPES.TinyInt}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.TinyInt.inspect"></a>[function <span class="apidocSignatureSpan">mssql.TinyInt.</span>inspect ()](#apidoc.element.mssql.TinyInt.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.UDT"></a>[module mssql.UDT](#apidoc.module.mssql.UDT)

#### <a name="apidoc.element.mssql.UDT.UDT"></a>[function <span class="apidocSignatureSpan">mssql.</span>UDT ()](#apidoc.element.mssql.UDT.UDT)
- description and source-code
```javascript
UDT() {
  return {type: TYPES.UDT}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UDT.inspect"></a>[function <span class="apidocSignatureSpan">mssql.UDT.</span>inspect ()](#apidoc.element.mssql.UDT.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.UniqueIdentifier"></a>[module mssql.UniqueIdentifier](#apidoc.module.mssql.UniqueIdentifier)

#### <a name="apidoc.element.mssql.UniqueIdentifier.UniqueIdentifier"></a>[function <span class="apidocSignatureSpan">mssql.</span>UniqueIdentifier ()](#apidoc.element.mssql.UniqueIdentifier.UniqueIdentifier)
- description and source-code
```javascript
UniqueIdentifier() {
  return {type: TYPES.UniqueIdentifier}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.UniqueIdentifier.inspect"></a>[function <span class="apidocSignatureSpan">mssql.UniqueIdentifier.</span>inspect ()](#apidoc.element.mssql.UniqueIdentifier.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.VarBinary"></a>[module mssql.VarBinary](#apidoc.module.mssql.VarBinary)

#### <a name="apidoc.element.mssql.VarBinary.VarBinary"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarBinary (length)](#apidoc.element.mssql.VarBinary.VarBinary)
- description and source-code
```javascript
VarBinary(length) {
  return {type: TYPES.VarBinary, length}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.VarBinary.inspect"></a>[function <span class="apidocSignatureSpan">mssql.VarBinary.</span>inspect ()](#apidoc.element.mssql.VarBinary.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.VarChar"></a>[module mssql.VarChar](#apidoc.module.mssql.VarChar)

#### <a name="apidoc.element.mssql.VarChar.VarChar"></a>[function <span class="apidocSignatureSpan">mssql.</span>VarChar (length)](#apidoc.element.mssql.VarChar.VarChar)
- description and source-code
```javascript
VarChar(length) {
  return {type: TYPES.VarChar, length}
}
```
- example usage
```shell
...

        console.dir(result1)

        // Stored procedure

        let result2 = await pool.request()
            .input('input_parameter', sql.Int, value)
            .output('output_parameter', sql.VarChar(50))
            .execute('procedure_name')

        console.dir(result2)
    } catch (err) {
        // ... error checks
    }
})()
...
```

#### <a name="apidoc.element.mssql.VarChar.inspect"></a>[function <span class="apidocSignatureSpan">mssql.VarChar.</span>inspect ()](#apidoc.element.mssql.VarChar.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Variant"></a>[module mssql.Variant](#apidoc.module.mssql.Variant)

#### <a name="apidoc.element.mssql.Variant.Variant"></a>[function <span class="apidocSignatureSpan">mssql.</span>Variant ()](#apidoc.element.mssql.Variant.Variant)
- description and source-code
```javascript
Variant() {
  return {type: TYPES.Variant}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Variant.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Variant.</span>inspect ()](#apidoc.element.mssql.Variant.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.Xml"></a>[module mssql.Xml](#apidoc.module.mssql.Xml)

#### <a name="apidoc.element.mssql.Xml.Xml"></a>[function <span class="apidocSignatureSpan">mssql.</span>Xml ()](#apidoc.element.mssql.Xml.Xml)
- description and source-code
```javascript
Xml() {
  return {type: TYPES.Xml}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.Xml.inspect"></a>[function <span class="apidocSignatureSpan">mssql.Xml.</span>inspect ()](#apidoc.element.mssql.Xml.inspect)
- description and source-code
```javascript
() => '[sql.${key}]'
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.base"></a>[module mssql.base](#apidoc.module.mssql.base)

#### <a name="apidoc.element.mssql.base.ConnectionError"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>ConnectionError (message, code)](#apidoc.element.mssql.base.ConnectionError)
- description and source-code
```javascript
class ConnectionError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new ConnectionError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'ConnectionError'
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.base.ConnectionPool"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>ConnectionPool (config, callback)](#apidoc.element.mssql.base.ConnectionPool)
- description and source-code
```javascript
class ConnectionPool extends EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Create new Connection.
   *
   * @param {Object|String} config Connection configuration object or connection string.
   * @param {basicCallback} [callback] A callback which is called after connection has established, or an error has occurred.
   */
</span>
  constructor (config, callback) {
    super()

    this.config = config
    this._connected = false
    this._connecting = false

    if (typeof this.config === 'string') {
      try {
        this.config = ConnectionString.resolve(this.config, driver.name)
      } catch (ex) {
        if (typeof callback === 'function') {
          return callback(ex)
        }
        throw ex
      }
    }

    // set defaults
    this.config.port = this.config.port || 1433
    this.config.options = this.config.options || {}
    this.config.stream = this.config.stream || false
    this.config.parseJSON = this.config.parseJSON || false

    if (/^(.*)\\(.*)$/.exec(this.config.server)) {
      this.config.server = RegExp.$1
      this.config.options.instanceName = RegExp.$2
    }

    if (typeof callback === 'function') {
      this.connect(callback)
    }
  }

  get connected () {
    return this._connected
  }

  get connecting () {
    return this._connecting
  }

  /**
   * Acquire connection from this connection pool.
   *
   * @param {ConnectionPool|Transaction|PreparedStatement} requester Requester.
   * @param {acquireCallback} [callback] A callback which is called after connection has been acquired, or an error has occurred
. If omited, method returns Promise.
   * @return {ConnectionPool|Promise}
   */

  acquire (requester, callback) {
    debug('conn: acquire')

    if (typeof callback === 'function') {
      this._acquire().then(connection => callback(null, connection)).catch(callback)
      return this
    }

    return this._acquire()
  }

  _acquire () {
    if (!this.pool) {
      return Promise.reject(new ConnectionError('Connection not yet open.', 'ENOTOPEN'))
    }

    return this.pool.acquire()
  }

  /**
   * Release connection back to the pool.
   *
   * @param {Connection} connection Previously acquired connection.
   * @return {ConnectionPool}
   */

  release (connection) {
    debug('conn: release')

    this.pool.release(connection)
    return this
  }

  /**
   * Creates a new connection pool with one active connection. This one initial connection serves as a probe to find out whether
 the configuration is valid.
   *
   * @param {basicCallback} [callback] A callback which is called after connection has established, or an error has occurred. If
 omited, method returns Promise.
   * @return {ConnectionPool|Promise}
   */

  connect (callback) {
    if (typeof callback === 'function') {
      this._connect(callback)
      return this
    }

    return new PromiseLibrary((resolve, reject) => {
      return this._connect(err => {
        if (err) return reject(err)
        resolve(this)
      })
    })
  }

  /**
   * @private
   * @param {basicCallback} callback
   */

  _connect (callback) {
    if (this._connected) {
      return callback(new ConnectionError('Database is already connected! Call close before connecting to different database.', '
EALREADYCONNECTED'))
    }

    if (this._connecting) {
      return callback(new ConnectionError('Already connecting to database! Call close before connecting to different database.', '
EALREADYCONNECTING'))
    }

    this._connecting = true

    // create one testing connection to check if everything is ok
    this._poolCreate().then((connection) => {
      this._poolDestroy(connection)
      if (!this._connecting) {
        // close was called before connection was established
        return // exit silently
      }

      // prepare pool
      this.pool = gp.createPool({
        create: this._poolCreate.bind(this),
        validate: this._poolValidate.bind(this),
        destroy: this._poolDestroy.bind(this)
      }, Object.assign({
        max: 10,
        min: 0,
        idleTimeoutMillis: 30000,
        testOnBorrow: true,
        autostart: false
      }, thi ...
```
- example usage
```shell
...
'''

## Connection Pools

'''javascript
const sql = require('mssql')

const pool1 = new sql.ConnectionPool(config, err => {
// ... error checks

// Query

pool1.request() // or: new sql.Request(pool1)
.query('select 1 as number', (err, result) => {
    // ... error checks
...
```

#### <a name="apidoc.element.mssql.base.PreparedStatement"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>PreparedStatement (parent)](#apidoc.element.mssql.base.PreparedStatement)
- description and source-code
```javascript
class PreparedStatement extends EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new Prepared Statement.
   *
   * @param {ConnectionPool|Transaction} [holder]
   */
</span>
  constructor (parent) {
    super()

    this.parent = parent || globalConnection
    this._handle = 0
    this.prepared = false
    this.parameters = {}
  }

  get connected () {
    return this.parent.connected
  }

  /**
   * Acquire connection from connection pool.
   *
   * @param {Request} request Request.
   * @param {ConnectionPool~acquireCallback} [callback] A callback which is called after connection has established, or an error
 has occurred. If omited, method returns Promise.
   * @return {PreparedStatement|Promise}
   */

  acquire (request, callback) {
    debug('ps: acquire')

    if (!this._acquiredConnection) {
      setImmediate(callback, new PreparedStatementError('Statement is not prepared. Call prepare() first.', 'ENOTPREPARED'))
      return this
    }

    if (this._activeRequest) {
      setImmediate(callback, new TransactionError("Can't acquire connection for the request. There is another request in progress
.", 'EREQINPROG'))
      return this
    }

    debug('ps: acquire ok')

    this._activeRequest = request
    setImmediate(callback, null, this._acquiredConnection)
    return this
  }

  /**
   * Release connection back to the pool.
   *
   * @param {Connection} connection Previously acquired connection.
   * @return {PreparedStatement}
   */

  release (connection) {
    debug('ps: release')

    if (connection === this._acquiredConnection) {
      this._activeRequest = null
      debug('ps: release ok')
    }

    return this
  }

  /**
   * Add an input parameter to the prepared statement.
   *
   * @param {String} name Name of the input parameter without @ char.
   * @param {*} type SQL data type of input parameter.
   * @return {PreparedStatement}
   */

  input (name, type) {
    if ((/(--| |\/\*|\*\/|')/).test(name)) {
      throw new PreparedStatementError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if (arguments.length < 2) {
      throw new PreparedStatementError('Invalid number of arguments. 2 arguments expected.', 'EARGS')
    }

    if (type instanceof Function) {
      type = type()
    }

    this.parameters[name] = {
      name,
      type: type.type,
      io: 1,
      length: type.length,
      scale: type.scale,
      precision: type.precision,
      tvpType: type.tvpType
    }

    return this
  }

  /**
   * Add an output parameter to the prepared statement.
   *
   * @param {String} name Name of the output parameter without @ char.
   * @param {*} type SQL data type of output parameter.
   * @return {PreparedStatement}
   */

  output (name, type) {
    if (/(--| |\/\*|\*\/|')/.test(name)) {
      throw new PreparedStatementError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if (arguments.length < 2) {
      throw new PreparedStatementError('Invalid number of arguments. 2 arguments expected.', 'EARGS')
    }

    if (type instanceof Function) type = type()

    this.parameters[name] = {
      name,
      type: type.type,
      io: 2,
      length: type.length,
      scale: type.scale,
      precision: type.precision
    }

    return this
  }

  /**
   * Prepare a statement.
   *
   * @param {String} statement SQL statement to prepare.
   * @param {basicCallback} [callback] A callback which is called after preparation has completed, or an error has occurred. If
omited, method returns Promise.
   * @return {PreparedStatement|Promise}
   */

  prepare (statement, callback) {
    if (typeof callback === 'function') {
      this._prepare(statement, callback)
      return this
    }

    return new PromiseLibrary((resolve, reject) => {
      this._prepare(statement, err => {
        if (err) return reject(err)
        resolve(this)
      })
    })
  }

  /**
   * @private
   * @param {String} statement
   * @param {basicCallback} callback
   */

  _prepare (statement, callback) {
    debug('ps: prepare')

    if (typeof statement === 'function') {
      callback = statement ...
```
- example usage
```shell
...
- EREQINPROG ('TransactionError') - Can't rollback transaction. There is a request in progress.

## Prepared Statement

**IMPORTANT:** always use 'PreparedStatement' class to create prepared statements - it ensures that all your executions of prepared
 statement are executed on one connection. Once you call 'prepare', a single connection is acquired from the connection pool and
 all subsequent executions are executed exclusively on this connection. After you call 'unprepare', the connection is then released
 back to the connection pool.

'''javascript
const ps = new sql.PreparedStatement(/* [pool] */)
'''

If you omit the connection argument, the global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.base.PreparedStatementError"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>PreparedStatementError (message, code)](#apidoc.element.mssql.base.PreparedStatementError)
- description and source-code
```javascript
class PreparedStatementError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new PreparedStatementError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'PreparedStatementError'
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.base.Request"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>Request (parent)](#apidoc.element.mssql.base.Request)
- description and source-code
```javascript
class Request extends EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Create new Request.
   *
   * @param {Connection|ConnectionPool|Transaction|PreparedStatement} parent If ommited, global connection is used instead.
   */
</span>
  constructor (parent) {
    super()

    this.canceled = false
    this.parent = parent || globalConnection
    this.parameters = {}
  }

  /**
   * Fetch request from tagged template string.
   *
   * @private
   * @param {String} method
   * @param {Array} strings
   * @param {Array} values
   * @return {Request}
   */

  _template (method, strings, values) {
    let command = [strings[0]]

    for (let index = 0; index < values.length; index++) {
      let value = values[index]
      this.input('param${index + 1}', value)
      command.push('@param${index + 1}', strings[index + 1])
    }

    return this[method](command.join(''))
  }

  /**
   * Add an input parameter to the request.
   *
   * @param {String} name Name of the input parameter without @ char.
   * @param {*} [type] SQL data type of input parameter. If you omit type, module automaticaly decide which SQL data type should
 be used based on JS data type.
   * @param {*} value Input parameter value. 'undefined' and 'NaN' values are automatically converted to 'null' values.
   * @return {Request}
   */

  input (name, type, value) {
    if ((/(--| |\/\*|\*\/|')/).test(name)) {
      throw new RequestError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if (arguments.length === 1) {
      throw new RequestError('Invalid number of arguments. At least 2 arguments expected.', 'EARGS')
    } else if (arguments.length === 2) {
      value = type
      type = getTypeByValue(value)
    }

    // support for custom data types
    if (value && typeof value.valueOf === 'function' && !(value instanceof Date)) value = value.valueOf()

    if (value === undefined) value = null // undefined to null
    if (typeof value === 'number' && isNaN(value)) value = null // NaN to null
    if (type instanceof Function) type = type()

    this.parameters[name] = {
      name,
      type: type.type,
      io: 1,
      value,
      length: type.length,
      scale: type.scale,
      precision: type.precision,
      tvpType: type.tvpType
    }

    return this
  }

  /**
   * Add an output parameter to the request.
   *
   * @param {String} name Name of the output parameter without @ char.
   * @param {*} type SQL data type of output parameter.
   * @param {*} [value] Output parameter value initial value. 'undefined' and 'NaN' values are automatically converted to 'null'
values. Optional.
   * @return {Request}
   */

  output (name, type, value) {
    if (!type) { type = TYPES.NVarChar }

    if ((/(--| |\/\*|\*\/|')/).test(name)) {
      throw new RequestError('SQL injection warning for param '${name}'', 'EINJECT')
    }

    if ((type === TYPES.Text) || (type === TYPES.NText) || (type === TYPES.Image)) {
      throw new RequestError('Deprecated types (Text, NText, Image) are not supported as OUTPUT parameters.', 'EDEPRECATED')
    }

    // support for custom data types
    if (value && typeof value.valueOf === 'function' && !(value instanceof Date)) value = value.valueOf()

    if (value === undefined) value = null // undefined to null
    if (typeof value === 'number' && isNaN(value)) value = null // NaN to null
    if (type instanceof Function) type = type()

    this.parameters[name] = {
      name,
      type: type.type,
      io: 2,
      value,
      length: type.length,
      scale: type.scale,
      precision: type.precision
    }

    return this
  }

  /**
   * Execute the SQL batch.
   *
   * @param {String} batch T-SQL batch to be executed.
   * @param {Request~requestCallback} [callback] A callback which is called after execution has completed, or an error has occurred
. If omited, method returns Promise.
   * @return {Request|Promise}
   */

  batch (batch, callback) {
    if (this.stream == null && this.connection) this.stream = this.connection.config.stream
    this.rowsAffected = 0

    if (typeof callback === 'function') {
      this._batch(batc ...
```
- example usage
```shell
...
const sql = require('mssql')

sql.connect(config, err => {
// ... error checks

// Query

new sql.Request().query('select 1 as number', (err, result) => {
    // ... error checks

    console.dir(result)
})

// Stored Procedure
...
```

#### <a name="apidoc.element.mssql.base.RequestError"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>RequestError (message, code)](#apidoc.element.mssql.base.RequestError)
- description and source-code
```javascript
class RequestError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new RequestError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      if (message.info) {
        this.number = message.info.number || message.code // err.code is returned by msnodesql driver
        this.lineNumber = message.info.lineNumber
        this.state = message.info.state || message.sqlstate // err.sqlstate is returned by msnodesql driver
        this.class = message.info.class
        this.serverName = message.info.serverName
        this.procName = message.info.procName
      } else {
        this.number = message.code // err.code is returned by msnodesql driver
        this.state = message.sqlstate // err.sqlstate is returned by msnodesql driver
      }

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'RequestError'
    if ((/^\[Microsoft\]\[SQL Server Native Client 11\.0\](?:\[SQL Server\])?([\s\S]*)$/).exec(this.message)) {
      this.message = RegExp.$1
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.base.Transaction"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>Transaction (parent)](#apidoc.element.mssql.base.Transaction)
- description and source-code
```javascript
class Transaction extends EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Create new Transaction.
   *
   * @param {Connection} [holder] If ommited, global connection is used instead.
   */
</span>
  constructor (parent) {
    super()

    this.parent = parent || globalConnection
    this.isolationLevel = ISOLATION_LEVEL.READ_COMMITTED
    this.name = ''
  }

  get connected () {
    return this.parent.connected
  }

  /**
   * Acquire connection from connection pool.
   *
   * @param {Request} request Request.
   * @param {ConnectionPool~acquireCallback} [callback] A callback which is called after connection has established, or an error
 has occurred. If omited, method returns Promise.
   * @return {Transaction|Promise}
   */

  acquire (request, callback) {
    debug('tran: acquire')

    if (!this._acquiredConnection) {
      setImmediate(callback, new TransactionError('Transaction has not begun. Call begin() first.', 'ENOTBEGUN'))
      return this
    }

    if (this._activeRequest) {
      setImmediate(callback, new TransactionError("Can't acquire connection for the request. There is another request in progress
.", 'EREQINPROG'))
      return this
    }

    debug('tran: acquire ok')

    this._activeRequest = request
    setImmediate(callback, null, this._acquiredConnection)
    return this
  }

  /**
   * Release connection back to the pool.
   *
   * @param {Connection} connection Previously acquired connection.
   * @return {Transaction}
   */

  release (connection) {
    debug('tran: release')

    if (connection === this._acquiredConnection) {
      this._activeRequest = null
      debug('tran: release ok')
    }

    return this
  }

  /**
   * Begin a transaction.
   *
   * @param {Number} [isolationLevel] Controls the locking and row versioning behavior of TSQL statements issued by a connection
.
   * @param {basicCallback} [callback] A callback which is called after transaction has began, or an error has occurred. If omited
, method returns Promise.
   * @return {Transaction|Promise}
   */

  begin (isolationLevel, callback) {
    if (isolationLevel instanceof Function) {
      callback = isolationLevel
      isolationLevel = undefined
    }

    if (typeof callback === 'function') {
      this._begin(isolationLevel, err => {
        if (!err) {
          this.emit('begin')
          debug('tran: begin ok')
        }
        callback(err)
      })
      return this
    }

    return new PromiseLibrary((resolve, reject) => {
      this._begin(isolationLevel, err => {
        if (err) return reject(err)
        this.emit('begin')
        debug('tran: begin ok')
        resolve(this)
      })
    })
  }

  /**
   * @private
   * @param {Number} [isolationLevel]
   * @param {basicCallback} [callback]
   * @return {Transaction}
   */

  _begin (isolationLevel, callback) {
    debug('tran: begin')

    if (this._acquiredConnection) {
      return setImmediate(callback, new TransactionError('Transaction has already begun.', 'EALREADYBEGUN'))
    }

    this._aborted = false
    this._rollbackRequested = false
    this.isolationLevel = isolationLevel || this.isolationLevel

    setImmediate(callback)
  }

  /**
   * Commit a transaction.
   *
   * @param {basicCallback} [callback] A callback which is called after transaction has commited, or an error has occurred. If omited
, method returns Promise.
   * @return {Transaction|Promise}
   */

  commit (callback) {
    if (typeof callback === 'function') {
      this._commit(err => {
        if (!err) {
          this.emit('commit')
          debug('tran: commit')
        }
        callback(err)
      })
      return this
    }

    return new PromiseLibrary((resolve, reject) => {
      this._commit(err => {
        if (err) return reject(err)
        this.emit('commit')
        debug('tran: commit')
        resolve()
      })
    })
  }

  /**
   * @private
   * @param {basicCallback} [callback]
   * @return {Transaction}
   */

  _commit (callback) {
    debug('tran: commit')

    if (this._aborted) {
      return setImmediate(callback, new TransactionError('Transaction has been aborted.', ' ...
```
- example usage
```shell
...
'''

## Transaction

**IMPORTANT:** always use 'Transaction' class to create transactions - it ensures that all your requests are executed on one connection
. Once you call 'begin', a single connection is acquired from the connection pool and all subsequent requests (initialized with
the 'Transaction' object) are executed exclusively on this connection. After you call 'commit' or 'rollback', connection is then
 released back to the connection pool.

'''javascript
const transaction = new sql.Transaction(/* [pool] */)
'''

If you omit connection argument, global connection is used instead.

__Example__

'''javascript
...
```

#### <a name="apidoc.element.mssql.base.TransactionError"></a>[function <span class="apidocSignatureSpan">mssql.base.</span>TransactionError (message, code)](#apidoc.element.mssql.base.TransactionError)
- description and source-code
```javascript
class TransactionError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * Creates a new TransactionError.
   *
   * @param {String} message Error message.
   * @param {String} [code] Error code.
   */
</span>
  constructor (message, code) {
    if (message instanceof Error) {
      super(message.message)
      this.code = message.code || code

      Object.defineProperty(this, 'originalError', {enumerable: true, value: message})
    } else {
      super(message)
      this.code = code
    }

    this.name = 'TransactionError'
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.connectionstring"></a>[module mssql.connectionstring](#apidoc.module.mssql.connectionstring)

#### <a name="apidoc.element.mssql.connectionstring.parse"></a>[function <span class="apidocSignatureSpan">mssql.connectionstring.</span>parse (string)](#apidoc.element.mssql.connectionstring.parse)
- description and source-code
```javascript
parse = function (string) {
  let cursor = 0
  let parsing = 'name'
  let param = null
  let buffer = ''
  let quotes = null
  const parsed = {}
  const original = {}

  Object.defineProperty(parsed, '__original__', {value: original})
  Object.defineProperty(parsed, 'toString', {
    value () {
      const out = []
      for (const key in this) {
        if (IGNORE_KEYS.indexOf(key) === -1) {
          const esc = original[key].escape || ['', '']
          out.push('${original[key].name}=${esc[0] || ''}${this[key]}${esc[1] || ''}')
        }
      }
      return out.join(';')
    }
  })

  while (cursor < string.length) {
    const char = string.charAt(cursor)
    switch (char) {
      case '=':
        if (parsing === 'name') {
          buffer = buffer.trim()
          param = buffer.toLowerCase()
          original[param] = {name: buffer}
          parsing = 'value'
          buffer = ''
        } else {
          buffer += char
        }
        break

      case '\'': case '"':
        if (parsing === 'value') {
          if (!buffer.trim().length) {
            // value is wrapped in qotes
            original[param].escape = [char, char]
            quotes = char
            buffer = ''
          } else if (quotes) {
            if (char === quotes) {
              // found same char as used for wrapping quotes
              if (char === string.charAt(cursor + 1)) {
                // escaped quote
                buffer += char
                cursor++
              } else {
                // end of value
                parsed[param] = buffer
                param = null
                parsing = null
                buffer = ''
                quotes = null
              }
            } else {
              buffer += char
            }
          } else {
            buffer += char
          }
        } else {
          throw new Error('Invalid connection string.')
        }
        break

      case '{':
        if (parsing === 'value') {
          if (buffer.trim().length === 0) {
            // value is wrapped in qotes
            original[param].escape = ['{', '}']
            quotes = '{}'
            buffer = ''
          } else {
            buffer += char
          }
        } else {
          throw new Error('Invalid connection string.')
        }
        break

      case '}':
        if (parsing === 'value') {
          if (quotes === '{}') {
            // end of value
            parsed[param] = buffer
            param = null
            parsing = null
            buffer = ''
            quotes = null
          } else {
            buffer += char
          }
        } else {
          throw new Error('Invalid connection string.')
        }
        break

      case ';':
        if (parsing === 'value') {
          if (quotes) {
            buffer += char
          } else {
            // end of value
            parsed[param] = buffer
            param = null
            parsing = 'name'
            buffer = ''
          }
        } else {
          buffer = ''
          parsing = 'name'
        }
        break

      default:
        buffer += char
    }

    cursor++
  }

  if (parsing === 'value') {
    // end of value
    parsed[param] = buffer
  }

  return parsed
}
```
- example usage
```shell
...
  if (arguments[i] !== null && arguments[i] !== undefined) {
    return arguments[i]
  }
}
}

const parseConnectionURI = function (uri) {
const parsed = url.parse(uri)
let instance
let user
let password

const path = parsed.pathname.substr(1).split('/')
if (path.length > 1) {
  instance = path.shift()
...
```

#### <a name="apidoc.element.mssql.connectionstring.resolve"></a>[function <span class="apidocSignatureSpan">mssql.connectionstring.</span>resolve (string, driver)](#apidoc.element.mssql.connectionstring.resolve)
- description and source-code
```javascript
resolve = function (string, driver) {
  const parsed = /^(mssql|tedious|msnodesql|tds):\/\//i.test(string) ? parseConnectionURI(string) : parseConnectionString(string
)
  const stream = (parsed.stream || '').toLowerCase()
  const encrypt = (parsed.encrypt || '').toLowerCase()

  if (driver === 'msnodesqlv8') {
    parsed.driver = 'SQL Server Native Client 11.0'

    if (parsed.__original__) {
      parsed.__original__.driver = {name: 'Driver', escape: ['{', '}']}
    }

    return {connectionString: parsed.toString()}
  }

  let user = parsed.uid || parsed.uid || parsed['user id']
  let server = parsed.server || parsed.address || parsed.addr || parsed['data source'] || parsed['network address']

  const config = {
    password: oror(parsed.pwd, parsed.password),
    database: oror(parsed.database, parsed['initial catalog']),
    connectionTimeout: oror(parsed.connectionTimeout, parsed.timeout, parsed['connect timeout'], parsed['connection timeout']),
    requestTimeout: oror(parsed.requestTimeout, parsed['request timeout']),
    stream: stream === 'true' || stream === 'yes' || stream === '1',
    options: {
      encrypt: encrypt === 'true' || encrypt === 'yes' || encrypt === '1'
    }
  }

  if (parsed.useUTC != null) {
    const utc = parsed.useUTC.toLowerCase()
    config.options.useUTC = utc === 'true' || utc === 'yes' || utc === '1'
  }
  if (config.connectionTimeout != null) {
    config.connectionTimeout = parseInt(config.connectionTimeout, 10)
  }
  if (config.requestTimeout != null) {
    config.requestTimeout = parseInt(config.requestTimeout, 10)
  }

  if (/^(.*)\\(.*)$/.exec(user)) {
    config.domain = RegExp.$1
    user = RegExp.$2
  }

  if (server) {
    server = server.trim()

    if (/^np:/i.test(server)) {
      throw new Error('Connection via Named Pipes is not supported.')
    }

    if (/^tcp:/i.test(server)) {
      server = server.substr(4)
    }

    if (/^(.*)\\(.*)$/.exec(server)) {
      server = RegExp.$1
      config.options.instanceName = RegExp.$2
    }

    if (/^(.*),(.*)$/.exec(server)) {
      server = RegExp.$1.trim()
      config.port = parseInt(RegExp.$2.trim(), 10)
    }

    if (server === '.' || server === '(.)' || server.toLowerCase() === '(localdb)' || server.toLowerCase() === '(local)') {
      server = 'localhost'
    }
  }

  config.user = user
  config.server = server
  return config
}
```
- example usage
```shell
...

this.config = config
this._connected = false
this._connecting = false

if (typeof this.config === 'string') {
  try {
    this.config = ConnectionString.resolve(this.config, driver.name)
  } catch (ex) {
    if (typeof callback === 'function') {
      return callback(ex)
    }
    throw ex
  }
}
...
```



# <a name="apidoc.module.mssql.datatypes"></a>[module mssql.datatypes](#apidoc.module.mssql.datatypes)

#### <a name="apidoc.element.mssql.datatypes.cast"></a>[function <span class="apidocSignatureSpan">mssql.datatypes.</span>cast (value, type, options)](#apidoc.element.mssql.datatypes.cast)
- description and source-code
```javascript
(value, type, options) => {
  if (value == null) {
    return null
  }

  switch (typeof value) {
    case 'string':
      return 'N'${value.replace(/'/g, '\'\'')}''

    case 'number':
      return value

    case 'boolean':
      return value ? 1 : 0

    case 'object':
      if (value instanceof Date) {
        let ns = value.getUTCMilliseconds() / 1000
        if (value.nanosecondDelta != null) {
          ns += value.nanosecondDelta
        }
        const scale = options.scale == null ? 7 : options.scale

        if (scale > 0) {
          ns = String(ns).substr(1, scale + 1)
        } else {
          ns = ''
        }

        return 'N'${value.getUTCFullYear()}-${zero(value.getUTCMonth() + 1)}-${zero(value.getUTCDate())} ${zero(value.getUTCHours
())}:${zero(value.getUTCMinutes())}:${zero(value.getUTCSeconds())}${ns}''
      } else if (Buffer.isBuffer(value)) {
        return '0x${value.toString('hex')}'
      }

      return null

    default:
      return null
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
(type, options) => {
  switch (type) {
    case TYPES.VarChar: case TYPES.VarBinary:
      return '${type.declaration} (${options.length > 8000 ? 'MAX' : (options.length == null ? 'MAX' : options.length)})'
    case TYPES.NVarChar:
      return '${type.declaration} (${options.length > 4000 ? 'MAX' : (options.length == null ? 'MAX' : options.length)})'
    case TYPES.Char: case TYPES.NChar: case TYPES.Binary:
      return '${type.declaration} (${options.length == null ? 1 : options.length})'
    case TYPES.Decimal: case TYPES.Numeric:
      return '${type.declaration} (${options.precision == null ? 18 : options.precision}, ${options.scale == null ? 0 : options.
scale})'
    case TYPES.Time: case TYPES.DateTime2: case TYPES.DateTimeOffset:
      return '${type.declaration} (${options.scale == null ? 7 : options.scale})'
    case TYPES.TVP:
      return '${options.tvpType} readonly'
    default:
      return type.declaration
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mssql.map"></a>[module mssql.map](#apidoc.module.mssql.map)

#### <a name="apidoc.element.mssql.map.register"></a>[function <span class="apidocSignatureSpan">mssql.map.</span>register (jstype, sqltype)](#apidoc.element.mssql.map.register)
- description and source-code
```javascript
register = function (jstype, sqltype) {
  for (let index = 0; index < this.length; index++) {
    let item = this[index]
    if (item.js === jstype) {
      this.splice(index, 1)
      break
    }
  }

  this.push({
    js: jstype,
    sql: sqltype
  })

  return null
}
```
- example usage
```shell
...
- 'sql.Table' -> 'sql.TVP'

Default data type for unknown object is 'sql.NVarChar'.

You can define your own type map.

'''javascript
sql.map.register(MyClass, sql.Text)
'''

You can also overwrite the default type map.

'''javascript
sql.map.register(Number, sql.BigInt)
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
NVarChar(length) {
  return {type: TYPES.NVarChar, length}
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
Int() {
  return {type: TYPES.Int}
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
Bit() {
  return {type: TYPES.Bit}
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
DateTime() {
  return {type: TYPES.DateTime}
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
VarBinary(length) {
  return {type: TYPES.VarBinary, length}
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

#### <a name="apidoc.element.mssql.map.4.js.prototype.equals"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>equals (b)](#apidoc.element.mssql.map.4.js.prototype.equals)
- description and source-code
```javascript
function equals(b) {
  if (!(b instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');

  if (this === b)
    return true;

  return binding.compare(this, b) === 0;
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
...
 * @param {String} event Event name.
 * @param {Function} handler Event handler.
 * @return {ConnectionPool}
 */

module.exports.exports.removeListener = module.exports.exports.off = function removeListener (event, handler) {
  if (!globalConnectionHandlers[event]) return globalConnection
  const index = globalConnectionHandlers[event].indexOf(handler)
  if (index === -1) return globalConnection
  globalConnectionHandlers[event].splice(index, 1)
  if (globalConnectionHandlers[event].length === 0) globalConnectionHandlers[event] = undefined

  if (globalConnection) globalConnection.removeListener(event, handler)
  return globalConnection
}
...
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
n/a
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
  if (count < 1) {
    return points
  }

  for (let i = 1; i <= count; i++) {
    const point = new Point()
    points.push(point)
    point.x = buffer.readDoubleLE(buffer.position)
    point.y = buffer.readDoubleLE(buffer.position + 8)
    buffer.position += 16
  }

  return points
}
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
    attribute: 0x01,
    pointOffset: 0
  })
} else {
  for (let i = 1; i <= count; i++) {
    figures.push({
      attribute: buffer.readUInt8(buffer.position),
      pointOffset: buffer.readInt32LE(buffer.position + 1)
    })

    buffer.position += 5
  }
}

return figures
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

let numberOfPoints
if (properties.P) {
  numberOfPoints = 1
} else if (properties.L) {
  numberOfPoints = 2
} else {
  numberOfPoints = buffer.readUInt32LE(buffer.position)
  buffer.position += 4
}

// console.log("numberOfPoints", numberOfPoints)

value.points = parsePoints(buffer, numberOfPoints)
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
  figures.push({
    attribute: 0x01,
    pointOffset: 0
  })
} else {
  for (let i = 1; i <= count; i++) {
    figures.push({
      attribute: buffer.readUInt8(buffer.position),
      pointOffset: buffer.readInt32LE(buffer.position + 1)
    })

    buffer.position += 5
  }
}
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

#### <a name="apidoc.element.mssql.map.4.js.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mssql.map.4.js.prototype.</span>toJSON ()](#apidoc.element.mssql.map.4.js.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.length) {
    const data = [];
    for (var i = 0; i < this.length; ++i)
      data[i] = this[i];
    return { type: 'Buffer', data };
  } else {
    return { type: 'Buffer', data: [] };
  }
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
if (driver === 'msnodesqlv8') {
  parsed.driver = 'SQL Server Native Client 11.0'

  if (parsed.__original__) {
    parsed.__original__.driver = {name: 'Driver', escape: ['{', '}']}
  }

  return {connectionString: parsed.toString()}
}

let user = parsed.uid || parsed.uid || parsed['user id']
let server = parsed.server || parsed.address || parsed.addr || parsed['data source'] || parsed['network address']

const config = {
  password: oror(parsed.pwd, parsed.password),
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
n/a
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
  if (name) {
    const parsed = Table.parseName(name)
    this.name = parsed.name
    this.schema = parsed.schema
    this.database = parsed.database
    this.path = (this.database ? '[${this.database}].' : '') + (this.schema ? '[${this.schema}].' : '') + '[${this.name}]'
    this.temporary = this.name.charAt(0) === '#'
  }

  this.columns = []
  this.rows = []

  Object.defineProperty(this.columns, 'add', {
    value (name, column, options) {
      if (column == null) {
        throw new Error('Column data type is not defined.')
      }
      if (column instanceof Function) {
        column = column()
      }

      options = options || {}
      column.name = name
      column.nullable = options.nullable
      column.primary = options.primary

      return this.push(column)
    }
  }
  )

  Object.defineProperty(this.rows, 'add', {
    value () {
      return this.push(Array.prototype.slice.call(arguments))
    }
  }
  )
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mssql.map.5.sql"></a>[function <span class="apidocSignatureSpan">mssql.map.5.</span>sql (tvpType)](#apidoc.element.mssql.map.5.sql)
- description and source-code
```javascript
TVP(tvpType) {
  return {type: TYPES.TVP, tvpType}
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
