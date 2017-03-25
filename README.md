# api documentation for  [browser-sync (v2.18.8)](http://www.browsersync.io/)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-browser-sync.svg)](https://travis-ci.org/npmdoc/node-npmdoc-browser-sync)
#### Live CSS Reload & Browser Syncing

[![NPM](https://nodei.co/npm/browser-sync.png?downloads=true)](https://www.npmjs.com/package/browser-sync)

[![apidoc](https://npmdoc.github.io/node-npmdoc-browser-sync/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-browser_sync_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-browser-sync/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-browser-sync/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Shane Osbourne"
    },
    "bin": {
        "browser-sync": "bin/browser-sync.js"
    },
    "bugs": {
        "url": "https://github.com/browsersync/browser-sync/issues"
    },
    "dependencies": {
        "browser-sync-client": "2.4.5",
        "browser-sync-ui": "0.6.3",
        "bs-recipes": "1.3.4",
        "chokidar": "1.6.1",
        "connect": "3.5.0",
        "dev-ip": "^1.0.1",
        "easy-extender": "2.3.2",
        "eazy-logger": "3.0.2",
        "emitter-steward": "^1.0.0",
        "fs-extra": "1.0.0",
        "http-proxy": "1.15.2",
        "immutable": "3.8.1",
        "localtunnel": "1.8.2",
        "micromatch": "2.3.11",
        "opn": "4.0.2",
        "portscanner": "2.1.1",
        "qs": "6.2.1",
        "resp-modifier": "6.0.2",
        "rx": "4.1.0",
        "serve-index": "1.8.0",
        "serve-static": "1.11.1",
        "server-destroy": "1.0.1",
        "socket.io": "1.6.0",
        "socket.io-client": "1.6.0",
        "ua-parser-js": "0.7.12",
        "yargs": "6.4.0"
    },
    "description": "Live CSS Reload & Browser Syncing",
    "devDependencies": {
        "browser-sync-spa": "1.0.3",
        "bs-html-injector": "3.0.3",
        "bs-latency": "1.0.0",
        "bs-rewrite-rules": "2.0.0",
        "bs-snippet-injector": "2.0.1",
        "chai": "3.5.0",
        "chalk": "1.1.3",
        "compression": "1.6.2",
        "eslint": "3.7.1",
        "graceful-fs": "4.1.9",
        "gulp": "3.9.1",
        "gulp-contribs": "0.0.3",
        "gulp-conventional-changelog": "1.1.0",
        "gulp-filter": "4.0.0",
        "http2": "^3.3.6",
        "istanbul": "0.4.5",
        "istanbul-coveralls": "1.0.3",
        "lodash-cli": "4.15.0",
        "mocha": "3.0.2",
        "q": "1.4.1",
        "request": "2.74.0",
        "rimraf": "2.5.4",
        "sinon": "1.17.5",
        "socket.io-client": "1.5.0",
        "supertest": "2.0.0",
        "vinyl": "1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "2fb4de253798d7cfb839afb9c2f801968490cec2",
        "tarball": "https://registry.npmjs.org/browser-sync/-/browser-sync-2.18.8.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "files": [
        "bin",
        "index.js",
        "lib",
        "lodash.custom.js"
    ],
    "gitHead": "9e0a170df275d35d09e098bff816fc7c9885842e",
    "homepage": "http://www.browsersync.io/",
    "keywords": [
        "browser sync",
        "css",
        "live reload",
        "sync"
    ],
    "license": "Apache-2.0",
    "maintainers": [
        {
            "name": "shakyshane",
            "email": "shane.osbourne8@gmail.com"
        }
    ],
    "name": "browser-sync",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/browsersync/browser-sync.git"
    },
    "scripts": {
        "cover": "npm run env && npm run cover-local && npm run coveralls",
        "cover-local": "istanbul cover -x lodash.custom.js _mocha -- --timeout 10000 --recursive ./test/specs",
        "coveralls": "istanbul-coveralls",
        "env": "node ./test/env.js",
        "lint": "eslint index.js lib bin examples test/specs gulpfile.js --fix",
        "lodash": "lodash include=isUndefined,isFunction,toArray,includes,union,each,isString,merge,isObject,set exports=node",
        "pre-release": "npm test && npm run pro-local && npm run pro",
        "pro": "protractor test/protractor/config.single.js",
        "pro-local": "node test/protractor/setup.js",
        "test": "npm run lint && npm run env && npm run unit",
        "unit": "mocha --recursive test/specs --timeout 10000 --bail"
    },
    "version": "2.18.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module browser-sync](#apidoc.module.browser-sync)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>browser_sync (emitter)](#apidoc.element.browser-sync.browser_sync)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>create (name, emitter)](#apidoc.element.browser-sync.create)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>exit ()](#apidoc.element.browser-sync.exit)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>get (name)](#apidoc.element.browser-sync.get)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>has (name)](#apidoc.element.browser-sync.has)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>init ()](#apidoc.element.browser-sync.init)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>notify ()](#apidoc.element.browser-sync.notify)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>pause ()](#apidoc.element.browser-sync.pause)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>reload ()](#apidoc.element.browser-sync.reload)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>reset ()](#apidoc.element.browser-sync.reset)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>resume ()](#apidoc.element.browser-sync.resume)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>stream ()](#apidoc.element.browser-sync.stream)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>use ()](#apidoc.element.browser-sync.use)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>watch ()](#apidoc.element.browser-sync.watch)
1.  object <span class="apidocSignatureSpan">browser-sync.</span>async
1.  object <span class="apidocSignatureSpan">browser-sync.</span>browser_sync.prototype
1.  object <span class="apidocSignatureSpan">browser-sync.</span>connect_utils
1.  object <span class="apidocSignatureSpan">browser-sync.</span>file_event_handler
1.  object <span class="apidocSignatureSpan">browser-sync.</span>file_utils
1.  object <span class="apidocSignatureSpan">browser-sync.</span>file_watcher
1.  object <span class="apidocSignatureSpan">browser-sync.</span>hooks
1.  object <span class="apidocSignatureSpan">browser-sync.</span>http_protocol
1.  object <span class="apidocSignatureSpan">browser-sync.</span>instances
1.  object <span class="apidocSignatureSpan">browser-sync.</span>logger
1.  object <span class="apidocSignatureSpan">browser-sync.</span>options
1.  object <span class="apidocSignatureSpan">browser-sync.</span>plugins
1.  object <span class="apidocSignatureSpan">browser-sync.</span>server
1.  object <span class="apidocSignatureSpan">browser-sync.</span>sockets
1.  object <span class="apidocSignatureSpan">browser-sync.</span>utils

#### [module browser-sync.async](#apidoc.module.browser-sync.async)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>getEmptyPort (bs, done)](#apidoc.element.browser-sync.async.getEmptyPort)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>getExtraPortForProxy (bs, done)](#apidoc.element.browser-sync.async.getExtraPortForProxy)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>getOnlineStatus (bs, done)](#apidoc.element.browser-sync.async.getOnlineStatus)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>initUserPlugins (bs, done)](#apidoc.element.browser-sync.async.initUserPlugins)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>mergeMiddlewares (bs, done)](#apidoc.element.browser-sync.async.mergeMiddlewares)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>mergeUiSettings (bs, done)](#apidoc.element.browser-sync.async.mergeUiSettings)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>resolveInlineUserPlugins (bs, done)](#apidoc.element.browser-sync.async.resolveInlineUserPlugins)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>setFileWatchers (bs, done)](#apidoc.element.browser-sync.async.setFileWatchers)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>setInternalEvents (bs, done)](#apidoc.element.browser-sync.async.setInternalEvents)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>setOptions (bs, done)](#apidoc.element.browser-sync.async.setOptions)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>startServer (bs, done)](#apidoc.element.browser-sync.async.startServer)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>startSockets (bs, done)](#apidoc.element.browser-sync.async.startSockets)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>startTunnel (bs, done)](#apidoc.element.browser-sync.async.startTunnel)
1.  [function <span class="apidocSignatureSpan">browser-sync.async.</span>startUi (bs, done)](#apidoc.element.browser-sync.async.startUi)

#### [module browser-sync.browser_sync](#apidoc.module.browser-sync.browser_sync)
1.  [function <span class="apidocSignatureSpan">browser-sync.</span>browser_sync (emitter)](#apidoc.element.browser-sync.browser_sync.browser_sync)

#### [module browser-sync.browser_sync.prototype](#apidoc.module.browser-sync.browser_sync.prototype)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>_addMiddlewareToStack (entry)](#apidoc.element.browser-sync.browser_sync.prototype._addMiddlewareToStack)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>addMiddleware (route, handle, opts)](#apidoc.element.browser-sync.browser_sync.prototype.addMiddleware)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>addRewriteRule (rule)](#apidoc.element.browser-sync.browser_sync.prototype.addRewriteRule)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>callback (name)](#apidoc.element.browser-sync.browser_sync.prototype.callback)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>cleanup (cb)](#apidoc.element.browser-sync.browser_sync.prototype.cleanup)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getExternalSocketConnector (opts)](#apidoc.element.browser-sync.browser_sync.prototype.getExternalSocketConnector)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getLogger (name)](#apidoc.element.browser-sync.browser_sync.prototype.getLogger)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getMiddleware (type)](#apidoc.element.browser-sync.browser_sync.prototype.getMiddleware)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOption (name)](#apidoc.element.browser-sync.browser_sync.prototype.getOption)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOptionIn (path)](#apidoc.element.browser-sync.browser_sync.prototype.getOptionIn)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOptions ()](#apidoc.element.browser-sync.browser_sync.prototype.getOptions)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getSocketConnector (opts)](#apidoc.element.browser-sync.browser_sync.prototype.getSocketConnector)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getSocketIoScript ()](#apidoc.element.browser-sync.browser_sync.prototype.getSocketIoScript)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getUserPlugin (name)](#apidoc.element.browser-sync.browser_sync.prototype.getUserPlugin)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getUserPlugins (filter)](#apidoc.element.browser-sync.browser_sync.prototype.getUserPlugins)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>init (options, cb)](#apidoc.element.browser-sync.browser_sync.prototype.init)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>registerCleanupTask (fn)](#apidoc.element.browser-sync.browser_sync.prototype.registerCleanupTask)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>registerPlugin (module, opts, cb)](#apidoc.element.browser-sync.browser_sync.prototype.registerPlugin)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>removeMiddleware (id)](#apidoc.element.browser-sync.browser_sync.prototype.removeMiddleware)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>removeRewriteRule (id)](#apidoc.element.browser-sync.browser_sync.prototype.removeRewriteRule)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>resetMiddlewareStack ()](#apidoc.element.browser-sync.browser_sync.prototype.resetMiddlewareStack)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>serveFile (path, props)](#apidoc.element.browser-sync.browser_sync.prototype.serveFile)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setMany (fn, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setMany)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setOption (name, value, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setOption)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setOptionIn (path, value, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setOptionIn)
1.  [function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setRewriteRules (rules)](#apidoc.element.browser-sync.browser_sync.prototype.setRewriteRules)

#### [module browser-sync.connect_utils](#apidoc.module.browser-sync.connect_utils)
1.  [function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>clientScript (options, both)](#apidoc.element.browser-sync.connect_utils.clientScript)
1.  [function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>getConnectionUrl (options)](#apidoc.element.browser-sync.connect_utils.getConnectionUrl)
1.  [function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>getNamespace (socketOpts, options)](#apidoc.element.browser-sync.connect_utils.getNamespace)
1.  [function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>scriptTags (options)](#apidoc.element.browser-sync.connect_utils.scriptTags)
1.  [function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>socketConnector (options)](#apidoc.element.browser-sync.connect_utils.socketConnector)

#### [module browser-sync.file_event_handler](#apidoc.module.browser-sync.file_event_handler)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_event_handler.</span>applyReloadOperators (subject, options)](#apidoc.element.browser-sync.file_event_handler.applyReloadOperators)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_event_handler.</span>fileChanges (subject, options)](#apidoc.element.browser-sync.file_event_handler.fileChanges)

#### [module browser-sync.file_utils](#apidoc.module.browser-sync.file_utils)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_utils.</span>changedFile (bs, data)](#apidoc.element.browser-sync.file_utils.changedFile)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_utils.</span>getFileInfo (data, options)](#apidoc.element.browser-sync.file_utils.getFileInfo)

#### [module browser-sync.file_watcher](#apidoc.module.browser-sync.file_watcher)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_watcher.</span>plugin (bs)](#apidoc.element.browser-sync.file_watcher.plugin)
1.  [function <span class="apidocSignatureSpan">browser-sync.file_watcher.</span>watch (patterns, opts, cb)](#apidoc.element.browser-sync.file_watcher.watch)

#### [module browser-sync.hooks](#apidoc.module.browser-sync.hooks)

#### [module browser-sync.http_protocol](#apidoc.module.browser-sync.http_protocol)
1.  [function <span class="apidocSignatureSpan">browser-sync.http_protocol.</span>getUrl (args, url)](#apidoc.element.browser-sync.http_protocol.getUrl)
1.  [function <span class="apidocSignatureSpan">browser-sync.http_protocol.</span>middleware (bs)](#apidoc.element.browser-sync.http_protocol.middleware)

#### [module browser-sync.logger](#apidoc.module.browser-sync.logger)
1.  [function <span class="apidocSignatureSpan">browser-sync.logger.</span>getLogger (name)](#apidoc.element.browser-sync.logger.getLogger)
1.  [function <span class="apidocSignatureSpan">browser-sync.logger.</span>plugin (emitter, bs)](#apidoc.element.browser-sync.logger.plugin)
1.  object <span class="apidocSignatureSpan">browser-sync.</span>logger
1.  object <span class="apidocSignatureSpan">browser-sync.logger.</span>callbacks

#### [module browser-sync.options](#apidoc.module.browser-sync.options)
1.  [function <span class="apidocSignatureSpan">browser-sync.options.</span>update (options)](#apidoc.element.browser-sync.options.update)

#### [module browser-sync.plugins](#apidoc.module.browser-sync.plugins)
1.  [function <span class="apidocSignatureSpan">browser-sync.plugins.</span>requirePlugin (item)](#apidoc.element.browser-sync.plugins.requirePlugin)
1.  [function <span class="apidocSignatureSpan">browser-sync.plugins.</span>resolvePlugin (item)](#apidoc.element.browser-sync.plugins.resolvePlugin)

#### [module browser-sync.server](#apidoc.module.browser-sync.server)
1.  [function <span class="apidocSignatureSpan">browser-sync.server.</span>createServer (bs)](#apidoc.element.browser-sync.server.createServer)
1.  [function <span class="apidocSignatureSpan">browser-sync.server.</span>plugin (bs)](#apidoc.element.browser-sync.server.plugin)

#### [module browser-sync.sockets](#apidoc.module.browser-sync.sockets)
1.  [function <span class="apidocSignatureSpan">browser-sync.sockets.</span>init (server, clientEvents, bs)](#apidoc.element.browser-sync.sockets.init)
1.  [function <span class="apidocSignatureSpan">browser-sync.sockets.</span>plugin (server, clientEvents, bs)](#apidoc.element.browser-sync.sockets.plugin)

#### [module browser-sync.utils](#apidoc.module.browser-sync.utils)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>UAParser (uastring, extensions)](#apidoc.element.browser-sync.utils.UAParser)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>_makeUrl (scheme, host, port)](#apidoc.element.browser-sync.utils._makeUrl)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>arrayify (incoming)](#apidoc.element.browser-sync.utils.arrayify)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>connect ()](#apidoc.element.browser-sync.utils.connect)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>defaultCallback (err)](#apidoc.element.browser-sync.utils.defaultCallback)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>eachSeries (arr, iterator, callback)](#apidoc.element.browser-sync.utils.eachSeries)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>easyExtender (plugins, hooks)](#apidoc.element.browser-sync.utils.easyExtender)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>fail (kill, errMessage, cb)](#apidoc.element.browser-sync.utils.fail)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getConfigErrors (options)](#apidoc.element.browser-sync.utils.getConfigErrors)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getHostIp (options, devIp)](#apidoc.element.browser-sync.utils.getHostIp)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getPort (port, max, cb)](#apidoc.element.browser-sync.utils.getPort)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getPorts (options, cb)](#apidoc.element.browser-sync.utils.getPorts)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUaString (ua)](#apidoc.element.browser-sync.utils.getUaString)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrl (url, options)](#apidoc.element.browser-sync.utils.getUrl)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrlOptions (options)](#apidoc.element.browser-sync.utils.getUrlOptions)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrls (external, local, scheme, options)](#apidoc.element.browser-sync.utils.getUrls)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>isList (maybeList)](#apidoc.element.browser-sync.utils.isList)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>open (url, name, bs)](#apidoc.element.browser-sync.utils.open)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>openBrowser (url, options, bs)](#apidoc.element.browser-sync.utils.openBrowser)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>serveStatic (root, options)](#apidoc.element.browser-sync.utils.serveStatic)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>verifyConfig (options, cb)](#apidoc.element.browser-sync.utils.verifyConfig)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>willCauseReload (needles, haystack)](#apidoc.element.browser-sync.utils.willCauseReload)
1.  [function <span class="apidocSignatureSpan">browser-sync.utils.</span>xip (host, options)](#apidoc.element.browser-sync.utils.xip)
1.  object <span class="apidocSignatureSpan">browser-sync.utils.</span>devIp
1.  object <span class="apidocSignatureSpan">browser-sync.utils.</span>portscanner



# <a name="apidoc.module.browser-sync"></a>[module browser-sync](#apidoc.module.browser-sync)

#### <a name="apidoc.element.browser-sync.browser_sync"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>browser_sync (emitter)](#apidoc.element.browser-sync.browser_sync)
- description and source-code
```javascript
browser_sync = function (emitter) {

    var bs      = this;

    bs.cwd      = process.cwd();
    bs.active   = false;
    bs.paused   = false;
    bs.config   = config;
    bs.utils    = utils;
    bs.events   = bs.emitter = emitter;

    bs._userPlugins   = [];
    bs._reloadQueue   = [];
    bs._cleanupTasks  = [];
    bs._browserReload = false;

    // Plugin management
    bs.pluginManager = new EE(defaultPlugins, hooks);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.create"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>create (name, emitter)](#apidoc.element.browser-sync.create)
- description and source-code
```javascript
function create(name, emitter) {

    name    = name    || new Date().getTime();
    emitter = emitter || newEmitter();

    var browserSync = new BrowserSync(emitter);

    var instance = {
        name:      name,
        instance:  browserSync,
        exit:      require("./lib/public/exit")(browserSync),
        notify:    require("./lib/public/notify")(browserSync),
        pause:     require("./lib/public/pause")(browserSync),
        resume:    require("./lib/public/resume")(browserSync),
        reload:    require("./lib/public/reload")(emitter),
        stream:    require("./lib/public/stream")(emitter),
        cleanup:   browserSync.cleanup.bind(browserSync),
        use:       browserSync.registerPlugin.bind(browserSync),
        getOption: browserSync.getOption.bind(browserSync),
        emitter:   browserSync.events,
        watch:     require("./lib/file-watcher").watch
    };

    browserSync.publicInstance = instance;
    instance.init = require("./lib/public/init")(browserSync, name, pjson);

    Object.defineProperty(instance, "active", {
        get: function () {
            return browserSync.active;
        }
    });

    Object.defineProperty(instance, "paused", {
        get: function () {
            return browserSync.paused;
        }
    });

<span class="apidocCodeCommentSpan">    /**
     * Access to client-side socket for emitting events
     *
     * @property sockets
     */
</span>    Object.defineProperty(instance, "sockets", {
        get: function () {
            if (!browserSync.active) {
                return {
                    emit: function () {},
                    on: function () {}
                };
            } else {
                return browserSync.io.sockets;
            }
        }
    });

    instances.push(instance);

    return instance;
}
```
- example usage
```shell
...
function initSingleton() {
var instance;
if (instances.length) {
    instance = instances.filter(function (item) {
        return item.name === "singleton";
    });
    if (instance.length) {
        logger.error("{yellow:You tried to start Browsersync twice!} To create multiple instances, use {cyan:browserSync.create().
init()");
        return instance;
    }
}
var args = Array.prototype.slice.call(arguments);
singleton = create("singleton", getSingletonEmitter());

if (singletonPlugins.length) {
...
```

#### <a name="apidoc.element.browser-sync.exit"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>exit ()](#apidoc.element.browser-sync.exit)
- description and source-code
```javascript
exit = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
...
        if (_.isFunction(cb)) {
            if (errMessage.message) { // Is this an error object?
                cb(errMessage);
            } else {
                cb(new Error(errMessage));
            }
        }
        process.exit(1);
    }
},
/**
 * Add support for xip.io urls
 * @param {String} host
 * @param {Object} options
 * @returns {String}
...
```

#### <a name="apidoc.element.browser-sync.get"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>get (name)](#apidoc.element.browser-sync.get)
- description and source-code
```javascript
get = function (name) {
    var instance = getSingle(name);
    if (instance) {
        return instance;
    }
    throw new Error("An instance with the name '%s' was not found.".replace("%s", name));
}
```
- example usage
```shell
...
     * @param bs
     * @param done
     */
    getExtraPortForProxy: function (bs, done) {
/**
 * An extra port is not needed in snippet/server mode
 */
if (bs.options.get("mode") !== "proxy") {
    return done();
}

/**
 * Web socket support is disabled by default
 */
if (!bs.options.getIn(["proxy", "ws"])) {
...
```

#### <a name="apidoc.element.browser-sync.has"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>has (name)](#apidoc.element.browser-sync.has)
- description and source-code
```javascript
has = function (name) {
    var instance = getSingle(name);
    if (instance) {
        return true;
    }
    return false;
}
```
- example usage
```shell
...
return getFromString(item);
    }

    if (!isMap(item)) {
return new Plugin().mergeDeep({errors: [new Error("Plugin not supported in this format")]});
    }

    if (item.has("module")) {

var nameOrObj = item.get("module");
var options = item.get("options");

/**
 * The 'module' key can be a string, this allows
 * inline plugin references, but with options
...
```

#### <a name="apidoc.element.browser-sync.init"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>init ()](#apidoc.element.browser-sync.init)
- description and source-code
```javascript
function initSingleton() {
    var instance;
    if (instances.length) {
        instance = instances.filter(function (item) {
            return item.name === "singleton";
        });
        if (instance.length) {
            logger.error("{yellow:You tried to start Browsersync twice!} To create multiple instances, use {cyan:browserSync.create
().init()");
            return instance;
        }
    }
    var args = Array.prototype.slice.call(arguments);
    singleton = create("singleton", getSingletonEmitter());

    if (singletonPlugins.length) {
        singletonPlugins.forEach(function (obj) {
            singleton.instance.registerPlugin.apply(singleton.instance, obj.args);
        });
    }

    singleton.init.apply(null, args);
    return singleton;
}
```
- example usage
```shell
...
function initSingleton() {
var instance;
if (instances.length) {
    instance = instances.filter(function (item) {
        return item.name === "singleton";
    });
    if (instance.length) {
        logger.error("{yellow:You tried to start Browsersync twice!} To create multiple instances, use {cyan:browserSync.create().
init()");
        return instance;
    }
}
var args = Array.prototype.slice.call(arguments);
singleton = create("singleton", getSingletonEmitter());

if (singletonPlugins.length) {
...
```

#### <a name="apidoc.element.browser-sync.notify"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>notify ()](#apidoc.element.browser-sync.notify)
- description and source-code
```javascript
notify = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.pause"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>pause ()](#apidoc.element.browser-sync.pause)
- description and source-code
```javascript
pause = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.reload"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>reload ()](#apidoc.element.browser-sync.reload)
- description and source-code
```javascript
reload = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.reset"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>reset ()](#apidoc.element.browser-sync.reset)
- description and source-code
```javascript
reset = function () {
    instances.forEach(function (item) {
        item.cleanup();
    });
    instances        = [];
    singletonPlugins = [];
    singletonEmitter = false;
    singleton        = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.resume"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>resume ()](#apidoc.element.browser-sync.resume)
- description and source-code
```javascript
resume = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.stream"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>stream ()](#apidoc.element.browser-sync.stream)
- description and source-code
```javascript
stream = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.use"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>use ()](#apidoc.element.browser-sync.use)
- description and source-code
```javascript
use = function () {
    var args = Array.prototype.slice.call(arguments);
    singletonPlugins.push({
        args: args
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.watch"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>watch ()](#apidoc.element.browser-sync.watch)
- description and source-code
```javascript
watch = function () {
    var args = Array.prototype.slice.call(arguments);
    if (singleton) {
        return singleton[name].apply(singleton, args);
    } else {
        if (publicUtils.isStreamArg(name, args)) {
            return new PassThrough({objectMode: true});
        }
    }
}
```
- example usage
```shell
...

    if (typeof opts === "function") {
        cb = opts;
        opts = {};
    }

    var watcher = require("chokidar")
        .watch(patterns, opts);

    if (_.isFunction(cb)) {
        watcher.on("all", cb);
    }

    return watcher;
}
...
```



# <a name="apidoc.module.browser-sync.async"></a>[module browser-sync.async](#apidoc.module.browser-sync.async)

#### <a name="apidoc.element.browser-sync.async.getEmptyPort"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>getEmptyPort (bs, done)](#apidoc.element.browser-sync.async.getEmptyPort)
- description and source-code
```javascript
getEmptyPort = function (bs, done) {
    utils.getPorts(bs.options, function (err, port) {
        if (err) {
            return utils.fail(true, err, bs.cb);
        }
        bs.debug("Found a free port: {magenta:%s", port);
        done(null, {
            options: {
                port: port
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.getExtraPortForProxy"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>getExtraPortForProxy (bs, done)](#apidoc.element.browser-sync.async.getExtraPortForProxy)
- description and source-code
```javascript
getExtraPortForProxy = function (bs, done) {
<span class="apidocCodeCommentSpan">    /**
     * An extra port is not needed in snippet/server mode
     */
</span>    if (bs.options.get("mode") !== "proxy") {
        return done();
    }

    /**
     * Web socket support is disabled by default
     */
    if (!bs.options.getIn(["proxy", "ws"])) {
        return done();
    }

    /**
     * Use 1 higher than server port by default...
     */
    var socketPort = bs.options.get("port") + 1;

    /**
     * Or use the user-defined socket.port option instead
     */
    if (bs.options.hasIn(["socket", "port"])) {
        socketPort = bs.options.getIn(["socket", "port"]);
    }

    utils.getPort(socketPort, null, function (err, port) {
        if (err) {
            return utils.fail(true, err, bs.cb);
        }
        done(null, {
            optionsIn: [
                {
                    path: ["socket", "port"],
                    value: port
                }
            ]
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.getOnlineStatus"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>getOnlineStatus (bs, done)](#apidoc.element.browser-sync.async.getOnlineStatus)
- description and source-code
```javascript
getOnlineStatus = function (bs, done) {
    if (_.isUndefined(bs.options.get("online")) && _.isUndefined(process.env.TESTING)) {
        require("dns").resolve("www.google.com", function (err) {
            var online = false;
            if (err) {
                bs.debug("Could not resolve www.google.com, setting {magenta:online: false}");
            } else {
                bs.debug("Resolved www.google.com, setting {magenta:online: true}");
                online = true;
            }
            done(null, {
                options: {
                    online: online
                }
            });
        });
    } else {
        done();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.initUserPlugins"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>initUserPlugins (bs, done)](#apidoc.element.browser-sync.async.initUserPlugins)
- description and source-code
```javascript
initUserPlugins = function (bs, done) {

    bs.pluginManager.initUserPlugins(bs);

    done(null, {
        options: {
            userPlugins: bs.getUserPlugins()
        }
    });
}
```
- example usage
```shell
...
},
/**
 * @param {BrowserSync} bs
 * @param {Function} done
 */
initUserPlugins: function (bs, done) {

    bs.pluginManager.initUserPlugins(bs);

    done(null, {
        options: {
            userPlugins: bs.getUserPlugins()
        }
    });
}
...
```

#### <a name="apidoc.element.browser-sync.async.mergeMiddlewares"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>mergeMiddlewares (bs, done)](#apidoc.element.browser-sync.async.mergeMiddlewares)
- description and source-code
```javascript
mergeMiddlewares = function (bs, done) {

    done(null, {
        options: {
            middleware: bs.pluginManager.hook(
                "server:middleware",
                bs.options.get("middleware")
            )
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.mergeUiSettings"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>mergeUiSettings (bs, done)](#apidoc.element.browser-sync.async.mergeUiSettings)
- description and source-code
```javascript
mergeUiSettings = function (bs, done) {

    if (!bs.ui) {
        return done();
    }

    done(null, {
        options: {
            urls: bs.options.get("urls").merge(bs.ui.options.get("urls"))
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.resolveInlineUserPlugins"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>resolveInlineUserPlugins (bs, done)](#apidoc.element.browser-sync.async.resolveInlineUserPlugins)
- description and source-code
```javascript
resolveInlineUserPlugins = function (bs, done) {

    var plugins = bs.options
        .get("plugins")
        .map(pluginUtils.resolvePlugin)
        .map(pluginUtils.requirePlugin);

    plugins
        .forEach(function (plugin) {
            if (plugin.get("errors").size) {
                return logPluginError(plugin);
            }
            var jsPlugin = plugin.toJS();
            jsPlugin.options = jsPlugin.options || {};
            jsPlugin.options.moduleName = jsPlugin.moduleName;
            bs.registerPlugin(jsPlugin.module, jsPlugin.options);
        });

    function logPluginError (plugin) {
        utils.fail(true, plugin.getIn(["errors", 0]), bs.cb);
    }

    done();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.setFileWatchers"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>setFileWatchers (bs, done)](#apidoc.element.browser-sync.async.setFileWatchers)
- description and source-code
```javascript
setFileWatchers = function (bs, done) {
    done(null, {
        instance: {
            watchers: bs.pluginManager.get("file:watcher")(bs)
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.setInternalEvents"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>setInternalEvents (bs, done)](#apidoc.element.browser-sync.async.setInternalEvents)
- description and source-code
```javascript
setInternalEvents = function (bs, done) {
    require("./internal-events")(bs);
    done();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.setOptions"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>setOptions (bs, done)](#apidoc.element.browser-sync.async.setOptions)
- description and source-code
```javascript
setOptions = function (bs, done) {
    done(null, {
        options: {
            urls:        utils.getUrlOptions(bs.options),
            snippet:     connectUtils.scriptTags(bs.options),
            scriptPaths: Immutable.fromJS(connectUtils.clientScript(bs.options, true)),
            files:       bs.pluginManager.hook(
                "files:watch",
                bs.options.get("files"),
                bs.pluginManager.pluginOptions
            )
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.startServer"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>startServer (bs, done)](#apidoc.element.browser-sync.async.startServer)
- description and source-code
```javascript
startServer = function (bs, done) {

    var server = bs.pluginManager.get("server")(bs);

    done(null, {
        instance: {
            server: server.server,
            app: server.app
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.startSockets"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>startSockets (bs, done)](#apidoc.element.browser-sync.async.startSockets)
- description and source-code
```javascript
startSockets = function (bs, done) {

    var clientEvents = bs.pluginManager.hook(
        "client:events",
        bs.options.get("clientEvents").toJS()
    );

    // Start the socket, needs an existing server.
    var io = bs.pluginManager.get("socket")(
        bs.server,
        clientEvents,
        bs
    );

    done(null, {
        instance: {
            io: io
        },
        options: {
            clientEvents: Immutable.fromJS(clientEvents)
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.startTunnel"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>startTunnel (bs, done)](#apidoc.element.browser-sync.async.startTunnel)
- description and source-code
```javascript
startTunnel = function (bs, done) {
    if (bs.options.get("tunnel") && bs.options.get("online")) {
        var localTunnel = require("./tunnel");
        localTunnel(bs, function (err, tunnel) {
            if (err) {
                return done(err);
            } else {
                return done(null, {
                    optionsIn: [
                        {
                            path:  ["urls", "tunnel"],
                            value: tunnel.url
                        }
                    ],
                    instance: {
                        tunnel: tunnel
                    }
                });
            }
        });
    } else {
        done();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.async.startUi"></a>[function <span class="apidocSignatureSpan">browser-sync.async.</span>startUi (bs, done)](#apidoc.element.browser-sync.async.startUi)
- description and source-code
```javascript
startUi = function (bs, done) {

    var PLUGIN_NAME = "UI";
    var userPlugins   = bs.getUserPlugins();
    var ui            = bs.pluginManager.get(PLUGIN_NAME);
    var uiOpts        = bs.options.get("ui");

    if (!uiOpts || uiOpts.get("enabled") === false) {
        return done();
    }

    // if user provided a UI, use it instead
    if (userPlugins.some(function (item) {
        return item.name === PLUGIN_NAME;
    })) {
        uiOpts = bs.options.get("ui").mergeDeep(Immutable.fromJS(bs.pluginManager.pluginOptions[PLUGIN_NAME]));
    }

    return ui(uiOpts.toJS(), bs, function (err, ui) {
        if (err) {
            return done(err);
        }
        done(null, {
            instance: {
                ui: ui
            }
        });
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.browser_sync"></a>[module browser-sync.browser_sync](#apidoc.module.browser-sync.browser_sync)

#### <a name="apidoc.element.browser-sync.browser_sync.browser_sync"></a>[function <span class="apidocSignatureSpan">browser-sync.</span>browser_sync (emitter)](#apidoc.element.browser-sync.browser_sync.browser_sync)
- description and source-code
```javascript
browser_sync = function (emitter) {

    var bs      = this;

    bs.cwd      = process.cwd();
    bs.active   = false;
    bs.paused   = false;
    bs.config   = config;
    bs.utils    = utils;
    bs.events   = bs.emitter = emitter;

    bs._userPlugins   = [];
    bs._reloadQueue   = [];
    bs._cleanupTasks  = [];
    bs._browserReload = false;

    // Plugin management
    bs.pluginManager = new EE(defaultPlugins, hooks);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.browser_sync.prototype"></a>[module browser-sync.browser_sync.prototype](#apidoc.module.browser-sync.browser_sync.prototype)

#### <a name="apidoc.element.browser-sync.browser_sync.prototype._addMiddlewareToStack"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>_addMiddlewareToStack (entry)](#apidoc.element.browser-sync.browser_sync.prototype._addMiddlewareToStack)
- description and source-code
```javascript
_addMiddlewareToStack = function (entry) {
    var bs = this;
    if (bs.options.get("mode") === "proxy") {
        bs.app.stack.splice(bs.app.stack.length-1, 0, entry);
    } else {
        bs.app.stack.push(entry);
    }
}
```
- example usage
```shell
...
            res.setHeader("Content-Type", props.type);
            res.end(props.content);
        },
        id: "Browsersync - " + _serveFileCount++,
        route: path
    };

    bs._addMiddlewareToStack(entry);
};

/**
 * Add middlewares on the fly
 * @param {{route: string, handle: function, id?: string}}
 */
BrowserSync.prototype._addMiddlewareToStack = function (entry) {
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.addMiddleware"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>addMiddleware (route, handle, opts)](#apidoc.element.browser-sync.browser_sync.prototype.addMiddleware)
- description and source-code
```javascript
addMiddleware = function (route, handle, opts) {

    var bs   = this;

    if (!bs.app) {
        return;
    }

    opts = opts || {};

    if (!opts.id) {
        opts.id = "bs-mw-" + _addMiddlewareCount++;
    }

    if (route === "*") {
        route = "";
    }

    var entry = {
        id: opts.id,
        route: route,
        handle: handle
    };

    if (opts.override) {
        entry.override = true;
    }

    bs.options = bs.options.update("middleware", function (mw) {
        if (bs.options.get("mode") === "proxy") {
            return mw.insert(mw.size-1, entry);
        }
        return mw.concat(entry);
    });

    bs.resetMiddlewareStack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.addRewriteRule"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>addRewriteRule (rule)](#apidoc.element.browser-sync.browser_sync.prototype.addRewriteRule)
- description and source-code
```javascript
addRewriteRule = function (rule) {
    var bs = this;

    bs.options = bs.options.update("rewriteRules", function (rules) {
        return rules.concat(rule);
    });

    bs.resetMiddlewareStack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.callback"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>callback (name)](#apidoc.element.browser-sync.browser_sync.prototype.callback)
- description and source-code
```javascript
callback = function (name) {

    var bs  = this;
    var cb  = bs.options.getIn(["callbacks", name]);

    if (_.isFunction(cb)) {
        cb.apply(bs.publicInstance, _.toArray(arguments).slice(1));
    }
}
```
- example usage
```shell
...
            urls:    bs.options.get("urls").toJS(),
            tunnel:  bs.options.getIn(["urls", "tunnel"])
        });

        /**
         * Call any option-provided callbacks
         */
        bs.callback("ready", null, bs);

        /**
         * Finally, call the user-provided callback given as last arg
         */
        bs.cb(null, bs);
    };
}
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.cleanup"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>cleanup (cb)](#apidoc.element.browser-sync.browser_sync.prototype.cleanup)
- description and source-code
```javascript
cleanup = function (cb) {

    var bs = this;
    if (!bs.active) {
        return;
    }

    // Remove all event listeners
    if (bs.events) {
        bs.debug("Removing event listeners...");
        bs.events.removeAllListeners();
    }

    // Close any core file watchers
    if (bs.watchers) {
        Object.keys(bs.watchers).forEach(function (key) {
            bs.watchers[key].watchers.forEach(function (watcher) {
                watcher.close();
            });
        });
    }

    // Run any additional clean up tasks
    bs._cleanupTasks.forEach(function (fn) {
        if (_.isFunction(fn)) {
            fn(bs);
        }
    });

    // Reset the flag
    bs.debug("Setting {magenta:active: false");
    bs.active = false;
    bs.paused = false;

    bs.pluginManager.plugins        = {};
    bs.pluginManager.pluginOptions  = {};
    bs.pluginManager.defaultPlugins = defaultPlugins;

    bs._userPlugins                = [];
    bs.userPlugins                 = [];
    bs._reloadTimer                = undefined;
    bs._reloadQueue                = [];
    bs._cleanupTasks               = [];

    if (_.isFunction(cb)) {
        cb(null, bs);
    }
}
```
- example usage
```shell
...

/**
 * Reset the state of the module.
 * (should only be needed for test environments)
 */
module.exports.reset = function () {
    instances.forEach(function (item) {
        item.cleanup();
    });
    instances        = [];
    singletonPlugins = [];
    singletonEmitter = false;
    singleton        = false;
};
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getExternalSocketConnector"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getExternalSocketConnector (opts)](#apidoc.element.browser-sync.browser_sync.prototype.getExternalSocketConnector)
- description and source-code
```javascript
getExternalSocketConnector = function (opts) {

    var bs = this;

    return connectUtils.socketConnector(
        bs.options.withMutations(function (item) {
            item.set("socket", item.get("socket").merge(opts));
            if (!bs.options.getIn(["proxy", "ws"])) {
                item.set("mode", "snippet");
            }
        })
    );
}
```
- example usage
```shell
...
*/
BrowserSync.prototype.getSocketConnector = function (opts) {

   var bs = this;

   return function (req, res) {
       res.setHeader("Content-Type", "text/javascript");
       res.end(bs.getExternalSocketConnector(opts));
   };
};

/**
* Socket connector as a string
* @param {Object} opts
* @returns {*}
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getLogger"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getLogger (name)](#apidoc.element.browser-sync.browser_sync.prototype.getLogger)
- description and source-code
```javascript
getLogger = function (name) {
    return logger.clone(function (config) {
        config.prefix = config.prefix + template.replace("%s", name);
        return config;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getMiddleware"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getMiddleware (type)](#apidoc.element.browser-sync.browser_sync.prototype.getMiddleware)
- description and source-code
```javascript
getMiddleware = function (type) {

    var types = {
        "connector": connectUtils.socketConnector(this.options),
        "socket-js": require("./snippet").utils.getSocketScript()
    };

    if (type in types) {
        return function (req, res) {
            res.setHeader("Content-Type", "text/javascript");
            res.end(types[type]);
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getOption"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOption (name)](#apidoc.element.browser-sync.browser_sync.prototype.getOption)
- description and source-code
```javascript
getOption = function (name) {

    this.debug("Getting option: {magenta:%s", name);
    return this.options.get(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getOptionIn"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOptionIn (path)](#apidoc.element.browser-sync.browser_sync.prototype.getOptionIn)
- description and source-code
```javascript
getOptionIn = function (path) {

    this.debug("Getting option via path: {magenta:%s", path);
    return this.options.getIn(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getOptions"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getOptions ()](#apidoc.element.browser-sync.browser_sync.prototype.getOptions)
- description and source-code
```javascript
getOptions = function () {
    return this.options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getSocketConnector"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getSocketConnector (opts)](#apidoc.element.browser-sync.browser_sync.prototype.getSocketConnector)
- description and source-code
```javascript
getSocketConnector = function (opts) {

    var bs = this;

    return function (req, res) {
        res.setHeader("Content-Type", "text/javascript");
        res.end(bs.getExternalSocketConnector(opts));
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getSocketIoScript"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getSocketIoScript ()](#apidoc.element.browser-sync.browser_sync.prototype.getSocketIoScript)
- description and source-code
```javascript
getSocketIoScript = function () {

    return require("./snippet").utils.getSocketScript();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getUserPlugin"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getUserPlugin (name)](#apidoc.element.browser-sync.browser_sync.prototype.getUserPlugin)
- description and source-code
```javascript
getUserPlugin = function (name) {

    var bs = this;

    var items = bs.getUserPlugins(function (item) {
        return item["plugin:name"] === name;
    });

    if (items && items.length) {
        return items[0];
    }

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.getUserPlugins"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>getUserPlugins (filter)](#apidoc.element.browser-sync.browser_sync.prototype.getUserPlugins)
- description and source-code
```javascript
getUserPlugins = function (filter) {

    var bs = this;

    filter = filter || function () {
        return true;
    };

<span class="apidocCodeCommentSpan">    /**
     * Transform Plugins option
     */
</span>    bs.userPlugins = bs._userPlugins.filter(filter).map(function (plugin) {
        return {
            name: plugin["plugin:name"],
            active: plugin._enabled,
            opts: bs.pluginManager.pluginOptions[plugin["plugin:name"]]
        };
    });

    return bs.userPlugins;
}
```
- example usage
```shell
...
     *
     * @param {BrowserSync} bs
     * @param {Function} done
     */
    startUi: function (bs, done) {

var PLUGIN_NAME = "UI";
var userPlugins   = bs.getUserPlugins();
var ui            = bs.pluginManager.get(PLUGIN_NAME);
var uiOpts        = bs.options.get("ui");

if (!uiOpts || uiOpts.get("enabled") === false) {
    return done();
}
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.init"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>init (options, cb)](#apidoc.element.browser-sync.browser_sync.prototype.init)
- description and source-code
```javascript
init = function (options, cb) {

<span class="apidocCodeCommentSpan">    /**
     * Safer access to 'this'
     * @type {BrowserSync}
     */
</span>    var bs = this;

    /**
     * Set user-provided callback, or assign a noop
     * @type {Function}
     */
    bs.cb  = cb || utils.defaultCallback;

    /**
     * Verify provided config.
     * Some options are not compatible and will cause us to
     * end the process.
     */
    if (!utils.verifyConfig(options, bs.cb)) {
        return;
    }

    /**
     * Save a reference to the original options
     * @type {Map}
     * @private
     */
    bs._options = options;

    /**
     * Set additional options that depend on what the
     * user may of provided
     * @type {Map}
     */
    bs.options  = require("./options").update(options);

    /**
     * Kick off default plugins.
     */
    bs.pluginManager.init();

    /**
     * Create a base logger & debugger.
     */
    bs.logger   = bs.pluginManager.get("logger")(bs.events, bs);
    bs.debugger = bs.logger.clone({useLevelPrefixes: true});
    bs.debug    = bs.debugger.debug;

    /**
     * Run each setup task in sequence
     */
    eachSeries(
        asyncTasks,
        taskRunner(bs),
        tasksComplete(bs)
    );

    return this;
}
```
- example usage
```shell
...
function initSingleton() {
var instance;
if (instances.length) {
    instance = instances.filter(function (item) {
        return item.name === "singleton";
    });
    if (instance.length) {
        logger.error("{yellow:You tried to start Browsersync twice!} To create multiple instances, use {cyan:browserSync.create().
init()");
        return instance;
    }
}
var args = Array.prototype.slice.call(arguments);
singleton = create("singleton", getSingletonEmitter());

if (singletonPlugins.length) {
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.registerCleanupTask"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>registerCleanupTask (fn)](#apidoc.element.browser-sync.browser_sync.prototype.registerCleanupTask)
- description and source-code
```javascript
registerCleanupTask = function (fn) {

    this._cleanupTasks.push(fn);
}
```
- example usage
```shell
...
                    if (!bs.paused && data.namespace === "core") {
                        bs.events.emit("file:reload", fileUtils.getFileInfo(data, bs.options));
                    }
                });
            }
        });

    bs.registerCleanupTask(function() {
        handler.dispose();
        reloader.dispose();
    });
};
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.registerPlugin"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>registerPlugin (module, opts, cb)](#apidoc.element.browser-sync.browser_sync.prototype.registerPlugin)
- description and source-code
```javascript
registerPlugin = function (module, opts, cb) {

    var bs = this;

    bs.pluginManager.registerPlugin(module, opts, cb);

    if (module["plugin:name"]) {
        bs._userPlugins.push(module);
    }
}
```
- example usage
```shell
...
    .forEach(function (plugin) {
        if (plugin.get("errors").size) {
            return logPluginError(plugin);
        }
        var jsPlugin = plugin.toJS();
        jsPlugin.options = jsPlugin.options || {};
        jsPlugin.options.moduleName = jsPlugin.moduleName;
        bs.registerPlugin(jsPlugin.module, jsPlugin.options);
    });

function logPluginError (plugin) {
    utils.fail(true, plugin.getIn(["errors", 0]), bs.cb);
}

done();
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.removeMiddleware"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>removeMiddleware (id)](#apidoc.element.browser-sync.browser_sync.prototype.removeMiddleware)
- description and source-code
```javascript
removeMiddleware = function (id) {

    var bs = this;

    if (!bs.app) {
        return;
    }

    bs.options = bs.options.update("middleware", function (mw) {
        return mw.filter(function (mw) {
            return mw.id !== id;
        });
    });

    bs.resetMiddlewareStack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.removeRewriteRule"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>removeRewriteRule (id)](#apidoc.element.browser-sync.browser_sync.prototype.removeRewriteRule)
- description and source-code
```javascript
removeRewriteRule = function (id) {
    var bs = this;
    bs.options = bs.options.update("rewriteRules", function (rules) {
        return rules.filter(function (rule) {
            return rule.id !== id;
        });
    });

    bs.resetMiddlewareStack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.resetMiddlewareStack"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>resetMiddlewareStack ()](#apidoc.element.browser-sync.browser_sync.prototype.resetMiddlewareStack)
- description and source-code
```javascript
resetMiddlewareStack = function () {

    var bs = this;
    var middlewares = require("./server/utils").getMiddlewares(bs, bs.options);

    bs.app.stack = middlewares;
}
```
- example usage
```shell
...
   bs.options = bs.options.update("middleware", function (mw) {
       if (bs.options.get("mode") === "proxy") {
           return mw.insert(mw.size-1, entry);
       }
       return mw.concat(entry);
   });

   bs.resetMiddlewareStack();
};

/**
* Remove middlewares on the fly
* @param {String} id
* @returns {Server}
*/
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.serveFile"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>serveFile (path, props)](#apidoc.element.browser-sync.browser_sync.prototype.serveFile)
- description and source-code
```javascript
serveFile = function (path, props) {

    var bs = this;
    var mode = bs.options.get("mode");
    var entry = {
        handle: function (req, res) {
            res.setHeader("Content-Type", props.type);
            res.end(props.content);
        },
        id: "Browsersync - " + _serveFileCount++,
        route: path
    };

    bs._addMiddlewareToStack(entry);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.setMany"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setMany (fn, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setMany)
- description and source-code
```javascript
setMany = function (fn, opts) {

    var bs = this;

    opts = opts || {};

    bs.debug("Setting multiple Options");
    bs.options = bs.options.withMutations(fn);
    if (!opts.silent) {
        bs.events.emit("options:set", {options: bs.options.toJS()});
    }
    return this.options;
}
```
- example usage
```shell
...
function setOptions (bs, options) {

/**
 * If multiple options were set, act on the immutable map
 * in an efficient way
 */
if (Object.keys(options).length > 1) {
    bs.setMany(function (item) {
        Object.keys(options).forEach(function (key) {
            item.set(key, options[key]);
            return item;
        });
    });
} else {
    Object.keys(options).forEach(function (key) {
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.setOption"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setOption (name, value, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setOption)
- description and source-code
```javascript
setOption = function (name, value, opts) {

    var bs = this;

    opts = opts || {};

    bs.debug("Setting Option: {cyan:%s} - {magenta:%s", name, value.toString());

    bs.options = bs.options.set(name, value);

    if (!opts.silent) {
        bs.events.emit("options:set", {path: name, value: value, options: bs.options});
    }
    return this.options;
}
```
- example usage
```shell
...
           Object.keys(options).forEach(function (key) {
               item.set(key, options[key]);
               return item;
           });
       });
   } else {
       Object.keys(options).forEach(function (key) {
           bs.setOption(key, options[key]);
       });
   }
}

/**
* At this point, ALL async tasks have completed
* @param {BrowserSync} bs
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.setOptionIn"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setOptionIn (path, value, opts)](#apidoc.element.browser-sync.browser_sync.prototype.setOptionIn)
- description and source-code
```javascript
setOptionIn = function (path, value, opts) {

    var bs = this;

    opts = opts || {};

    bs.debug("Setting Option: {cyan:%s} - {magenta:%s", path.join("."), value.toString());
    bs.options = bs.options.setIn(path, value);
    if (!opts.silent) {
        bs.events.emit("options:set", {path: path, value: value, options: bs.options});
    }
    return bs.options;
}
```
- example usage
```shell
...
}

/**
 * Any options returned that require path access?
 */
if (out.optionsIn) {
    out.optionsIn.forEach(function (item) {
        bs.setOptionIn(item.path, item.value);
    });
}

/**
 * Any instance properties returned?
 */
if (out.instance) {
...
```

#### <a name="apidoc.element.browser-sync.browser_sync.prototype.setRewriteRules"></a>[function <span class="apidocSignatureSpan">browser-sync.browser_sync.prototype.</span>setRewriteRules (rules)](#apidoc.element.browser-sync.browser_sync.prototype.setRewriteRules)
- description and source-code
```javascript
setRewriteRules = function (rules) {
    var bs = this;
    bs.options = bs.options.update("rewriteRules", function (_) {
        return rules;
    });

    bs.resetMiddlewareStack();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.connect_utils"></a>[module browser-sync.connect_utils](#apidoc.module.browser-sync.connect_utils)

#### <a name="apidoc.element.browser-sync.connect_utils.clientScript"></a>[function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>clientScript (options, both)](#apidoc.element.browser-sync.connect_utils.clientScript)
- description and source-code
```javascript
clientScript = function (options, both) {

    var prefix    = options.getIn(["socket", "clientPath"]);
    var script    = prefix + "/browser-sync-client.js";
    var versioned = prefix + "/browser-sync-client.js?v=" + options.get("version");

    if (both) {
        return {
            path: script,
            versioned: versioned
        };
    }

    return versioned;
}
```
- example usage
```shell
...
 * @param {Function} done
 */
setOptions: function (bs, done) {
    done(null, {
        options: {
            urls:        utils.getUrlOptions(bs.options),
            snippet:     connectUtils.scriptTags(bs.options),
            scriptPaths: Immutable.fromJS(connectUtils.clientScript(bs.options, true)),
            files:       bs.pluginManager.hook(
                "files:watch",
                bs.options.get("files"),
                bs.pluginManager.pluginOptions
            )
        }
    });
...
```

#### <a name="apidoc.element.browser-sync.connect_utils.getConnectionUrl"></a>[function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>getConnectionUrl (options)](#apidoc.element.browser-sync.connect_utils.getConnectionUrl)
- description and source-code
```javascript
getConnectionUrl = function (options) {

    var socketOpts       = options.get("socket").toJS();
    var namespace        = connectUtils.getNamespace(socketOpts, options);

    var protocol         = "";
    var withHostnamePort = "'{protocol}' + location.hostname + ':{port}{ns}'";
    var withHost         = "'{protocol}' + location.host + '{ns}'";
    var withDomain       = "'{domain}{ns}'";
    var port             = options.get("port");

    // default use-case is server/proxy
    var string           = withHost;

    if (options.get("mode") !== "server") {
        protocol = options.get("scheme") + "://";
        string   = withHostnamePort;
    }

    if (options.get("mode") === "proxy" && options.getIn(["proxy", "ws"])) {
        port = options.getIn(["socket", "port"]);
    }

<span class="apidocCodeCommentSpan">    /**
     * Ensure socket.domain is always a string (for noop replacements later)
     */
</span>    socketOpts.domain = (function () {
        if (options.get("localOnly")) {
            string = withDomain;
            return [
                options.get("scheme"),
                "://localhost:",
                options.get("port")
            ].join("");
        }
        if (socketOpts.domain) {
            string = withDomain;
            /**
             * User provided a function
             */
            if (_.isFunction(socketOpts.domain)) {
                return socketOpts.domain.call(null, options);
            }
            /**
             * User provided a string
             */
            if (_.isString(socketOpts.domain)) {
                return socketOpts.domain;
            }
        }
        return "";
    })();

    return string
        .replace("{protocol}", protocol)
        .replace("{port}",     port)
        .replace("{domain}",   socketOpts.domain.replace("{port}", port))
        .replace("{ns}",       namespace);
}
```
- example usage
```shell
...
     * @param {Map} options
     * @returns {String}
     */
    socketConnector: function (options) {

var socket        = options.get("socket");
var template      = fs.readFileSync(config.templates.connector, "utf-8");
var url           = connectUtils.getConnectionUrl(options);

/**
 * ***Backwards compatibility***. While 'socket.path' is technically a
 * socketIoClientConfig property, it's been documented previously
 * as a top-level option, so must stay.
 */
var clientConfig  = socket
...
```

#### <a name="apidoc.element.browser-sync.connect_utils.getNamespace"></a>[function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>getNamespace (socketOpts, options)](#apidoc.element.browser-sync.connect_utils.getNamespace)
- description and source-code
```javascript
getNamespace = function (socketOpts, options) {

    var namespace = socketOpts.namespace;

    if (typeof namespace === "function") {
        return namespace(options);
    }

    if (!namespace.match(/^\//)) {
        namespace = "/" + namespace;
    }

    return namespace;
}
```
- example usage
```shell
...
    /**
     * @param {Map} options
     * @returns {string}
     */
    getConnectionUrl: function (options) {

var socketOpts       = options.get("socket").toJS();
var namespace        = connectUtils.getNamespace(socketOpts, options);

var protocol         = "";
var withHostnamePort = "'{protocol}' + location.hostname + ':{port}{ns}'";
var withHost         = "'{protocol}' + location.host + '{ns}'";
var withDomain       = "'{domain}{ns}'";
var port             = options.get("port");
...
```

#### <a name="apidoc.element.browser-sync.connect_utils.scriptTags"></a>[function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>scriptTags (options)](#apidoc.element.browser-sync.connect_utils.scriptTags)
- description and source-code
```javascript
scriptTags = function (options) {

    var scriptPath     = this.clientScript(options);
    var async          = options.getIn(["snippetOptions", "async"]);
    var scriptDomain   = options.getIn(["script", "domain"]);

<span class="apidocCodeCommentSpan">    /**
     * Generate the [src] attribute based on user options
     */
</span>    var scriptSrc = (function () {

        if (options.get("localOnly")) {
            return [
                options.get("scheme"),
                "://localhost:",
                options.get("port"),
                scriptPath
            ].join("");
        }

        /**
         * First, was "scriptPath" set? if so the user wanted full control over the
         * script tag output
         *
         */
        if (_.isFunction(options.get("scriptPath"))) {
            return options.get("scriptPath").apply(null, getScriptArgs(options, scriptPath));
        }

        /**
         * Next, if "script.domain" was given, allow that + the path to the JS file
         * eg:
         *  script.domain=localhost:3000
         * -> localhost:3000/browser-sync/browser-sync-client.js
         */
        if (scriptDomain) {
            if (_.isFunction(scriptDomain)) {
                return scriptDomain.call(null, options) + scriptPath;
            }
            if (scriptDomain.match(/\{port\}/)) {
                return scriptDomain.replace("{port}", options.get("port")) + scriptPath;
            }
            return scriptDomain + scriptPath;
        }

        /**
         * Now if server or proxy, use dynamic script
         * eg:
         *  browser-sync start --server
         * ->
         *  "HOST:3000/browser-sync/browser-sync-client.js".replace("HOST", location.hostname)
         */
        if (options.get("server") || options.get("proxy")) {
            return scriptPath;
        }

        /**
         * Final use case is snippet mode
         * -> "http://HOST:3000/browser-sync/browser-sync-client.js".replace("HOST", location.hostname)
         * -> "//HOST:3000/browser-sync/browser-sync-client.js".replace("HOST", location.hostname)"
         */
        return getPath(options, scriptPath, options.get("port"));
    })();

    /**
     * Decide which template shall be used to generate the script tags
     */
    var template = (function () {
        if (scriptDomain || options.get("localOnly")) {
            return config.templates.scriptTagSimple;
        }
        return config.templates.scriptTag;
    })();

    /**
     * Finally read the template file from disk and replace
     * the dynamic values.
     */
    return fs.readFileSync(template, "utf8")
        .replace("%script%", scriptSrc)
        .replace("%async%", async ? "async" : "");
}
```
- example usage
```shell
...
 * @param {BrowserSync} bs
 * @param {Function} done
 */
setOptions: function (bs, done) {
    done(null, {
        options: {
            urls:        utils.getUrlOptions(bs.options),
            snippet:     connectUtils.scriptTags(bs.options),
            scriptPaths: Immutable.fromJS(connectUtils.clientScript(bs.options, true)),
            files:       bs.pluginManager.hook(
                "files:watch",
                bs.options.get("files"),
                bs.pluginManager.pluginOptions
            )
        }
...
```

#### <a name="apidoc.element.browser-sync.connect_utils.socketConnector"></a>[function <span class="apidocSignatureSpan">browser-sync.connect_utils.</span>socketConnector (options)](#apidoc.element.browser-sync.connect_utils.socketConnector)
- description and source-code
```javascript
socketConnector = function (options) {

    var socket        = options.get("socket");
    var template      = fs.readFileSync(config.templates.connector, "utf-8");
    var url           = connectUtils.getConnectionUrl(options);

<span class="apidocCodeCommentSpan">    /**
     * ***Backwards compatibility***. While 'socket.path' is technically a
     * socketIoClientConfig property, it's been documented previously
     * as a top-level option, so must stay.
     */
</span>    var clientConfig  = socket
        .get("socketIoClientConfig")
        .merge({
            path: socket.get("path")
        });

    template = template
        .replace("%config%", JSON.stringify(clientConfig.toJS()))
        .replace("%url%",  url);

    return template;
}
```
- example usage
```shell
...
/**
 * Get middleware
 * @returns {*}
 */
BrowserSync.prototype.getMiddleware = function (type) {

var types = {
    "connector": connectUtils.socketConnector(this.options),
    "socket-js": require("./snippet").utils.getSocketScript()
};

if (type in types) {
    return function (req, res) {
        res.setHeader("Content-Type", "text/javascript");
        res.end(types[type]);
...
```



# <a name="apidoc.module.browser-sync.file_event_handler"></a>[module browser-sync.file_event_handler](#apidoc.module.browser-sync.file_event_handler)

#### <a name="apidoc.element.browser-sync.file_event_handler.applyReloadOperators"></a>[function <span class="apidocSignatureSpan">browser-sync.file_event_handler.</span>applyReloadOperators (subject, options)](#apidoc.element.browser-sync.file_event_handler.applyReloadOperators)
- description and source-code
```javascript
function applyReloadOperators(subject, options) {
    var operators = [
        {
            option: "reloadDebounce",
            fnName: "debounce"
        },
        {
            option: "reloadThrottle",
            fnName: "throttle"
        },
        {
            option: "reloadDelay",
            fnName: "delay"
        }
    ];

    return applyOperators(operators, subject, options, options.getIn(["debug", "scheduler"]));
}
```
- example usage
```shell
...
    }
};

Object.keys(events).forEach(function (event) {
    bs.events.on(event, events[event]);
});

var reloader = fileHandler.applyReloadOperators(fromEvent(bs.events, "_browser:reload"), bs.options)
    .subscribe(function() {
        bs.events.emit("browser:reload");
    });

var coreNamespacedWatchers = fromEvent(bs.events, "file:changed")
    .filter(function() { return bs.options.get("codeSync") })
    .filter(function(x) { return  x.namespace === "core" });
...
```

#### <a name="apidoc.element.browser-sync.file_event_handler.fileChanges"></a>[function <span class="apidocSignatureSpan">browser-sync.file_event_handler.</span>fileChanges (subject, options)](#apidoc.element.browser-sync.file_event_handler.fileChanges)
- description and source-code
```javascript
function fileChanges(subject, options) {
    var operators = [
        {
            option: "reloadThrottle",
            fnName: "throttle"
        },
        {
            option: "reloadDelay",
            fnName: "delay"
        }
    ];

    var scheduler = options.getIn(["debug", "scheduler"]);

<span class="apidocCodeCommentSpan">    /**
     * if the 'reloadDebounce' option was provided, create
     * a stream buffered/debounced stream of events
     */
</span>    var initial = (function() {
        if (options.get("reloadDebounce") > 0) {
            return getAggregatedDebouncedStream(subject, options, scheduler);
        }
        return subject;
    })();

    return applyOperators(operators, initial, options, scheduler)
        .map(function(xs) {

            var items = [].concat(xs);
            var paths = items.map(function (x) { return x.path });

            if (utils.willCauseReload(paths, options.get("injectFileTypes").toJS())) {
                return {
                    type: "reload",
                    files: items
                }
            }
            return {
                type: "inject",
                files: items
            }
        });
}
```
- example usage
```shell
...
        bs.events.emit("browser:reload");
    });

var coreNamespacedWatchers = fromEvent(bs.events, "file:changed")
    .filter(function() { return bs.options.get("codeSync") })
    .filter(function(x) { return  x.namespace === "core" });

var handler = fileHandler.fileChanges(coreNamespacedWatchers, bs.options)
    .subscribe(function (x) {
        if (x.type === "reload") {
            bs.events.emit("browser:reload");
        }
        if (x.type === "inject") {
            x.files.forEach(function(data) {
                if (!bs.paused && data.namespace === "core") {
...
```



# <a name="apidoc.module.browser-sync.file_utils"></a>[module browser-sync.file_utils](#apidoc.module.browser-sync.file_utils)

#### <a name="apidoc.element.browser-sync.file_utils.changedFile"></a>[function <span class="apidocSignatureSpan">browser-sync.file_utils.</span>changedFile (bs, data)](#apidoc.element.browser-sync.file_utils.changedFile)
- description and source-code
```javascript
changedFile = function (bs, data) {
<span class="apidocCodeCommentSpan">    /**
     * If the event property is undefined, infer that it's a 'change'
     * event due the fact this handler is for emitter.emit("file:changed")
     */
</span>    if (_.isUndefined(data.event)) {
        data.event = "change";
    }
    /**
     * Chokidar always sends an 'event' property - which could be
     * 'add' 'unlink' etc etc so we need to check for that and only
     * respond to 'change', for now.
     */
    if (bs.options.get("watchEvents").indexOf(data.event) > -1) {
        if (!bs.paused && data.namespace === "core") {
            bs.events.emit("file:reload", fileUtils.getFileInfo(data, bs.options));
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.file_utils.getFileInfo"></a>[function <span class="apidocSignatureSpan">browser-sync.file_utils.</span>getFileInfo (data, options)](#apidoc.element.browser-sync.file_utils.getFileInfo)
- description and source-code
```javascript
getFileInfo = function (data, options) {

    data.ext      = require("path").extname(data.path).slice(1);
    data.basename = require("path").basename(data.path);

    var obj = {
        ext:           data.ext,
        path:          data.path,
        basename:      data.basename,
        event:         data.event,
        type:          "inject"
    };

    // RELOAD page
    if (!_.includes(options.get("injectFileTypes").toJS(), obj.ext)) {
        obj.url  = obj.path;
        obj.type = "reload";
    }

    obj.path = data.path;
    obj.log  = data.log;

    return obj;
}
```
- example usage
```shell
...
    /**
     * Chokidar always sends an 'event' property - which could be
     * 'add' 'unlink' etc etc so we need to check for that and only
     * respond to 'change', for now.
     */
    if (bs.options.get("watchEvents").indexOf(data.event) > -1) {
        if (!bs.paused && data.namespace === "core") {
            bs.events.emit("file:reload", fileUtils.getFileInfo(data, bs.options));
        }
    }
},
/**
 * @param data
 * @param options
 * @returns {{assetFileName: *, fileExtension: String}}
...
```



# <a name="apidoc.module.browser-sync.file_watcher"></a>[module browser-sync.file_watcher](#apidoc.module.browser-sync.file_watcher)

#### <a name="apidoc.element.browser-sync.file_watcher.plugin"></a>[function <span class="apidocSignatureSpan">browser-sync.file_watcher.</span>plugin (bs)](#apidoc.element.browser-sync.file_watcher.plugin)
- description and source-code
```javascript
plugin = function (bs) {

    var options = bs.options;
    var emitter = bs.emitter;

    var defaultWatchOptions = options.get("watchOptions").toJS();

    return options.get("files").reduce(function (map, glob, namespace) {

<span class="apidocCodeCommentSpan">        /**
         * Default CB when not given
         * @param event
         * @param path
         */
</span>        var fn = function (event, path) {
            emitter.emit("file:changed", {
                event: event,
                path: path,
                namespace: namespace
            });
        };

        var jsItem = glob.toJS();

        if (jsItem.globs.length) {
            var watcher = watch(jsItem.globs, defaultWatchOptions, fn);
            map[namespace] = {
                watchers: [watcher]
            };
        }

        if (jsItem.objs.length) {
            jsItem.objs.forEach(function (item) {
                if (!_.isFunction(item.fn)) {
                    item.fn = fn;
                }
                var watcher = watch(item.match, item.options || defaultWatchOptions, item.fn.bind(bs.publicInstance));
                if (!map[namespace]) {
                    map[namespace] = {
                        watchers: [watcher]
                    };
                } else {
                    map[namespace].watchers.push(watcher);
                }
            });
        }

        return map;

    }, {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.file_watcher.watch"></a>[function <span class="apidocSignatureSpan">browser-sync.file_watcher.</span>watch (patterns, opts, cb)](#apidoc.element.browser-sync.file_watcher.watch)
- description and source-code
```javascript
function watch(patterns, opts, cb) {

    if (typeof opts === "function") {
        cb = opts;
        opts = {};
    }

    var watcher = require("chokidar")
        .watch(patterns, opts);

    if (_.isFunction(cb)) {
        watcher.on("all", cb);
    }

    return watcher;
}
```
- example usage
```shell
...

    if (typeof opts === "function") {
        cb = opts;
        opts = {};
    }

    var watcher = require("chokidar")
        .watch(patterns, opts);

    if (_.isFunction(cb)) {
        watcher.on("all", cb);
    }

    return watcher;
}
...
```



# <a name="apidoc.module.browser-sync.hooks"></a>[module browser-sync.hooks](#apidoc.module.browser-sync.hooks)



# <a name="apidoc.module.browser-sync.http_protocol"></a>[module browser-sync.http_protocol](#apidoc.module.browser-sync.http_protocol)

#### <a name="apidoc.element.browser-sync.http_protocol.getUrl"></a>[function <span class="apidocSignatureSpan">browser-sync.http_protocol.</span>getUrl (args, url)](#apidoc.element.browser-sync.http_protocol.getUrl)
- description and source-code
```javascript
getUrl = function (args, url) {
    return [
        url,
        require("./config").httpProtocol.path,
        "?",
        queryString.stringify(args)
    ].join("");
}
```
- example usage
```shell
...

var scheme = options.get("scheme");

var port   = options.get("port");
var urls   = {};

if (options.get("online") === false) {
    urls.local = utils.getUrl(scheme + "://localhost:" + port, options);
    return Immutable.fromJS(urls);
}

var external  = utils.xip(utils.getHostIp(options, devIp), options);
var localhost = "localhost";

if (options.get("xip")) {
...
```

#### <a name="apidoc.element.browser-sync.http_protocol.middleware"></a>[function <span class="apidocSignatureSpan">browser-sync.http_protocol.</span>middleware (bs)](#apidoc.element.browser-sync.http_protocol.middleware)
- description and source-code
```javascript
middleware = function (bs) {

    return function (req, res) {

        var params = queryString.parse(req.url.replace(/^.*\?/, ""));
        var output;

        if (!Object.keys(params).length) {
            output = [
                "Error: No Parameters were provided.",
                "Example: http://localhost:3000/__browser_sync__?method=reload&args=core.css"
            ];
            res.writeHead(500, {"Content-Type": "text/plain"});
            res.end(output.join("\n"));
            return;
        }

        try {

            require("./public/" + params.method)(bs.events).apply(null, [params.args]);

            output = [
                "Called public API method '.%s()'".replace("%s", params.method),
                "With args: " + JSON.stringify(params.args)
            ];

            res.end(output.join("\n"));

        } catch (e) {

            res.writeHead(404, {"Content-Type": "text/plain"});
            res.write("Public API method '" + params.method + "' not found.");
            res.end();

            return;
        }
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.logger"></a>[module browser-sync.logger](#apidoc.module.browser-sync.logger)

#### <a name="apidoc.element.browser-sync.logger.getLogger"></a>[function <span class="apidocSignatureSpan">browser-sync.logger.</span>getLogger (name)](#apidoc.element.browser-sync.logger.getLogger)
- description and source-code
```javascript
getLogger = function (name) {
    return logger.clone(function (config) {
        config.prefix = config.prefix + template.replace("%s", name);
        return config;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.logger.plugin"></a>[function <span class="apidocSignatureSpan">browser-sync.logger.</span>plugin (emitter, bs)](#apidoc.element.browser-sync.logger.plugin)
- description and source-code
```javascript
plugin = function (emitter, bs) {

    var logPrefix = bs.options.get("logPrefix");
    var logLevel  = bs.options.get("logLevel");

    // Should set logger level here!
    logger.setLevel(logLevel);

    if (logPrefix) {
        if (_.isFunction(logPrefix)) {
            logger.setPrefix(logPrefix);
        } else {
            logger.setPrefix(template.replace("%s", logPrefix));
        }
    }

    _.each(exports.callbacks, function (func, event) {
        emitter.on(event, func.bind(this, bs));
    });

    return logger;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.options"></a>[module browser-sync.options](#apidoc.module.browser-sync.options)

#### <a name="apidoc.element.browser-sync.options.update"></a>[function <span class="apidocSignatureSpan">browser-sync.options.</span>update (options)](#apidoc.element.browser-sync.options.update)
- description and source-code
```javascript
update = function (options) {

    return options.withMutations(function (item) {

        setMode(item);
        setScheme(item);
        setStartPath(item);
        setProxyWs(item);
        setServerOpts(item);
        setNamespace(item);
        fixSnippetOptions(item);
        fixRewriteRules(item);
        setMiddleware(item);
        setOpen(item);

        if (item.get("uiPort")) {
            item.setIn(["ui", "port"], item.get("uiPort"));
        }
    });
}
```
- example usage
```shell
...
bs._options = options;

/**
 * Set additional options that depend on what the
 * user may of provided
 * @type {Map}
 */
bs.options  = require("./options").update(options);

/**
 * Kick off default plugins.
 */
bs.pluginManager.init();

/**
...
```



# <a name="apidoc.module.browser-sync.plugins"></a>[module browser-sync.plugins](#apidoc.module.browser-sync.plugins)

#### <a name="apidoc.element.browser-sync.plugins.requirePlugin"></a>[function <span class="apidocSignatureSpan">browser-sync.plugins.</span>requirePlugin (item)](#apidoc.element.browser-sync.plugins.requirePlugin)
- description and source-code
```javascript
function requirePlugin(item) {

<span class="apidocCodeCommentSpan">    /**
     * if the "module" property already exists and
     * is not a string, then we bail and don't bother looking
     * for the file
     */
</span>    if (item.get("module") && typeof item.get("module") !== "string") {
        return item;
    }

    try {
        /**
         * Try a raw node require() call - this will be how
         * regular "npm installed" plugins wil work
         */
        var maybe = path.resolve(process.cwd(), "node_modules", item.get("name"));
        return item.set("module", require(maybe));
    } catch (e) {
        /**
         * If require threw an MODULE_NOT_FOUND error, try again
         * by resolving from cwd. This is needed since cli
         * users will not add ./ to the front of a path (which
         * node requires to resolve from cwd)
         */
        if (e.code === "MODULE_NOT_FOUND") {
            var maybe = path.resolve(process.cwd(), item.get("name"));
            if (fs.existsSync(maybe)) {
                return item.set("module", require(maybe));
            } else {
                /**
                 * Finally return a plugin that contains the error
                 * this will be picked up later and discarded
                 */
                return item.update("errors", function (errors) {
                    return errors.concat(e);
                });
            }
        }
        throw e;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.plugins.resolvePlugin"></a>[function <span class="apidocSignatureSpan">browser-sync.plugins.</span>resolvePlugin (item)](#apidoc.element.browser-sync.plugins.resolvePlugin)
- description and source-code
```javascript
function resolvePlugin(item) {

<span class="apidocCodeCommentSpan">    /**
     * Handle when string was given, such as plugins: ['bs-html-injector']
     */
</span>    if (typeof item === "string") {
        return getFromString(item);
    }

    if (!isMap(item)) {
        return new Plugin().mergeDeep({errors: [new Error("Plugin not supported in this format")]});
    }

    if (item.has("module")) {

        var nameOrObj = item.get("module");
        var options = item.get("options");

        /**
         * The 'module' key can be a string, this allows
         * inline plugin references, but with options
         * eg:
         *
         * bs.init({
         *     plugins: [
         *         {
         *             module: './myjs-file.js'
         *             options: {
         *                 files: "*.html"
         *             }
         *         }
         *     ]
         * });
         */
        if (typeof nameOrObj === "string") {
            return getFromString(nameOrObj)
                .mergeDeep({
                    options: options
                });
        }

        /**
         * If the plugin was given completely inline (because it needs options)
         * eg:
         *
         * bs.init({
         *     plugins: [
         *         {
         *             module: {
         *                 plugin: function() {
         *                     console.log('My plugin code')
         *                 }
         *             },
         *             options: {
         *                 files: "*.html"
         *             }
         *         }
         *     ]
         * })
         */
        if (Immutable.Map.isMap(nameOrObj)) {
            return new Plugin({
                module: nameOrObj,
                options: options
            });
        }
    }

    /**
     * If a module was given directly. For example, ater calling require.
     *
     * eg:
     *    var myplugin = require('./some-js');
     *    bs.init({plugins: [myplugin]});
     */
    if (item.has("plugin")) {
        return new Plugin({
            module: item
        })
    }

    /**
     * If we reach here, the plugin option was used incorrectly
     */
    return new Plugin().mergeDeep({errors: [new Error("Plugin was not configured correctly")]})
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.server"></a>[module browser-sync.server](#apidoc.module.browser-sync.server)

#### <a name="apidoc.element.browser-sync.server.createServer"></a>[function <span class="apidocSignatureSpan">browser-sync.server.</span>createServer (bs)](#apidoc.element.browser-sync.server.createServer)
- description and source-code
```javascript
function createServer(bs) {

    var proxy   = bs.options.get("proxy");
    var server  = bs.options.get("server");

    if (!proxy && !server) {
        return require("./snippet-server")(bs);
    }

    if (proxy) {
        return require("./proxy-server")(bs);
    }

    if (server) {
        return require("./static-server")(bs);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.server.plugin"></a>[function <span class="apidocSignatureSpan">browser-sync.server.</span>plugin (bs)](#apidoc.element.browser-sync.server.plugin)
- description and source-code
```javascript
plugin = function (bs) {

    var debug   = bs.debug;
    var proxy   = bs.options.get("proxy");
    var type    = bs.options.get("mode");

    var bsServer = createServer(bs);

    if (type === "server" || type === "snippet") {
        debug("Static Server running ({magenta:%s}) ...", bs.options.get("scheme"));
    }

    if (proxy) {
        debug("Proxy running, proxing: {magenta:%s}", proxy.get("target"));
    }

    if (bsServer) {

<span class="apidocCodeCommentSpan">        /**
         * Allow server to be destroyed gracefully
         */
</span>        enableDestroy(bsServer.server);

        /**
         * Listen on the available port
         */
        bsServer.server.listen(bs.options.get("port"));

        /**
         * Hack to deal with https://github.com/socketio/socket.io/issues/1602#issuecomment-224270022
         */
        bs.registerCleanupTask(function () {
            if (bs.io && bs.io.sockets) {
                setCloseReceived(bs.io.sockets);
            }
            if (bs.ui && bs.ui.socket) {
                setCloseReceived(bs.ui.socket);
            }
        });

        /**
         * Destroy the server on cleanup
         */
        bs.registerCleanupTask(function () {
            bsServer.server.destroy();
        });
    }

    function setCloseReceived(io) {
        Object.keys(io.sockets).forEach(function (key) {
            _.set(io.sockets[key], "conn.transport.socket._closeReceived", true);
        });
    }

    debug("Running mode: %s", type.toUpperCase());

    return {
        server: bsServer.server,
        app:    bsServer.app
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.sockets"></a>[module browser-sync.sockets](#apidoc.module.browser-sync.sockets)

#### <a name="apidoc.element.browser-sync.sockets.init"></a>[function <span class="apidocSignatureSpan">browser-sync.sockets.</span>init (server, clientEvents, bs)](#apidoc.element.browser-sync.sockets.init)
- description and source-code
```javascript
init = function (server, clientEvents, bs) {

    var emitter      = bs.events;

    var socketConfig = bs.options
        .get("socket")
        .toJS();

    if (bs.options.get("mode") === "proxy" && bs.options.getIn(["proxy", "ws"])) {
        server = utils.getServer(null, bs.options).server;
        server.listen(bs.options.getIn(["socket", "port"]));
        bs.registerCleanupTask(function () {
            server.close();
        });
    }

    var socketIoConfig  = socketConfig.socketIoOptions;
    socketIoConfig.path = socketConfig.path;

    var io = socket(server, socketIoConfig);

    // Override default namespace.
    io.sockets = io.of(socketConfig.namespace);

    io.set("heartbeat interval", socketConfig.clients.heartbeatTimeout);

    var steward  = new Steward(emitter);
    bs.registerCleanupTask(steward.destroy.bind(steward));

<span class="apidocCodeCommentSpan">    /**
     * Listen for new connections
     */
</span>    io.sockets.on("connection", handleConnection);

    /**
     * Handle each new connection
     * @param {Object} client
     */
    function handleConnection (client) {

        // set ghostmode callbacks
        if (bs.options.get("ghostMode")) {

            addGhostMode(client);
        }

        client.emit("connection", bs.options.toJS()); //todo - trim the amount of options sent to clients

        emitter.emit("client:connected", {
            ua: client.handshake.headers["user-agent"]
        });
    }

    /**
     * @param {string} event
     * @param {Socket.client} client
     * @param {Object} data
     */
    function handleClientEvent(event, client, data) {

        if (steward.valid(client.id)) {

            client.broadcast.emit(event, data);
        }
    }

    /**
     * @param client
     */
    function addGhostMode (client) {

        clientEvents.forEach(addEvent);

        function addEvent(event) {

            client.on(event, handleClientEvent.bind(null, event, client));
        }
    }

    return io;
}
```
- example usage
```shell
...
function initSingleton() {
var instance;
if (instances.length) {
    instance = instances.filter(function (item) {
        return item.name === "singleton";
    });
    if (instance.length) {
        logger.error("{yellow:You tried to start Browsersync twice!} To create multiple instances, use {cyan:browserSync.create().
init()");
        return instance;
    }
}
var args = Array.prototype.slice.call(arguments);
singleton = create("singleton", getSingletonEmitter());

if (singletonPlugins.length) {
...
```

#### <a name="apidoc.element.browser-sync.sockets.plugin"></a>[function <span class="apidocSignatureSpan">browser-sync.sockets.</span>plugin (server, clientEvents, bs)](#apidoc.element.browser-sync.sockets.plugin)
- description and source-code
```javascript
plugin = function (server, clientEvents, bs) {
    return exports.init(server, clientEvents, bs);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-sync.utils"></a>[module browser-sync.utils](#apidoc.module.browser-sync.utils)

#### <a name="apidoc.element.browser-sync.utils.UAParser"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>UAParser (uastring, extensions)](#apidoc.element.browser-sync.utils.UAParser)
- description and source-code
```javascript
UAParser = function (uastring, extensions) {

    if (!(this instanceof UAParser)) {
        return new UAParser(uastring, extensions).getResult();
    }

    var ua = uastring || ((window && window.navigator && window.navigator.userAgent) ? window.navigator.userAgent : EMPTY);
    var rgxmap = extensions ? util.extend(regexes, extensions) : regexes;

    this.getBrowser = function () {
        var browser = mapper.rgx.apply(this, rgxmap.browser);
        browser.major = util.major(browser.version);
        return browser;
    };
    this.getCPU = function () {
        return mapper.rgx.apply(this, rgxmap.cpu);
    };
    this.getDevice = function () {
        return mapper.rgx.apply(this, rgxmap.device);
    };
    this.getEngine = function () {
        return mapper.rgx.apply(this, rgxmap.engine);
    };
    this.getOS = function () {
        return mapper.rgx.apply(this, rgxmap.os);
    };
    this.getResult = function() {
        return {
            ua      : this.getUA(),
            browser : this.getBrowser(),
            engine  : this.getEngine(),
            os      : this.getOS(),
            device  : this.getDevice(),
            cpu     : this.getCPU()
        };
    };
    this.getUA = function () {
        return ua;
    };
    this.setUA = function (uastring) {
        ua = uastring;
        return this;
    };
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils._makeUrl"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>_makeUrl (scheme, host, port)](#apidoc.element.browser-sync.utils._makeUrl)
- description and source-code
```javascript
_makeUrl = function (scheme, host, port) {
    return scheme + "://" + host + ":" + port;
}
```
- example usage
```shell
...
     * @param {String} scheme
     * @param {Object} options
     * @returns {{local: string, external: string}}
     */
    getUrls: function (external, local, scheme, options) {

var urls = {
    local: utils.getUrl(utils._makeUrl(scheme, local, options.get("port")), options)
};

if (external !== local) {
    urls.external = utils.getUrl(utils._makeUrl(scheme, external, options.get("port")), options);
}

return urls;
...
```

#### <a name="apidoc.element.browser-sync.utils.arrayify"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>arrayify (incoming)](#apidoc.element.browser-sync.utils.arrayify)
- description and source-code
```javascript
arrayify = function (incoming) {
    if (List.isList(incoming)) {
        return incoming.toArray();
    }
    return [].concat(incoming).filter(Boolean);
}
```
- example usage
```shell
...

    if (rewriteRules) {
        rules = rules.concat(rewriteRules);
    }

    return {
        rules: rules,
        blacklist: utils.arrayify(options.get("blacklist")),
        whitelist: utils.arrayify(options.get("whitelist"))
    };
},
/**
 * @param {Object} req
 * @param {Array} [excludeList]
 * @returns {Object}
...
```

#### <a name="apidoc.element.browser-sync.utils.connect"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>connect ()](#apidoc.element.browser-sync.utils.connect)
- description and source-code
```javascript
function createServer() {
  function app(req, res, next){ app.handle(req, res, next); }
  merge(app, proto);
  merge(app, EventEmitter.prototype);
  app.route = '/';
  app.stack = [];
  return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils.defaultCallback"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>defaultCallback (err)](#apidoc.element.browser-sync.utils.defaultCallback)
- description and source-code
```javascript
defaultCallback = function (err) {
    if (err && err.message) {
        console.error(err.message);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils.eachSeries"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>eachSeries (arr, iterator, callback)](#apidoc.element.browser-sync.utils.eachSeries)
- description and source-code
```javascript
eachSeries = function (arr, iterator, callback) {
    callback = callback || function () {};
    var completed = 0;
    var iterate = function () {
        iterator(arr[completed], function (err) {
            if (err) {
                callback(err);
                callback = function () {};
            } else {
                ++completed;
                if (completed >= arr.length) {
                    callback();
                } else {
                    iterate();
                }
            }
        });
    };
    iterate();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils.easyExtender"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>easyExtender (plugins, hooks)](#apidoc.element.browser-sync.utils.easyExtender)
- description and source-code
```javascript
easyExtender = function (plugins, hooks) {

    this.plugins        = {};
    this.pluginOptions  = {};
    this.returnValues   = {};

    this.hooks          = hooks;
    this.defaultPlugins = plugins;

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils.fail"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>fail (kill, errMessage, cb)](#apidoc.element.browser-sync.utils.fail)
- description and source-code
```javascript
fail = function (kill, errMessage, cb) {
    if (kill) {
        if (_.isFunction(cb)) {
            if (errMessage.message) { // Is this an error object?
                cb(errMessage);
            } else {
                cb(new Error(errMessage));
            }
        }
        process.exit(1);
    }
}
```
- example usage
```shell
...
 * and keep incrementing until an available one is found.
 * @param {BrowserSync} bs
 * @param {Function} done
 */
getEmptyPort: function (bs, done) {
    utils.getPorts(bs.options, function (err, port) {
        if (err) {
            return utils.fail(true, err, bs.cb);
        }
        bs.debug("Found a free port: {magenta:%s", port);
        done(null, {
            options: {
                port: port
            }
        });
...
```

#### <a name="apidoc.element.browser-sync.utils.getConfigErrors"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getConfigErrors (options)](#apidoc.element.browser-sync.utils.getConfigErrors)
- description and source-code
```javascript
getConfigErrors = function (options) {

    var messages = require("./config").errors;

    var errors = [];

    if (options.get("server") && options.get("proxy")) {
        errors.push(messages["server+proxy"]);
    }

    return errors;
}
```
- example usage
```shell
...
    return errors;
},
/**
 * @param {Map} options
 * @param {Function} [cb]
 */
verifyConfig: function (options, cb) {
    var errors = utils.getConfigErrors(options);
    if (errors.length) {
        utils.fail(true, errors.join("\n"), cb);
        return false;
    }
    return true;
},
/**
...
```

#### <a name="apidoc.element.browser-sync.utils.getHostIp"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getHostIp (options, devIp)](#apidoc.element.browser-sync.utils.getHostIp)
- description and source-code
```javascript
getHostIp = function (options, devIp) {

    if (options) {
        var host = options.get("host");
        if (host && host !== "localhost") {
            return host;
        }
        if (options.get("detect") === false || !devIp.length) {
            return false;
        }
    }

    return devIp.length ? devIp[0] : false;
}
```
- example usage
```shell
...
var urls   = {};

if (options.get("online") === false) {
    urls.local = utils.getUrl(scheme + "://localhost:" + port, options);
    return Immutable.fromJS(urls);
}

var external  = utils.xip(utils.getHostIp(options, devIp), options);
var localhost = "localhost";

if (options.get("xip")) {
    localhost = "127.0.0.1";
}

localhost = utils.xip(localhost, options);
...
```

#### <a name="apidoc.element.browser-sync.utils.getPort"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getPort (port, max, cb)](#apidoc.element.browser-sync.utils.getPort)
- description and source-code
```javascript
getPort = function (port, max, cb) {
    portScanner.findAPortNotInUse(port, max, {
        host: "localhost",
        timeout: 1000
    }, cb);
}
```
- example usage
```shell
...
/**
 * Or use the user-defined socket.port option instead
 */
if (bs.options.hasIn(["socket", "port"])) {
    socketPort = bs.options.getIn(["socket", "port"]);
}

utils.getPort(socketPort, null, function (err, port) {
    if (err) {
        return utils.fail(true, err, bs.cb);
    }
    done(null, {
        optionsIn: [
            {
                path: ["socket", "port"],
...
```

#### <a name="apidoc.element.browser-sync.utils.getPorts"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getPorts (options, cb)](#apidoc.element.browser-sync.utils.getPorts)
- description and source-code
```javascript
getPorts = function (options, cb) {

    var port  = options.get("port");
    var ports = options.get("ports"); // backwards compatibility
    var max;

    if (ports) {
        port = ports.get("min");
        max  = ports.get("max") || null;
    }

    utils.getPort(port, max, cb);
}
```
- example usage
```shell
...
 * BrowserSync needs at least 1 free port.
 * It will check the one provided in config
 * and keep incrementing until an available one is found.
 * @param {BrowserSync} bs
 * @param {Function} done
 */
getEmptyPort: function (bs, done) {
    utils.getPorts(bs.options, function (err, port) {
        if (err) {
            return utils.fail(true, err, bs.cb);
        }
        bs.debug("Found a free port: {magenta:%s", port);
        done(null, {
            options: {
                port: port
...
```

#### <a name="apidoc.element.browser-sync.utils.getUaString"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUaString (ua)](#apidoc.element.browser-sync.utils.getUaString)
- description and source-code
```javascript
getUaString = function (ua) {
    return parser.setUA(ua).getBrowser();
}
```
- example usage
```shell
...
    /**
     * Client connected logging
     * @param {BrowserSync} bs
     * @param data
     */
    "client:connected": function (bs, data) {

var uaString = utils.getUaString(data.ua);
var msg = "{cyan:Browser Connected: {magenta:%s, version: %s}";
var method = "info";

if (!bs.options.get("logConnections")) {
    method = "debug";
}
...
```

#### <a name="apidoc.element.browser-sync.utils.getUrl"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrl (url, options)](#apidoc.element.browser-sync.utils.getUrl)
- description and source-code
```javascript
getUrl = function (url, options) {

    var prefix = "/";
    var startPath = options.get("startPath");

    if (startPath) {
        if (startPath.charAt(0) === "/") {
            prefix = "";
        }
        url = url + prefix + startPath;
    }

    return url;
}
```
- example usage
```shell
...

var scheme = options.get("scheme");

var port   = options.get("port");
var urls   = {};

if (options.get("online") === false) {
    urls.local = utils.getUrl(scheme + "://localhost:" + port, options);
    return Immutable.fromJS(urls);
}

var external  = utils.xip(utils.getHostIp(options, devIp), options);
var localhost = "localhost";

if (options.get("xip")) {
...
```

#### <a name="apidoc.element.browser-sync.utils.getUrlOptions"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrlOptions (options)](#apidoc.element.browser-sync.utils.getUrlOptions)
- description and source-code
```javascript
getUrlOptions = function (options) {

    var scheme = options.get("scheme");

    var port   = options.get("port");
    var urls   = {};

    if (options.get("online") === false) {
        urls.local = utils.getUrl(scheme + "://localhost:" + port, options);
        return Immutable.fromJS(urls);
    }

    var external  = utils.xip(utils.getHostIp(options, devIp), options);
    var localhost = "localhost";

    if (options.get("xip")) {
        localhost = "127.0.0.1";
    }

    localhost = utils.xip(localhost, options);

    return Immutable.fromJS(utils.getUrls(external, localhost, scheme, options));
}
```
- example usage
```shell
...
 *
 * @param {BrowserSync} bs
 * @param {Function} done
 */
setOptions: function (bs, done) {
    done(null, {
        options: {
            urls:        utils.getUrlOptions(bs.options),
            snippet:     connectUtils.scriptTags(bs.options),
            scriptPaths: Immutable.fromJS(connectUtils.clientScript(bs.options, true)),
            files:       bs.pluginManager.hook(
                "files:watch",
                bs.options.get("files"),
                bs.pluginManager.pluginOptions
            )
...
```

#### <a name="apidoc.element.browser-sync.utils.getUrls"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>getUrls (external, local, scheme, options)](#apidoc.element.browser-sync.utils.getUrls)
- description and source-code
```javascript
getUrls = function (external, local, scheme, options) {

    var urls = {
        local: utils.getUrl(utils._makeUrl(scheme, local, options.get("port")), options)
    };

    if (external !== local) {
        urls.external = utils.getUrl(utils._makeUrl(scheme, external, options.get("port")), options);
    }

    return urls;
}
```
- example usage
```shell
...

    if (options.get("xip")) {
        localhost = "127.0.0.1";
    }

    localhost = utils.xip(localhost, options);

    return Immutable.fromJS(utils.getUrls(external, localhost, scheme, options));
},
/**
 * Append a start path if given in options
 * @param {String} url
 * @param {Object} options
 * @returns {String}
 */
...
```

#### <a name="apidoc.element.browser-sync.utils.isList"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>isList (maybeList)](#apidoc.element.browser-sync.utils.isList)
- description and source-code
```javascript
function isList(maybeList) {
  return !!(maybeList && maybeList[IS_LIST_SENTINEL]);
}
```
- example usage
```shell
...
if (type === "server") {

    var baseDir = bs.options.getIn(["server", "baseDir"]);

    logUrls(bs.options.get("urls").toJS());

    if (baseDir) {
        if (utils.isList(baseDir)) {
            baseDir.forEach(serveFiles);
        } else {
            serveFiles(baseDir);
        }
    }
}
...
```

#### <a name="apidoc.element.browser-sync.utils.open"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>open (url, name, bs)](#apidoc.element.browser-sync.utils.open)
- description and source-code
```javascript
open = function (url, name, bs) {
    var options = (function () {
        if (_.isString(name)) {
            return {app: name};
        }
        if (Immutable.Map.isMap(name)) {
            return name.toJS();
        }
        return {};
    })();
    var opn = require("opn");
    opn(url, options).catch(function() {
        bs.events.emit("browser:error");
    });
}
```
- example usage
```shell
...
    }
}

if (open) {
    if (browser !== "default") {
        if (utils.isList(browser)) {
            browser.forEach(function (browser) {
                utils.open(url, browser, bs);
            });
        } else {
            utils.open(url, browser, bs); // single
        }
    } else {
        utils.open(url, null, bs);
    }
...
```

#### <a name="apidoc.element.browser-sync.utils.openBrowser"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>openBrowser (url, options, bs)](#apidoc.element.browser-sync.utils.openBrowser)
- description and source-code
```javascript
openBrowser = function (url, options, bs) {

    var open    = options.get("open");
    var browser = options.get("browser");

    if (_.isString(open)) {
        if (options.getIn(["urls", open])) {
            url = options.getIn(["urls", open]);
        }
    }

    if (open) {
        if (browser !== "default") {
            if (utils.isList(browser)) {
                browser.forEach(function (browser) {
                    utils.open(url, browser, bs);
                });
            } else {
                utils.open(url, browser, bs); // single
            }
        } else {
            utils.open(url, null, bs);
        }
    }
}
```
- example usage
```shell
...
 */
"service:running": function (data) {

    var mode = bs.options.get("mode");
    var open = bs.options.get("open");

    if (mode === "proxy" || mode === "server" || open === "ui" || open === "ui-external") {
        utils.openBrowser(data.url, bs.options, bs);
    }

    // log about any file watching
    if (bs.watchers) {
        bs.events.emit("file:watching", bs.watchers);
    }
},
...
```

#### <a name="apidoc.element.browser-sync.utils.serveStatic"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>serveStatic (root, options)](#apidoc.element.browser-sync.utils.serveStatic)
- description and source-code
```javascript
function serveStatic(root, options) {
  if (!root) {
    throw new TypeError('root path required')
  }

  if (typeof root !== 'string') {
    throw new TypeError('root path must be a string')
  }

  // copy options object
  var opts = Object.create(options || null)

  // fall-though
  var fallthrough = opts.fallthrough !== false

  // default redirect
  var redirect = opts.redirect !== false

  // headers listener
  var setHeaders = opts.setHeaders

  if (setHeaders && typeof setHeaders !== 'function') {
    throw new TypeError('option setHeaders must be function')
  }

  // setup options for send
  opts.maxage = opts.maxage || opts.maxAge || 0
  opts.root = resolve(root)

  // construct directory listener
  var onDirectory = redirect
    ? createRedirectDirectoryListener()
    : createNotFoundDirectoryListener()

  return function serveStatic (req, res, next) {
    if (req.method !== 'GET' && req.method !== 'HEAD') {
      if (fallthrough) {
        return next()
      }

      // method not allowed
      res.statusCode = 405
      res.setHeader('Allow', 'GET, HEAD')
      res.setHeader('Content-Length', '0')
      res.end()
      return
    }

    var forwardError = !fallthrough
    var originalUrl = parseUrl.original(req)
    var path = parseUrl(req).pathname

    // make sure redirect occurs at mount
    if (path === '/' && originalUrl.pathname.substr(-1) !== '/') {
      path = ''
    }

    // create send stream
    var stream = send(req, path, opts)

    // add directory handler
    stream.on('directory', onDirectory)

    // add headers listener
    if (setHeaders) {
      stream.on('headers', setHeaders)
    }

    // add file listener for fallthrough
    if (fallthrough) {
      stream.on('file', function onFile () {
        // once file is determined, always forward error
        forwardError = true
      })
    }

    // forward errors
    stream.on('error', function error (err) {
      if (forwardError || !(err.statusCode < 500)) {
        next(err)
        return
      }

      next()
    })

    // pipe
    stream.pipe(res)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-sync.utils.verifyConfig"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>verifyConfig (options, cb)](#apidoc.element.browser-sync.utils.verifyConfig)
- description and source-code
```javascript
verifyConfig = function (options, cb) {
    var errors = utils.getConfigErrors(options);
    if (errors.length) {
        utils.fail(true, errors.join("\n"), cb);
        return false;
    }
    return true;
}
```
- example usage
```shell
...
bs.cb  = cb || utils.defaultCallback;

/**
 * Verify provided config.
 * Some options are not compatible and will cause us to
 * end the process.
 */
if (!utils.verifyConfig(options, bs.cb)) {
    return;
}

/**
 * Save a reference to the original options
 * @type {Map}
 * @private
...
```

#### <a name="apidoc.element.browser-sync.utils.willCauseReload"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>willCauseReload (needles, haystack)](#apidoc.element.browser-sync.utils.willCauseReload)
- description and source-code
```javascript
willCauseReload = function (needles, haystack) {
    return needles.some(function (needle) {
        return !_.includes(haystack, path.extname(needle).replace(".", ""));
    });
}
```
- example usage
```shell
...

    return applyOperators(operators, initial, options, scheduler)
        .map(function(xs) {

var items = [].concat(xs);
var paths = items.map(function (x) { return x.path });

if (utils.willCauseReload(paths, options.get("injectFileTypes").toJS())) {
    return {
        type: "reload",
        files: items
    }
}
return {
    type: "inject",
...
```

#### <a name="apidoc.element.browser-sync.utils.xip"></a>[function <span class="apidocSignatureSpan">browser-sync.utils.</span>xip (host, options)](#apidoc.element.browser-sync.utils.xip)
- description and source-code
```javascript
xip = function (host, options) {
    var suffix = options.get("hostnameSuffix");
    if (options.get("xip")) {
        return host + ".xip.io";
    }
    if (suffix) {
        return host + suffix;
    }
    return host;
}
```
- example usage
```shell
...
var urls   = {};

if (options.get("online") === false) {
    urls.local = utils.getUrl(scheme + "://localhost:" + port, options);
    return Immutable.fromJS(urls);
}

var external  = utils.xip(utils.getHostIp(options, devIp), options);
var localhost = "localhost";

if (options.get("xip")) {
    localhost = "127.0.0.1";
}

localhost = utils.xip(localhost, options);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
