# api documentation for  [electrolyte (v0.4.0)](https://github.com/jaredhanson/electrolyte#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-electrolyte.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electrolyte) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electrolyte.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electrolyte)
#### Elegant dependency injection for Node.js.

[![NPM](https://nodei.co/npm/electrolyte.png?downloads=true)](https://www.npmjs.com/package/electrolyte)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electrolyte/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-electrolyte_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electrolyte/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electrolyte/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electrolyte/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "email": "jaredhanson@gmail.com",
        "url": "http://www.jaredhanson.net/"
    },
    "bugs": {
        "url": "http://github.com/jaredhanson/electrolyte/issues"
    },
    "contributors": [
        {
            "name": "Jeremie Miller",
            "email": "jeremie.miller@gmail.com",
            "url": "http://jeremie.com"
        }
    ],
    "dependencies": {
        "canonical-path": "0.0.2",
        "debug": "^2.2.0",
        "depd": "^1.0.1",
        "promise": "^7.1.1",
        "scripts": "0.1.x"
    },
    "description": "Elegant dependency injection for Node.js.",
    "devDependencies": {
        "chai": "3.x.x",
        "chai-express-handler": "git://github.com/jaredhanson/chai-express-handler.git",
        "make-node": "0.3.x",
        "mocha": "2.x.x",
        "sinon": "^1.17.4",
        "sinon-chai": "^2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "332dd574d628dd53c1a1f765cc70e016b84decb1",
        "tarball": "https://registry.npmjs.org/electrolyte/-/electrolyte-0.4.0.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "548b5ea846ee4ef2406163fde57a3c46d2a776e4",
    "homepage": "https://github.com/jaredhanson/electrolyte#readme",
    "keywords": [
        "require",
        "dependency",
        "dependencies",
        "injection",
        "di",
        "ioc"
    ],
    "license": "MIT",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://opensource.org/licenses/MIT"
        }
    ],
    "main": "./lib",
    "maintainers": [
        {
            "name": "jaredhanson",
            "email": "jaredhanson@gmail.com"
        }
    ],
    "name": "electrolyte",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jaredhanson/electrolyte.git"
    },
    "scripts": {
        "test": "mocha --reporter spec --require test/bootstrap/node test/*.test.js test/**/*.test.js"
    },
    "version": "0.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module electrolyte](#apidoc.module.electrolyte)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>Container ()](#apidoc.element.electrolyte.Container)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>dir (options)](#apidoc.element.electrolyte.dir)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>fs (options)](#apidoc.element.electrolyte.fs)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>injectedcontainer (c, spec, ns)](#apidoc.element.electrolyte.injectedcontainer)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>node (arg0)](#apidoc.element.electrolyte.node)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>node_modules ()](#apidoc.element.electrolyte.node_modules)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>spec (id, mod, source)](#apidoc.element.electrolyte.spec)
1.  number <span class="apidocSignatureSpan">electrolyte.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">electrolyte.</span>Container.prototype
1.  object <span class="apidocSignatureSpan">electrolyte.</span>_events
1.  object <span class="apidocSignatureSpan">electrolyte.</span>_order
1.  object <span class="apidocSignatureSpan">electrolyte.</span>_resolvers
1.  object <span class="apidocSignatureSpan">electrolyte.</span>_sources
1.  object <span class="apidocSignatureSpan">electrolyte.</span>_specs
1.  object <span class="apidocSignatureSpan">electrolyte.</span>domain
1.  object <span class="apidocSignatureSpan">electrolyte.</span>injectedcontainer.prototype
1.  object <span class="apidocSignatureSpan">electrolyte.</span>spec.prototype

#### [module electrolyte.Container](#apidoc.module.electrolyte.Container)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>Container ()](#apidoc.element.electrolyte.Container.Container)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.</span>super_ ()](#apidoc.element.electrolyte.Container.super_)

#### [module electrolyte.Container.prototype](#apidoc.module.electrolyte.Container.prototype)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_create (id, parent)](#apidoc.element.electrolyte.Container.prototype._create)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_loadSpec (id, cb)](#apidoc.element.electrolyte.Container.prototype._loadSpec)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_registerSpec (id, mod, source)](#apidoc.element.electrolyte.Container.prototype._registerSpec)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>create (id, parent)](#apidoc.element.electrolyte.Container.prototype.create)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>loader (arg0, arg1, arg2)](#apidoc.element.electrolyte.Container.prototype.loader)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>resolve (id, parent)](#apidoc.element.electrolyte.Container.prototype.resolve)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>resolver (fn)](#apidoc.element.electrolyte.Container.prototype.resolver)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>specs ()](#apidoc.element.electrolyte.Container.prototype.specs)
1.  [function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>use (ns, s, options)](#apidoc.element.electrolyte.Container.prototype.use)

#### [module electrolyte._resolvers](#apidoc.module.electrolyte._resolvers)
1.  [function <span class="apidocSignatureSpan">electrolyte._resolvers.</span>0 (id)](#apidoc.element.electrolyte._resolvers.0)

#### [module electrolyte.injectedcontainer](#apidoc.module.electrolyte.injectedcontainer)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>injectedcontainer (c, spec, ns)](#apidoc.element.electrolyte.injectedcontainer.injectedcontainer)

#### [module electrolyte.injectedcontainer.prototype](#apidoc.module.electrolyte.injectedcontainer.prototype)
1.  [function <span class="apidocSignatureSpan">electrolyte.injectedcontainer.prototype.</span>create (id)](#apidoc.element.electrolyte.injectedcontainer.prototype.create)
1.  [function <span class="apidocSignatureSpan">electrolyte.injectedcontainer.prototype.</span>specs (q)](#apidoc.element.electrolyte.injectedcontainer.prototype.specs)

#### [module electrolyte.spec](#apidoc.module.electrolyte.spec)
1.  [function <span class="apidocSignatureSpan">electrolyte.</span>spec (id, mod, source)](#apidoc.element.electrolyte.spec.spec)

#### [module electrolyte.spec.prototype](#apidoc.module.electrolyte.spec.prototype)
1.  [function <span class="apidocSignatureSpan">electrolyte.spec.prototype.</span>create (container)](#apidoc.element.electrolyte.spec.prototype.create)
1.  [function <span class="apidocSignatureSpan">electrolyte.spec.prototype.</span>instantiate ()](#apidoc.element.electrolyte.spec.prototype.instantiate)



# <a name="apidoc.module.electrolyte"></a>[module electrolyte](#apidoc.module.electrolyte)

#### <a name="apidoc.element.electrolyte.Container"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>Container ()](#apidoc.element.electrolyte.Container)
- description and source-code
```javascript
function Container() {
  EventEmitter.call(this);
  this._specs = {};
  this._sources = {};
  this._order = [];
  this._resolvers = [];

  this.resolver(require('./resolvers/id')());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.dir"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>dir (options)](#apidoc.element.electrolyte.dir)
- description and source-code
```javascript
dir = function (options) {
  if ('string' == typeof options) {
    options = { dirname: options }
  }
  options = options || {};
  var dirname = options.dirname || 'app'
    , extensions = options.extensions
    , dir = path.resolve(dirname);

  return function app(id) {
    var aid = path.join(dir, id)
      , script = scripts.resolve(aid, extensions);

    if (!existsSync(script)) { return; }
    return require(script);
  };
}
```
- example usage
```shell
...
#### Configure the Loader

When a component is '@require''d by another component, Electrolyte will
automatically load and instantiate it.  The loader needs to be configured with
location where an application's components are found:

'''javascript
IoC.use(IoC.dir('app/components'));
'''

#### @require vs require()

Loading components is similar in many regards to 'require'ing a module, with
one primary difference: components have the ability to return an object that
is configured according to application-level or environment-specific settings.
...
```

#### <a name="apidoc.element.electrolyte.fs"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>fs (options)](#apidoc.element.electrolyte.fs)
- description and source-code
```javascript
fs = function (options) {
  if ('string' == typeof options) {
    options = { dirname: options }
  }
  options = options || {};
  var dirname = options.dirname || 'app'
    , extensions = options.extensions
    , dir = path.resolve(dirname);

  return function app(id) {
    var aid = path.join(dir, id)
      , script = scripts.resolve(aid, extensions);

    if (!existsSync(script)) { return; }
    return require(script);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.injectedcontainer"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>injectedcontainer (c, spec, ns)](#apidoc.element.electrolyte.injectedcontainer)
- description and source-code
```javascript
function InjectedContainer(c, spec, ns) {
  this._c = c;
  this._spec = spec;
  this._ns = ns || '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.node"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>node (arg0)](#apidoc.element.electrolyte.node)
- description and source-code
```javascript
node = function (arg0) {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.node_modules"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>node_modules ()](#apidoc.element.electrolyte.node_modules)
- description and source-code
```javascript
node_modules = function () {

  return function(id) {
    try {
      var module = require(id);
      module['@literal'] = true;
      return module;
    } catch (ex) {
      return;
    }
  };
}
```
- example usage
```shell
...
inject modules themselves.  This is typical with modules that provide
network-related functionality that needs to be mocked out in test environments.

Electrolyte can be configured to do this automatically, by configuring the loader
to inject modules:

'''javascript
IoC.use(IoC.node_modules());
''''

With that in place, the database component above can be re-written as follows:

'''javascript
exports = module.exports = function(mysql, settings) {
var connection = mysql.createConnection({
...
```

#### <a name="apidoc.element.electrolyte.spec"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>spec (id, mod, source)](#apidoc.element.electrolyte.spec)
- description and source-code
```javascript
function Spec(id, mod, source) {
  var keys, i, len;

  this.id = id;
  this.dependencies = mod['@require'] || [];
  this.singleton = mod['@singleton'];
  this.implements = mod['@implements'] || [];
  if (typeof this.implements == 'string') {
    this.implements = [ this.implements ]
  }
  this.a = {};

  if (typeof mod === 'object' || typeof mod === 'function') {
    keys = Object.keys(mod);
    for (i = 0, len = keys.length; i < len; ++i) {
      if (keys[i].indexOf('@') == 0) {
        this.a[keys[i]] = mod[keys[i]];
      }
    }
  }
  this._source = source;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electrolyte.Container"></a>[module electrolyte.Container](#apidoc.module.electrolyte.Container)

#### <a name="apidoc.element.electrolyte.Container.Container"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>Container ()](#apidoc.element.electrolyte.Container.Container)
- description and source-code
```javascript
function Container() {
  EventEmitter.call(this);
  this._specs = {};
  this._sources = {};
  this._order = [];
  this._resolvers = [];

  this.resolver(require('./resolvers/id')());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.super_"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.</span>super_ ()](#apidoc.element.electrolyte.Container.super_)
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



# <a name="apidoc.module.electrolyte.Container.prototype"></a>[module electrolyte.Container.prototype](#apidoc.module.electrolyte.Container.prototype)

#### <a name="apidoc.element.electrolyte.Container.prototype._create"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_create (id, parent)](#apidoc.element.electrolyte.Container.prototype._create)
- description and source-code
```javascript
_create = function (id, parent) {
  var psource = parent ? parent._source : undefined;

  // built-ins
  switch (id) {
  case '!container':
    return Promise.resolve(new InjectedContainer(this, parent, psource && psource.namespace));
  }

  return new Promise(function(resolve, reject) {
    if (parent && id[0] == '.') {
      // resolve relative component ID
      id = path.join(path.dirname(parent.id), id);
    }
    id = this.resolve(id, parent);

    var spec = this._specs[id];
    if (spec) {
      return resolve(spec.create(this));
    } else {
      var self = this;
      this._loadSpec(id, function(err, spec) {
        if (err && err.code == 'SPEC_NOT_FOUND') {
          reject(new Error('Unable to create object "' + id + '" required by: ' + (parent && parent.id || 'unknown')));
        } else if (err) {
          return reject(err);
        }
        resolve(spec.create(self))
      });
    }
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype._loadSpec"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_loadSpec (id, cb)](#apidoc.element.electrolyte.Container.prototype._loadSpec)
- description and source-code
```javascript
_loadSpec = function (id, cb) {
  debug('autoload %s', id);
  var order = this._order
    , source, mod, rid
    , i, len;

  for (i = 0, len = order.length; i < len; ++i) {
    source = this._sources[order[i]];
    rid = path.relative(source.namespace, id);
    if (rid.indexOf('../') == 0) { continue; }
    mod = source.load(rid);

    if (mod) {
      spec = this._registerSpec(id, mod, source);
      return cb(null, spec);
    }
  }
  return cb(new SpecNotFoundError('Cannot find spec "' + id + '"'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype._registerSpec"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>_registerSpec (id, mod, source)](#apidoc.element.electrolyte.Container.prototype._registerSpec)
- description and source-code
```javascript
_registerSpec = function (id, mod, source) {
  var spec, pattern;

  if (mod['@literal']) {
    pattern = 'literal';
  } else if (typeof mod == 'function') {
    // The module exports a function.  If the function name begins with a
    // capital letter, it will be treated as a constructor.  Otherwise, it will
    // be treated as a factory function;
    var name = mod.name || 'anonymous';
    if (name[0] == name[0].toUpperCase()) {
      pattern = 'constructor';
    } else {
      pattern = 'factory';
    }
  }

  switch (pattern) {
  case 'factory':
    debug('register factory %s', id);
    spec = new FactorySpec(id, mod, source);
    break;
  case 'constructor':
    debug('register constructor %s', id);
    spec = new ConstructorSpec(id, mod, source);
    break;
  case 'literal':
  default:
    debug('register literal %s', id);
    spec = new LiteralSpec(id, mod, source);
    break;
  }

  this._specs[spec.id] = spec;
  return spec;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype.create"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>create (id, parent)](#apidoc.element.electrolyte.Container.prototype.create)
- description and source-code
```javascript
create = function (id, parent) {
  return this._create(id, parent);
}
```
- example usage
```shell
...
#### Creating Components

Components are created by asking the IoC container to create them:

'''javascript
var IoC = require('electrolyte');

var db = IoC.create('database');
'''

Electrolyte is smart enough to automatically traverse a component's dependencies
(and dependencies of dependencies, and so on), correctly wiring together the
complete object structure.

In the case of the database above, Electrolyte would first initialize the
...
```

#### <a name="apidoc.element.electrolyte.Container.prototype.loader"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>loader (arg0, arg1, arg2)](#apidoc.element.electrolyte.Container.prototype.loader)
- description and source-code
```javascript
loader = function (arg0, arg1, arg2) {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype.resolve"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>resolve (id, parent)](#apidoc.element.electrolyte.Container.prototype.resolve)
- description and source-code
```javascript
resolve = function (id, parent) {
  var resolvers = this._resolvers
    , fn, rid, i, len;
  for (i = 0, len = resolvers.length; i < len; ++i) {
    fn = resolvers[i];
    rid = fn(id, parent && parent.id);
    if (rid) { return rid; }
  }
  throw new Error('Unable to resolve interface "' + id + '" required by: ' + (parent && parent.id || 'unknown'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype.resolver"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>resolver (fn)](#apidoc.element.electrolyte.Container.prototype.resolver)
- description and source-code
```javascript
resolver = function (fn) {
  this._resolvers.push(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electrolyte.Container.prototype.specs"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>specs ()](#apidoc.element.electrolyte.Container.prototype.specs)
- description and source-code
```javascript
specs = function () {
  // TODO: Wrap specs so they can be created in an optimzied way

  var ids = Object.keys(this._specs)
    , specs = []
    , i, len;
  for (i = 0, len = ids.length; i < len; ++i) {
    specs.push(this._specs[ids[i]]);
  }
  return specs;
}
```
- example usage
```shell
...
InjectedContainer.prototype.specs = function(q) {
if (q && !Array.isArray(q)) {
  q = [ q ];
}

// Filter the exposed specs to only those that exist within the namespace
// of the object being created.
var specs = this._c.specs()
  , exposed = []
  , spec, rid, i, len;
for (i = 0, len = specs.length; i < len; ++i) {
  spec = specs[i];
  rid = path.relative(this._ns, spec.id);
  if (rid.indexOf('../') == 0) { continue; }
  if (!q) {
...
```

#### <a name="apidoc.element.electrolyte.Container.prototype.use"></a>[function <span class="apidocSignatureSpan">electrolyte.Container.prototype.</span>use (ns, s, options)](#apidoc.element.electrolyte.Container.prototype.use)
- description and source-code
```javascript
use = function (ns, s, options) {
  if (typeof ns !== 'string') {
    options = s;
    s = ns;
    ns = '';
  }
  options = options || {};

  var load = s
    , manifest = {}
    , ids, aid, spec, i, len;

  if (typeof s == 'object') {
    manifest = s;
    load = s.load || function noop(id) { return; };
  }

  if (typeof load != 'function') {
    throw new Error("Container#use requires a load function, was passed a '" + (typeof load) + "'");
  }

  var h = this._order.length;
  var source = { namespace: ns, load: load };
  this._sources[h] = source;
  this._order.unshift(h);

  ids = Object.keys(manifest);
  for (i = 0, len = ids.length; i < len; ++i) {
    aid = path.join(source.namespace, ids[i]);
    spec = manifest[ids[i]];
    if (spec === load) { continue; }
    this._registerSpec(aid, spec, source);
  }

  return this;
}
```
- example usage
```shell
...
#### Configure the Loader

When a component is '@require''d by another component, Electrolyte will
automatically load and instantiate it.  The loader needs to be configured with
location where an application's components are found:

'''javascript
IoC.use(IoC.dir('app/components'));
'''

#### @require vs require()

Loading components is similar in many regards to 'require'ing a module, with
one primary difference: components have the ability to return an object that
is configured according to application-level or environment-specific settings.
...
```



# <a name="apidoc.module.electrolyte._resolvers"></a>[module electrolyte._resolvers](#apidoc.module.electrolyte._resolvers)

#### <a name="apidoc.element.electrolyte._resolvers.0"></a>[function <span class="apidocSignatureSpan">electrolyte._resolvers.</span>0 (id)](#apidoc.element.electrolyte._resolvers.0)
- description and source-code
```javascript
0 = function (id) {
  if (/^[\w\-\.\/]+$/.test(id)) {
    return id;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electrolyte.injectedcontainer"></a>[module electrolyte.injectedcontainer](#apidoc.module.electrolyte.injectedcontainer)

#### <a name="apidoc.element.electrolyte.injectedcontainer.injectedcontainer"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>injectedcontainer (c, spec, ns)](#apidoc.element.electrolyte.injectedcontainer.injectedcontainer)
- description and source-code
```javascript
function InjectedContainer(c, spec, ns) {
  this._c = c;
  this._spec = spec;
  this._ns = ns || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electrolyte.injectedcontainer.prototype"></a>[module electrolyte.injectedcontainer.prototype](#apidoc.module.electrolyte.injectedcontainer.prototype)

#### <a name="apidoc.element.electrolyte.injectedcontainer.prototype.create"></a>[function <span class="apidocSignatureSpan">electrolyte.injectedcontainer.prototype.</span>create (id)](#apidoc.element.electrolyte.injectedcontainer.prototype.create)
- description and source-code
```javascript
create = function (id) {
  var aid = path.join(this._ns, id);
  var rid = path.relative(this._ns, aid);
  if (rid.indexOf('../') == 0) {
    return Promise.reject(new Error(id + ' not within namespace'));
  }

  return this._c.create(aid, this._spec);
}
```
- example usage
```shell
...
#### Creating Components

Components are created by asking the IoC container to create them:

'''javascript
var IoC = require('electrolyte');

var db = IoC.create('database');
'''

Electrolyte is smart enough to automatically traverse a component's dependencies
(and dependencies of dependencies, and so on), correctly wiring together the
complete object structure.

In the case of the database above, Electrolyte would first initialize the
...
```

#### <a name="apidoc.element.electrolyte.injectedcontainer.prototype.specs"></a>[function <span class="apidocSignatureSpan">electrolyte.injectedcontainer.prototype.</span>specs (q)](#apidoc.element.electrolyte.injectedcontainer.prototype.specs)
- description and source-code
```javascript
specs = function (q) {
  if (q && !Array.isArray(q)) {
    q = [ q ];
  }

  // Filter the exposed specs to only those that exist within the namespace
  // of the object being created.
  var specs = this._c.specs()
    , exposed = []
    , spec, rid, i, len;
  for (i = 0, len = specs.length; i < len; ++i) {
    spec = specs[i];
    rid = path.relative(this._ns, spec.id);
    if (rid.indexOf('../') == 0) { continue; }
    if (!q) {
      exposed.push(new ExposedSpec(rid, spec));
    } else if (spec.implements.some(function(i) { return i == q })) {
      // The spec implements one of the requested interfaces.
      exposed.push(new ExposedSpec(rid, spec));
    }
  }
  return exposed;
}
```
- example usage
```shell
...
InjectedContainer.prototype.specs = function(q) {
if (q && !Array.isArray(q)) {
  q = [ q ];
}

// Filter the exposed specs to only those that exist within the namespace
// of the object being created.
var specs = this._c.specs()
  , exposed = []
  , spec, rid, i, len;
for (i = 0, len = specs.length; i < len; ++i) {
  spec = specs[i];
  rid = path.relative(this._ns, spec.id);
  if (rid.indexOf('../') == 0) { continue; }
  if (!q) {
...
```



# <a name="apidoc.module.electrolyte.spec"></a>[module electrolyte.spec](#apidoc.module.electrolyte.spec)

#### <a name="apidoc.element.electrolyte.spec.spec"></a>[function <span class="apidocSignatureSpan">electrolyte.</span>spec (id, mod, source)](#apidoc.element.electrolyte.spec.spec)
- description and source-code
```javascript
function Spec(id, mod, source) {
  var keys, i, len;

  this.id = id;
  this.dependencies = mod['@require'] || [];
  this.singleton = mod['@singleton'];
  this.implements = mod['@implements'] || [];
  if (typeof this.implements == 'string') {
    this.implements = [ this.implements ]
  }
  this.a = {};

  if (typeof mod === 'object' || typeof mod === 'function') {
    keys = Object.keys(mod);
    for (i = 0, len = keys.length; i < len; ++i) {
      if (keys[i].indexOf('@') == 0) {
        this.a[keys[i]] = mod[keys[i]];
      }
    }
  }
  this._source = source;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electrolyte.spec.prototype"></a>[module electrolyte.spec.prototype](#apidoc.module.electrolyte.spec.prototype)

#### <a name="apidoc.element.electrolyte.spec.prototype.create"></a>[function <span class="apidocSignatureSpan">electrolyte.spec.prototype.</span>create (container)](#apidoc.element.electrolyte.spec.prototype.create)
- description and source-code
```javascript
create = function (container) {
  debug('create %s', this.id);

  // Immediately return cached instance.  Optimization for singleton and literal
  // components.
  if (this._instance) { return this._instance; }

  // Create an array of promises which, once resolved, will be an array of
  // objects that are dependencies of the object being created.
  var deps = this.dependencies
    , promises = []
    , promise, p;
  for (var i = 0, len = deps.length; i < len; ++i) {
    promise = container.create(deps[i], this);
    promises.push(promise);
  }

  // Resolve all the promises, and then instantiate the object with its
  // dependencies.
  p = Promise.all(promises)
    .then(function(args) {
      var i = this.instantiate.apply(this, args);
      container.emit('create', i, this);

      // Once the promise has been resolved, cache the object instance if the
      // spec was annotated as being a singleton.
      if (this.singleton) { this._instance = i; }
      return i;
    }.bind(this));

  // Cache the promise if the spec was annotated as being a singleton.  This
  // ensures that a singleton object is resolved, if the object is created
  // multiple times while waiting for resolution.  Upon the promise being
  // resolved, the created object will be cached.
  if (this.singleton) { this._instance = p; }
  return p;
}
```
- example usage
```shell
...
#### Creating Components

Components are created by asking the IoC container to create them:

'''javascript
var IoC = require('electrolyte');

var db = IoC.create('database');
'''

Electrolyte is smart enough to automatically traverse a component's dependencies
(and dependencies of dependencies, and so on), correctly wiring together the
complete object structure.

In the case of the database above, Electrolyte would first initialize the
...
```

#### <a name="apidoc.element.electrolyte.spec.prototype.instantiate"></a>[function <span class="apidocSignatureSpan">electrolyte.spec.prototype.</span>instantiate ()](#apidoc.element.electrolyte.spec.prototype.instantiate)
- description and source-code
```javascript
instantiate = function () {
  throw new Error("Spec#instantiate must be overridden by subclass");
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
