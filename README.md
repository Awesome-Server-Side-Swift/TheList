# The Awesome Server Side Swift List

A curated list of awesome Server Side Swift 3 projects.

Interested in conributing? Please see the [Contributing](#contributing) section below. Please note that components targeting iOS projects will not be considered unless there is a clear use case for a server side implementation. Projects must also be SPM modules that can be included as dependancies, unless otherwise stated.

Thanks goes out to [vsouza](https://github.com/vsouza) for the inspiration of his Awesome iOS list!

## Table of Contents

* [Server Side Swift Frameworks](#server-side-swift-frameworks)
* [Server Side Utilities](#server-side-utilities)
	* [File System](#file-system)
	* [Compression](#compression)
	* [Encryption / Cryptography](#encryption--cryptography)
	* [Logging](#logging)
	* [Command Line Access](#command-line-access)
	* [iOS Notifications](#ios-notifications)
	* [Networking](#networking)
	* [Configuration](#configuration)
	* [Testing](#testing)
	* [Miscellaneous](#miscellaneous)
* [Authentication](#authentication)
* [Templating](#templating)
* [Parsers](#parsers)
	* [JSON](#json)
	* [XML](#XML)
	* [Miscellaneous Parsers](#miscellaneous-parsers)
* [Utility](#utility)
	* [Strings](#strings)
* [Database Connectors](#database-connectors)
	* [MySQL](#mysql)
	* [PostgreSQL](#postgresql)
	* [SQLite](#sqlite)
	* [MongoDB](#mongodb)
	* [Redis](#redis)
	* [FileMaker](#filemaker)
* [ORM](#orm)
* [Web Server Connectivity](#web-server-connectivity)
	* [HTTP](#http-libraries)
	* [WebSockets](#websockets)

## Server Side Swift Frameworks
Server Side Swift frameworks are projects that provide an infrastructure with which you can build a working Swift API.

* [Kitura](https://github.com/IBM-Swift/Kitura)
* [Perfect](https://github.com/PerfectlySoft/Perfect)
* [Vapor](https://github.com/vapor/vapor)
* [Zewo](https://github.com/Zewo/Zewo)

## Server Side Utilities

### File System

* [Perfect File / Dir](https://github.com/PerfectlySoft/Perfect) (in core library).

### Compression

* [Perfect-Zip](https://github.com/PerfectlySoft/Perfect-Zip) - Perfect Zip compression utility.
* [Zewo gzip](https://github.com/Zewo/gzip) - gzip data compression from Swift, OS X & Linux ready.
* [Zewo zlib](https://github.com/Zewo/zlib) - SwiftPM-compatible fork of zlib, OS X & Linux ready.
* [Vapor gzip](https://github.com/vapor/gzip-provider)

### Encryption / Cryptography

* [AES256CBC](https://github.com/SwiftyBeaver/AES256CBC) - convenient AES256 encryption of strings
* [CryptoSwift](https://github.com/krzyzanowskim/CryptoSwift) - A growing collection of standard and secure cryptographic algorithms implemented in Swift
* [Perfect OpenSSL](https://github.com/PerfectlySoft/Perfect-COpenSSL) - OpenSSL module (without Homebrew dependancy)
* [SwiftMD5](https://github.com/iamjono/SwiftMD5) - A pure Swift implementation of MD5
* [Vapor TLS](https://github.com/vapor/tls) - Swift OpenSSL and TLS wrapper.
* [Vapor Crypto](https://github.com/vapor/crypto) (Formerly CryptoKitten).
* [Zewo OpenSSL](https://github.com/Zewo/COpenSSL)

### Logging

* [Zewo Log](https://github.com/ZewoGraveyard/Log)
* [Perfect Logging](https://github.com/PerfectlySoft/Perfect) - component of core Perfect Library.
* [Vapor SwiftyBeaver](https://github.com/SwiftyBeaver/SwiftyBeaver-Vapor) - Logging Provider for Vapor, the server-side Swift 3 web framework
* [SwiftyBeaver](https://github.com/SwiftyBeaver/SwiftyBeaver) - convenient logging during development & release to console, file & cloud

### Command Line Access

* [SysProcess](https://github.com/PerfectlySoft/Perfect) - component of core Perfect Library.
* [Vapor Console](https://github.com/vapor/console) - Swift wrapper for Console I/O

### iOS Notifications

* [Perfect-Notifications](https://github.com/PerfectlySoft/Perfect-Notifications) - iOS Notifications, etc. for Perfect.

### Networking

* [Perfect Networking Library](https://github.com/PerfectlySoft/Perfect-Net) - Core asynchronous networking package used in Perfect. Includes support for TCP, SSL, UNIX socket files and IO event handling.
* [Perfect CURL](https://github.com/PerfectlySoft/Perfect-CURL) - cURL support for Perfect.
* [Vapor Socks](https://github.com/vapor/socks) - Pure-Swift Sockets: TCP, UDP; Client, Server; Linux, OS X.
* [Zewo HTTP Client](https://github.com/Zewo/HTTPClient)
* [Zewo HTTPS Client](https://github.com/ZewoGraveyard/HTTPSClient)

### Configuration

* [JSON Config](https://github.com/iamjono/JSONConfig) - A Swift 3 JSON Config reader library. Reads JSON files for server side configuration.
* [Swifty-pList](https://github.com/iamjono/Swifty-pList) - A Swift 3 pList library. Reads & writes pLists for server side configuration.

### Testing

* [SwiftRandom](https://github.com/iamjono/SwiftRandom) - A tiny generator of random data for swift. SPM module.

### Miscellaneous

* [Pefect Thread Library](https://github.com/PerfectlySoft/Perfect-Thread) - Core threading library for Perfect Server Side Swift. Includes support for serial and concurrent thread queues, locks, read/write locks and events.
* [Zewo Threading](https://github.com/Zewo/Thread) - A concise and type-safe wrapper around the POSIX pthread API.
* [Console](https://github.com/vapor/console)
* [Zewo ZeroMQ](https://github.com/ZewoGraveyard/ZeroMQ) - Distributed Messaging platform.
* [Zewo UUID](https://github.com/Zewo/UUID) - Easily generate UUID's in Swift.
* [Perfect UUID](https://github.com/PerfectlySoft/Perfect) - included in Core library.
* [POSIXRegex](https://github.com/ZewoGraveyard/POSIXRegex) - provides POSIX Regular Expressions for Swift 3.0.
* [HTTP Serializer](https://github.com/ZewoGraveyard/HTTPSerializer)

## Authentication

* [Turnstile](https://github.com/stormpath/Turnstile) - an authentication framework for Swift. Integrations with:
 * [Vapor](https://github.com/vapor/vapor/tree/master/Sources/Auth/Authentication)
 * [Perfect](https://github.com/stormpath/Turnstile-Perfect)
* [Hashed Password](https://github.com/Zewo/HashedPassword)
* [JSON WebTokens](https://github.com/Zewo/JSONWebToken)

## Templating

* [Perfect Mustache](https://github.com/PerfectlySoft/Perfect-Mustache) - Mustache template support for Perfect.
* [Leaf](https://github.com/vapor/leaf) - An extensible templating language built for Vapor.
* [Vapor Markdown Provider](https://github.com/vapor/markdown-provider)
* [Vapor Mustache](https://github.com/vapor/mustache-provider)
* [Zewo Mustache](https://github.com/Zewo/Mustache)
* [MuttonChop](https://github.com/Danappelxx/MuttonChop) - Mustache templates in Swift

## Parsers

### JSON

* [Vapor JSON](https://github.com/vapor/json) - JSON wrapper around Node.
* [Perfect JSON Convertible objects](https://github.com/PerfectlySoft/Perfect) - included in the Perfect core library.
* [Zewo JSON](https://github.com/Zewo/JSON)
* [Vdka JSON](https://github.com/Vdka/JSON)
* [Zewo HTTPParser](https://github.com/ZewoGraveyard/HTTPParser) - HTTP (RFC 2616) parser for Swift 3.0.

### XML

* [Perfect XML](https://github.com/PerfectlySoft/Perfect-XML) - XML support for Perfect.
* [Zewo XML](https://github.com/Zewo/XML) - XML/HTML parser for Swift.

### Miscellaneous Parsers

* [URI Parser](https://github.com/ZewoGraveyard/URI) - URI (RFC 3986) for Swift 3.0.

## Utility

### Strings

* [SwiftString](https://github.com/iamjono/SwiftString) - A comprehensive, lightweight string extension for Swift 3

## Database Connectors

### MySQL

* [Perfect MySQL connector](https://github.com/PerfectlySoft/Perfect-MySQL) - A stand-alone Swift wrapper around the MySQL client library.
* [Vapor MySQL Provider](https://github.com/vapor/mysql-provider)
* [Vapor MySQL Interface](https://github.com/vapor/mysql)
* [MySQL driver for Fluent](https://github.com/vapor/mysql-driver)
* [Zewo MySQL Driver](https://github.com/Zewo/MySQL)

### PostgreSQL

* [Perfect PostgreSQL connector](https://github.com/PerfectlySoft/Perfect-PostgreSQL) - A stand-alone Swift wrapper around the libpq client library.
* [Vapor PostgreSQL interface](https://github.com/vapor/postgresql)
* [Fluent PostgreSQL Driver](https://github.com/vapor/postgresql-driver) 
* [Vapor SQLite3 wrapper for Swift](https://github.com/vapor/sqlite)
* [Zewo PostgreSQL](https://github.com/Zewo/PostgreSQL)

### SQLite

* [Perfect SQLite connector](https://github.com/PerfectlySoft/Perfect-SQLite) - A stand-alone Swift wrapper around the SQLite 3 client library.
* [SQLite3 provider for Vapor](https://github.com/vapor/sqlite-provider)
* [SQLite driver for Fluent](https://github.com/vapor/sqlite-driver)

### MongoDB

* [Perfect MongoDB connector](https://github.com/PerfectlySoft/Perfect-MongoDB) - A stand-alone Swift wrapper around the mongo-c client library.
* [MongoDB driver for Fluent](https://github.com/vapor/mongo-driver) - MongoDB driver for Fluent.
* [MongoKitten](https://github.com/OpenKitten/MongoKitten) - Native MongoDB driver for Swift, written in Swift

### Redis

* [Perfect Redis connector](https://github.com/PerfectlySoft/Perfect-Redis) - A stand-alone Swift wrapper around the Redis client library, enabling access to Redis.
* [Redbird](https://github.com/vapor/redbird) - Pure-Swift Redis client implemented from the original protocol spec. OS X + Linux compatible.
* [Vapor Redbird/Redis provider](https://github.com/vapor/redis-provider)
* [Zewo Redis client](https://github.com/Zewo/Redis) - Redis client for (pure) Swift.

### FileMaker

* [Perfect Filemaker connector](https://github.com/PerfectlySoft/Perfect-FileMaker) - A stand-alone Swift wrapper around the FileMaker XML Web publishing interface.

## ORM

* [Fluent](https://github.com/vapor/fluent) (Vapor) - Swift models, relationships, and querying for NoSQL and SQL databases.
* [SQL](https://github.com/Zewo/SQL) (Zewo) - Provides an ORM and base conformance for SQL adapters.

## Web Server Connectivity

### HTTP Libraries
Connectors to Web servers such as Apache, nginx.

* [Perfect HTTP Server](https://github.com/PerfectlySoft/Perfect-HTTPServer) - HTTP 1.1 Server for Perfect Server Side Swift.
* [Perfect HTTP Libraries](https://github.com/PerfectlySoft/Perfect-HTTP) - Base HTTP Support for Perfect.
* [Perfect FastCGI Apache 2.4](https://github.com/PerfectlySoft/Perfect-FastCGI-Apache2.4)
* [Perfect FastCGI](https://github.com/PerfectlySoft/Perfect-FastCGI) - FastCGI server for Perfect.
* [Vapor Engine](https://github.com/vapor/engine) - Pure Swift HTTP

### WebSockets

* [Zewo WebSocket Server](https://github.com/Zewo/WebSocketServer)
* [Zewo WebSocket Client](https://github.com/Zewo/WebSocketClient)
* [Perfect WebSockets](https://github.com/PerfectlySoft/Perfect-WebSockets) - WebSockets support for Perfect
* [Vapor Engine](https://github.com/vapor/engine) - Pure Swift WebSockets

### Distributed Messaging

* [Zewo ZeroMQ](https://github.com/Zewo/ZeroMQ)

## Contributing

Submit a pull request with changes. Please use GitHub Issues for dead or changed links only.

* Search previous suggestions before making a new one, as yours may be a duplicate.
* Make an individual pull request for each suggestion.
* Use the following format: [PACKAGE](LINK) - DESCRIPTION.
* New categories, or improvements to the existing categorization are welcome.
* Keep descriptions short and simple, but descriptive.
* End all descriptions with a full stop/period.
* Check your spelling and grammar.
* Make sure that your suggestion is positioned as the last item category.
* Make sure your text editor is set to remove trailing whitespace.
* Projects *must* work in Swift 3.0 (or above). ObjC and Swift 1 & 2 projects will not be considered.
* The Project must be an SPM module that can be included directly, unless otherwise stated.

Projects are ineligible if:

* The project is not in and of itself, an SPM module. 
* Doesn't have commit for more than two years.
* Only have README in another language (Chinese, Japanese, Portuguese and etc)
* We cannot clearly understand the objective.
* Without clear README


## License
Distributed under the MIT license. See [LICENSE](https://github.com/Awesome-Server-Side-Swift/TheList/blob/master/LICENSE) for more information.

## Code of Conduct

We welcome people of all ethnicities, nationalities, ages, gender, disability, levels of experience, and religious beliefs to use and contribute to this project. We pledge to foster and enforce a harassment-free environment of openness, respect, and cooperation for everyone in all project and public spaces online or offline.

Please report any behaviour that violates our Code of Conduct. The team is committed to enforcing this Code of Conduct to ensure everyone who wishes to use, contribute to, and comment on the project may do so freely and openly and without fear of reprisal.

We will investigate all complaints of unacceptable or abusive behaviour or comments expediently, and we will maintain the confidentiality of the person who reports any perceived infraction or wrongdoing to us. We will not tolerate any form of direct or indirect harassment or discrimination within the Swift community, and will take appropriate, fair, and corrective action to any instance of inappropriate behaviour.

The team maintains the right to remove, edit, or reject any comments, code, edits, or issues that do not align with our Code of Conduct.
