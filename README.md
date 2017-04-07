# api documentation for  [validatorjs (v3.11.0)](https://github.com/skaterdav85/validatorjs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-validatorjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-validatorjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-validatorjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-validatorjs)
#### Validation library inspired by Laravel's Validator

[![NPM](https://nodei.co/npm/validatorjs.png?downloads=true)](https://www.npmjs.com/package/validatorjs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-validatorjs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-validatorjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-validatorjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David",
        "email": "david@thejsguy.com"
    },
    "bugs": {
        "url": "https://github.com/skaterdav85/validatorjs/issues?labels=bug&milestone=1&page=1&state=open"
    },
    "contributors": [
        {
            "name": "Gary Green",
            "email": "holegary@gmail.com"
        },
        {
            "name": "Karol Janyst",
            "email": "lapkom@gmail.com"
        }
    ],
    "dependencies": {},
    "description": "Validation library inspired by Laravel's Validator",
    "devDependencies": {
        "browserify": "^13.0.1",
        "chai": "~3.5.0",
        "grunt": "1.0.1",
        "grunt-browserify": "^5.0.0",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-concat": "~1.0.1",
        "grunt-contrib-jshint": "1.0.0",
        "grunt-contrib-uglify": "1.0.1",
        "grunt-contrib-watch": "~1.0.0",
        "jit-grunt": "^0.10.0",
        "karma": "~1.1.0",
        "karma-browserify": "^5.0.5",
        "karma-chai": "~0.1.0",
        "karma-chrome-launcher": "~1.0.1",
        "karma-coverage": "~1.0.0",
        "karma-growl-notifications-reporter": "0.0.2",
        "karma-mocha": "~1.1.1",
        "karma-phantomjs-launcher": "~1.0.1",
        "mocha": "~2.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "d8177e62e663e4e06a6517540dfe1beabba2dfe5",
        "tarball": "https://registry.npmjs.org/validatorjs/-/validatorjs-3.11.0.tgz"
    },
    "gitHead": "8116e5a88d8ca0c4bb8ad2f6125d4afea6b1169d",
    "homepage": "https://github.com/skaterdav85/validatorjs#readme",
    "keywords": [
        "validatorjs",
        "validator.js",
        "data validation",
        "validator",
        "validate",
        "validation",
        "data",
        "laravel",
        "laravel-validator-for-js"
    ],
    "license": "MIT",
    "main": "./src/validator.js",
    "maintainers": [
        {
            "name": "garygreen",
            "email": "holegary@gmail.com"
        },
        {
            "name": "skaterdav85",
            "email": "dtang85@gmail.com"
        }
    ],
    "name": "validatorjs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/skaterdav85/validatorjs.git"
    },
    "scripts": {
        "test": "npm run test-node && npm run test-browser",
        "test-browser": "grunt dist && node node_modules/karma/bin/karma start --single-run --browsers PhantomJS",
        "test-node": "node node_modules/mocha/bin/mocha spec"
    },
    "version": "3.11.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module validatorjs](#apidoc.module.validatorjs)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>async (onFailedOne, onResolvedAll)](#apidoc.element.validatorjs.async)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>errors ()](#apidoc.element.validatorjs.errors)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>getDefaultLang ()](#apidoc.element.validatorjs.getDefaultLang)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>getMessages (lang)](#apidoc.element.validatorjs.getMessages)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>messages (lang, messages)](#apidoc.element.validatorjs.messages)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>register (name, fn, message)](#apidoc.element.validatorjs.register)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>registerAsync (name, fn, message)](#apidoc.element.validatorjs.registerAsync)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>setAttributeFormatter (func)](#apidoc.element.validatorjs.setAttributeFormatter)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>setMessages (lang, messages)](#apidoc.element.validatorjs.setMessages)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>stopOnError (attributes)](#apidoc.element.validatorjs.stopOnError)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>useLang (lang)](#apidoc.element.validatorjs.useLang)
1.  object <span class="apidocSignatureSpan">validatorjs.</span>async.prototype
1.  object <span class="apidocSignatureSpan">validatorjs.</span>attributes
1.  object <span class="apidocSignatureSpan">validatorjs.</span>errors.prototype
1.  object <span class="apidocSignatureSpan">validatorjs.</span>lang
1.  object <span class="apidocSignatureSpan">validatorjs.</span>messages.prototype
1.  object <span class="apidocSignatureSpan">validatorjs.</span>rules

#### [module validatorjs.async](#apidoc.module.validatorjs.async)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>async (onFailedOne, onResolvedAll)](#apidoc.element.validatorjs.async.async)

#### [module validatorjs.async.prototype](#apidoc.module.validatorjs.async.prototype)
1.  [function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>add (rule)](#apidoc.element.validatorjs.async.prototype.add)
1.  [function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>enableFiring ()](#apidoc.element.validatorjs.async.prototype.enableFiring)
1.  [function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>fire ()](#apidoc.element.validatorjs.async.prototype.fire)
1.  [function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>isAllResolved ()](#apidoc.element.validatorjs.async.prototype.isAllResolved)
1.  [function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>resolve (index)](#apidoc.element.validatorjs.async.prototype.resolve)

#### [module validatorjs.attributes](#apidoc.module.validatorjs.attributes)
1.  [function <span class="apidocSignatureSpan">validatorjs.attributes.</span>formatter (attribute)](#apidoc.element.validatorjs.attributes.formatter)
1.  object <span class="apidocSignatureSpan">validatorjs.attributes.</span>replacements

#### [module validatorjs.errors](#apidoc.module.validatorjs.errors)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>errors ()](#apidoc.element.validatorjs.errors.errors)

#### [module validatorjs.errors.prototype](#apidoc.module.validatorjs.errors.prototype)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>add (attribute, message)](#apidoc.element.validatorjs.errors.prototype.add)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>all ()](#apidoc.element.validatorjs.errors.prototype.all)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>constructor ()](#apidoc.element.validatorjs.errors.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>first (attribute)](#apidoc.element.validatorjs.errors.prototype.first)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>get (attribute)](#apidoc.element.validatorjs.errors.prototype.get)
1.  [function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>has (attribute)](#apidoc.element.validatorjs.errors.prototype.has)

#### [module validatorjs.lang](#apidoc.module.validatorjs.lang)
1.  [function <span class="apidocSignatureSpan">validatorjs.lang.</span>_get (lang)](#apidoc.element.validatorjs.lang._get)
1.  [function <span class="apidocSignatureSpan">validatorjs.lang.</span>_load (lang)](#apidoc.element.validatorjs.lang._load)
1.  [function <span class="apidocSignatureSpan">validatorjs.lang.</span>_make (lang)](#apidoc.element.validatorjs.lang._make)
1.  [function <span class="apidocSignatureSpan">validatorjs.lang.</span>_set (lang, rawMessages)](#apidoc.element.validatorjs.lang._set)
1.  [function <span class="apidocSignatureSpan">validatorjs.lang.</span>_setRuleMessage (lang, attribute, message)](#apidoc.element.validatorjs.lang._setRuleMessage)
1.  object <span class="apidocSignatureSpan">validatorjs.lang.</span>messages

#### [module validatorjs.messages](#apidoc.module.validatorjs.messages)
1.  [function <span class="apidocSignatureSpan">validatorjs.</span>messages (lang, messages)](#apidoc.element.validatorjs.messages.messages)

#### [module validatorjs.messages.prototype](#apidoc.module.validatorjs.messages.prototype)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_getAttributeName (attribute)](#apidoc.element.validatorjs.messages.prototype._getAttributeName)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_getTemplate (rule)](#apidoc.element.validatorjs.messages.prototype._getTemplate)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_replacePlaceholders (rule, template, data)](#apidoc.element.validatorjs.messages.prototype._replacePlaceholders)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setAttributeFormatter (func)](#apidoc.element.validatorjs.messages.prototype._setAttributeFormatter)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setAttributeNames (attributes)](#apidoc.element.validatorjs.messages.prototype._setAttributeNames)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setCustom (customMessages)](#apidoc.element.validatorjs.messages.prototype._setCustom)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>all ()](#apidoc.element.validatorjs.messages.prototype.all)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>constructor (lang, messages)](#apidoc.element.validatorjs.messages.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>render (rule)](#apidoc.element.validatorjs.messages.prototype.render)

#### [module validatorjs.rules](#apidoc.module.validatorjs.rules)
1.  [function <span class="apidocSignatureSpan">validatorjs.rules.</span>isAsync (name)](#apidoc.element.validatorjs.rules.isAsync)
1.  [function <span class="apidocSignatureSpan">validatorjs.rules.</span>isImplicit (name)](#apidoc.element.validatorjs.rules.isImplicit)
1.  [function <span class="apidocSignatureSpan">validatorjs.rules.</span>make (name, validator)](#apidoc.element.validatorjs.rules.make)
1.  [function <span class="apidocSignatureSpan">validatorjs.rules.</span>register (name, fn)](#apidoc.element.validatorjs.rules.register)
1.  [function <span class="apidocSignatureSpan">validatorjs.rules.</span>registerAsync (name, fn)](#apidoc.element.validatorjs.rules.registerAsync)
1.  object <span class="apidocSignatureSpan">validatorjs.rules.</span>asyncRules
1.  object <span class="apidocSignatureSpan">validatorjs.rules.</span>implicitRules



# <a name="apidoc.module.validatorjs"></a>[module validatorjs](#apidoc.module.validatorjs)

#### <a name="apidoc.element.validatorjs.async"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>async (onFailedOne, onResolvedAll)](#apidoc.element.validatorjs.async)
- description and source-code
```javascript
function AsyncResolvers(onFailedOne, onResolvedAll) {
  this.onResolvedAll = onResolvedAll;
  this.onFailedOne = onFailedOne;
  this.resolvers = {};
  this.resolversCount = 0;
  this.passed = [];
  this.failed = [];
  this.firing = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.errors"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>errors ()](#apidoc.element.validatorjs.errors)
- description and source-code
```javascript
errors = function () {
  this.errors = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.getDefaultLang"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>getDefaultLang ()](#apidoc.element.validatorjs.getDefaultLang)
- description and source-code
```javascript
getDefaultLang = function () {
  return this.prototype.lang;
}
```
- example usage
```shell
...
'''js
Validator.useLang('lang_code');
'''

Get the default language being used:

'''js
Validator.getDefaultLang(); // returns e.g. 'en'
'''

Override default messages for language:

'''js
var messages = Validator.getMessages('en');
messages.required = 'Whoops, :attribute field is required.';
...
```

#### <a name="apidoc.element.validatorjs.getMessages"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>getMessages (lang)](#apidoc.element.validatorjs.getMessages)
- description and source-code
```javascript
getMessages = function (lang) {
  return Lang._get(lang);
}
```
- example usage
```shell
...
	....
});
'''

Get the raw object of messages for the given language:

'''js
Validator.getMessages('lang_code');
'''

Switch the default language used by the validator:

'''js
Validator.useLang('lang_code');
'''
...
```

#### <a name="apidoc.element.validatorjs.messages"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>messages (lang, messages)](#apidoc.element.validatorjs.messages)
- description and source-code
```javascript
messages = function (lang, messages) {
  this.lang = lang;
  this.messages = messages;
  this.customMessages = {};
  this.attributeNames = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.register"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>register (name, fn, message)](#apidoc.element.validatorjs.register)
- description and source-code
```javascript
register = function (name, fn, message) {
  var lang = Validator.getDefaultLang();
  Rules.register(name, fn);
  Lang._setRuleMessage(lang, name, message);
}
```
- example usage
```shell
...
validation.passes(); // true

'''

### Registering Custom Validation Rules

'''js
Validator.register(name, callbackFn, errorMessage);
'''

__name__ {String} - The name of the rule.

__callbackFn__ {Function} - Returns a boolean to represent a successful or failed validation.

__errorMessage__ {String} - An optional string where you can specify a custom error message. _:attribute_ inside errorMessage will
 be replaced with the attribute name.
...
```

#### <a name="apidoc.element.validatorjs.registerAsync"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>registerAsync (name, fn, message)](#apidoc.element.validatorjs.registerAsync)
- description and source-code
```javascript
registerAsync = function (name, fn, message) {
  var lang = Validator.getDefaultLang();
  Rules.registerAsync(name, fn);
  Lang._setRuleMessage(lang, name, message);
}
```
- example usage
```shell
...
'''

### Asynchronous validation

Register an asynchronous rule which accepts a 'passes' callback:

'''js
Validator.registerAsync('username_available', function(username, attribute, req, passes) {
	// do your database/api checks here etc
	// then call the 'passes' method where appropriate:
	passes(); // if username is available
	passes(false, 'Username has already been taken.'); // if username is not available
});
'''
...
```

#### <a name="apidoc.element.validatorjs.setAttributeFormatter"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>setAttributeFormatter (func)](#apidoc.element.validatorjs.setAttributeFormatter)
- description and source-code
```javascript
setAttributeFormatter = function (func) {
  this.prototype.attributeFormatter = func;
}
```
- example usage
```shell
...

Alternatively you can supply global custom attribute names in your lang with the 'attributes' property.

You can also configure a custom attribute formatter:

'''js
// Configure global formatter.
Validator.setAttributeFormatter(function(attribute) {
	return attribute.replace(/_/g, ' ');
});

// Or configure formatter for particular instance.
var validator = new Validator({ first_name: '' }, { first_name: 'required' });
validator.setAttributeFormatter(function(attribute) {
	return attribute.replace(/_/g, ' ');
...
```

#### <a name="apidoc.element.validatorjs.setMessages"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>setMessages (lang, messages)](#apidoc.element.validatorjs.setMessages)
- description and source-code
```javascript
setMessages = function (lang, messages) {
  Lang._set(lang, messages);
  return this;
}
```
- example usage
```shell
...
'''

If you don't see support for your language, please add one to 'src/lang'!

You can also add your own custom language by calling 'setMessages':

'''js
Validator.setMessages('lang_code', {
	required: 'The :attribute field is required.',
	....
	....
});
'''

Get the raw object of messages for the given language:
...
```

#### <a name="apidoc.element.validatorjs.stopOnError"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>stopOnError (attributes)](#apidoc.element.validatorjs.stopOnError)
- description and source-code
```javascript
stopOnError = function (attributes) {
  this.prototype.stopOnAttributes = attributes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.useLang"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>useLang (lang)](#apidoc.element.validatorjs.useLang)
- description and source-code
```javascript
useLang = function (lang) {
  this.prototype.lang = lang;
}
```
- example usage
```shell
...
}
'''

Note: by default all _[] characters will be replaced with spaces.

### Language Support

Error messages are in English by default. To include another language in the browser, reference the language file in a script tag
 and call 'Validator.useLang('lang_code')'.

'''html
<script src="dist/validator.min.js"></script>
<script src="dist/lang/ru.js"></script>
<script>
	Validator.useLang('es');
</script>
...
```



# <a name="apidoc.module.validatorjs.async"></a>[module validatorjs.async](#apidoc.module.validatorjs.async)

#### <a name="apidoc.element.validatorjs.async.async"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>async (onFailedOne, onResolvedAll)](#apidoc.element.validatorjs.async.async)
- description and source-code
```javascript
function AsyncResolvers(onFailedOne, onResolvedAll) {
  this.onResolvedAll = onResolvedAll;
  this.onFailedOne = onFailedOne;
  this.resolvers = {};
  this.resolversCount = 0;
  this.passed = [];
  this.failed = [];
  this.firing = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.async.prototype"></a>[module validatorjs.async.prototype](#apidoc.module.validatorjs.async.prototype)

#### <a name="apidoc.element.validatorjs.async.prototype.add"></a>[function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>add (rule)](#apidoc.element.validatorjs.async.prototype.add)
- description and source-code
```javascript
add = function (rule) {
  var index = this.resolversCount;
  this.resolvers[index] = rule;
  this.resolversCount++;
  return index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.async.prototype.enableFiring"></a>[function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>enableFiring ()](#apidoc.element.validatorjs.async.prototype.enableFiring)
- description and source-code
```javascript
enableFiring = function () {
  this.firing = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.async.prototype.fire"></a>[function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>fire ()](#apidoc.element.validatorjs.async.prototype.fire)
- description and source-code
```javascript
fire = function () {

  if (!this.firing) {
    return;
  }

  if (this.isAllResolved()) {
    this.onResolvedAll(this.failed.length === 0);
  }

}
```
- example usage
```shell
...
  if (rule.passes === true) {
    this.passed.push(rule);
  } else if (rule.passes === false) {
    this.failed.push(rule);
    this.onFailedOne(rule);
  }

  this.fire();
},

/**
 * Determine if all have been resolved
 *
 * @return {boolean}
 */
...
```

#### <a name="apidoc.element.validatorjs.async.prototype.isAllResolved"></a>[function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>isAllResolved ()](#apidoc.element.validatorjs.async.prototype.isAllResolved)
- description and source-code
```javascript
isAllResolved = function () {
  return (this.passed.length + this.failed.length) === this.resolversCount;
}
```
- example usage
```shell
...
 */
fire: function() {

  if (!this.firing) {
    return;
  }

  if (this.isAllResolved()) {
    this.onResolvedAll(this.failed.length === 0);
  }

},

/**
 * Enable firing
...
```

#### <a name="apidoc.element.validatorjs.async.prototype.resolve"></a>[function <span class="apidocSignatureSpan">validatorjs.async.prototype.</span>resolve (index)](#apidoc.element.validatorjs.async.prototype.resolve)
- description and source-code
```javascript
resolve = function (index) {
  var rule = this.resolvers[index];
  if (rule.passes === true) {
    this.passed.push(rule);
  } else if (rule.passes === false) {
    this.failed.push(rule);
    this.onFailedOne(rule);
  }

  this.fire();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.attributes"></a>[module validatorjs.attributes](#apidoc.module.validatorjs.attributes)

#### <a name="apidoc.element.validatorjs.attributes.formatter"></a>[function <span class="apidocSignatureSpan">validatorjs.attributes.</span>formatter (attribute)](#apidoc.element.validatorjs.attributes.formatter)
- description and source-code
```javascript
function formatter(attribute) {
  return attribute.replace(/[_\[]/g, ' ').replace(/]/g, '');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.errors"></a>[module validatorjs.errors](#apidoc.module.validatorjs.errors)

#### <a name="apidoc.element.validatorjs.errors.errors"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>errors ()](#apidoc.element.validatorjs.errors.errors)
- description and source-code
```javascript
errors = function () {
  this.errors = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.errors.prototype"></a>[module validatorjs.errors.prototype](#apidoc.module.validatorjs.errors.prototype)

#### <a name="apidoc.element.validatorjs.errors.prototype.add"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>add (attribute, message)](#apidoc.element.validatorjs.errors.prototype.add)
- description and source-code
```javascript
add = function (attribute, message) {
  if (!this.has(attribute)) {
    this.errors[attribute] = [];
  }

  if (this.errors[attribute].indexOf(message) === -1) {
    this.errors[attribute].push(message);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.errors.prototype.all"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>all ()](#apidoc.element.validatorjs.errors.prototype.all)
- description and source-code
```javascript
all = function () {
  return this.errors;
}
```
- example usage
```shell
...

returns the first error message for an attribute, false otherwise

#### .get(attribute)

returns an array of error messages for an attribute, or an empty array if there are no errors

#### .all()

returns an object containing all error messages for all failing attributes

#### .has(attribute)

returns true if error messages exist for an attribute, false otherwise
...
```

#### <a name="apidoc.element.validatorjs.errors.prototype.constructor"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>constructor ()](#apidoc.element.validatorjs.errors.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  this.errors = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.errors.prototype.first"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>first (attribute)](#apidoc.element.validatorjs.errors.prototype.first)
- description and source-code
```javascript
first = function (attribute) {
  if (this.has(attribute)) {
    return this.errors[attribute][0];
  }

  return false;
}
```
- example usage
```shell
...
	email: 'required|email'
});

validation.fails(); // true
validation.passes(); // false

// Error messages
validation.errors.first('email'); // 'The email format is invalid.'
validation.errors.get('email'); // returns an array of all email error messages
'''

### Nested rules

Nested objects can also be validated. There are two ways to declare validation rules for nested objects. The first way is to declare
 the validation rules with a corresponding nested object structure that reflects the data. The second way is to declare validation
 rules with flattened key names. For example, to validate the following data:
...
```

#### <a name="apidoc.element.validatorjs.errors.prototype.get"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>get (attribute)](#apidoc.element.validatorjs.errors.prototype.get)
- description and source-code
```javascript
get = function (attribute) {
  if (this.has(attribute)) {
    return this.errors[attribute];
  }

  return [];
}
```
- example usage
```shell
...
});

validation.fails(); // true
validation.passes(); // false

// Error messages
validation.errors.first('email'); // 'The email format is invalid.'
validation.errors.get('email'); // returns an array of all email error messages
'''

### Nested rules

Nested objects can also be validated. There are two ways to declare validation rules for nested objects. The first way is to declare
 the validation rules with a corresponding nested object structure that reflects the data. The second way is to declare validation
 rules with flattened key names. For example, to validate the following data:

'''js
...
```

#### <a name="apidoc.element.validatorjs.errors.prototype.has"></a>[function <span class="apidocSignatureSpan">validatorjs.errors.prototype.</span>has (attribute)](#apidoc.element.validatorjs.errors.prototype.has)
- description and source-code
```javascript
has = function (attribute) {
  if (this.errors.hasOwnProperty(attribute)) {
    return true;
  }

  return false;
}
```
- example usage
```shell
...

returns an array of error messages for an attribute, or an empty array if there are no errors

#### .all()

returns an object containing all error messages for all failing attributes

#### .has(attribute)

returns true if error messages exist for an attribute, false otherwise

#### .errorCount

the number of validation errors
...
```



# <a name="apidoc.module.validatorjs.lang"></a>[module validatorjs.lang](#apidoc.module.validatorjs.lang)

#### <a name="apidoc.element.validatorjs.lang._get"></a>[function <span class="apidocSignatureSpan">validatorjs.lang.</span>_get (lang)](#apidoc.element.validatorjs.lang._get)
- description and source-code
```javascript
_get = function (lang) {
  this._load(lang);
  return this.messages[lang];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.lang._load"></a>[function <span class="apidocSignatureSpan">validatorjs.lang.</span>_load (lang)](#apidoc.element.validatorjs.lang._load)
- description and source-code
```javascript
_load = function (lang) {
  if (!this.messages[lang]) {
    var rawMessages = require('./lang/' + lang);
    this._set(lang, rawMessages);
  }
}
```
- example usage
```shell
...
 *
 * @param {string} lang
 * @param {string} attribute
 * @param {string|object} message
 * @return {void}
 */
_setRuleMessage: function(lang, attribute, message) {
  this._load(lang);
  if (message === undefined) {
    message = this.messages[lang].def;
  }

  this.messages[lang][attribute] = message;
},
...
```

#### <a name="apidoc.element.validatorjs.lang._make"></a>[function <span class="apidocSignatureSpan">validatorjs.lang.</span>_make (lang)](#apidoc.element.validatorjs.lang._make)
- description and source-code
```javascript
_make = function (lang) {
  this._load(lang);
  return new Messages(lang, this.messages[lang]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.lang._set"></a>[function <span class="apidocSignatureSpan">validatorjs.lang.</span>_set (lang, rawMessages)](#apidoc.element.validatorjs.lang._set)
- description and source-code
```javascript
_set = function (lang, rawMessages) {
  this.messages[lang] = rawMessages;
}
```
- example usage
```shell
...
 *
 * @param  {string} lang
 * @return {void}
 */
_load: function(lang) {
  if (!this.messages[lang]) {
    var rawMessages = require('./lang/' + lang);
    this._set(lang, rawMessages);
  }
},

/**
 * Get raw messages for language
 *
 * @param  {string} lang
...
```

#### <a name="apidoc.element.validatorjs.lang._setRuleMessage"></a>[function <span class="apidocSignatureSpan">validatorjs.lang.</span>_setRuleMessage (lang, attribute, message)](#apidoc.element.validatorjs.lang._setRuleMessage)
- description and source-code
```javascript
_setRuleMessage = function (lang, attribute, message) {
  this._load(lang);
  if (message === undefined) {
    message = this.messages[lang].def;
  }

  this.messages[lang][attribute] = message;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.messages"></a>[module validatorjs.messages](#apidoc.module.validatorjs.messages)

#### <a name="apidoc.element.validatorjs.messages.messages"></a>[function <span class="apidocSignatureSpan">validatorjs.</span>messages (lang, messages)](#apidoc.element.validatorjs.messages.messages)
- description and source-code
```javascript
messages = function (lang, messages) {
  this.lang = lang;
  this.messages = messages;
  this.customMessages = {};
  this.attributeNames = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.messages.prototype"></a>[module validatorjs.messages.prototype](#apidoc.module.validatorjs.messages.prototype)

#### <a name="apidoc.element.validatorjs.messages.prototype._getAttributeName"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_getAttributeName (attribute)](#apidoc.element.validatorjs.messages.prototype._getAttributeName)
- description and source-code
```javascript
_getAttributeName = function (attribute) {
  var name = attribute;
  if (this.attributeNames.hasOwnProperty(attribute)) {
    return this.attributeNames[attribute];
  } else if (this.messages.attributes.hasOwnProperty(attribute)) {
    name = this.messages.attributes[attribute];
  }

  if (this.attributeFormatter) {
    name = this.attributeFormatter(name);
  }

  return name;
}
```
- example usage
```shell
...
   * @param  {string} template
   * @param  {object} data
   * @return {string}
   */
  _replacePlaceholders: function(rule, template, data) {
    var message, attribute;

    data.attribute = this._getAttributeName(rule.attribute);
    data[rule.name] = rule.getParameters().join(',');

    if (typeof template === 'string' && typeof data === 'object') {
message = template;

for (attribute in data) {
  message = message.replace(new RegExp(':' + attribute, 'g'), data[attribute]);
...
```

#### <a name="apidoc.element.validatorjs.messages.prototype._getTemplate"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_getTemplate (rule)](#apidoc.element.validatorjs.messages.prototype._getTemplate)
- description and source-code
```javascript
_getTemplate = function (rule) {

  var messages = this.messages;
  var template = messages.def;
  var customMessages = this.customMessages;
  var formats = [rule.name + '.' + rule.attribute, rule.name];

  for (var i = 0, format; i < formats.length; i++) {
    format = formats[i];
    if (customMessages.hasOwnProperty(format)) {
      template = customMessages[format];
      break;
    } else if (messages.hasOwnProperty(format)) {
      template = messages[format];
      break;
    }
  }

  if (typeof template === 'object') {
    template = template[rule._getValueType()];
  }

  return template;
}
```
- example usage
```shell
...
   * @param  {Rule} rule
   * @return {string}
   */
  render: function(rule) {
if (rule.customMessage) {
  return rule.customMessage;
}
var template = this._getTemplate(rule);

var message;
if (Attributes.replacements[rule.name]) {
  message = Attributes.replacements[rule.name].apply(this, [template, rule]);
} else {
  message = this._replacePlaceholders(rule, template, {});
}
...
```

#### <a name="apidoc.element.validatorjs.messages.prototype._replacePlaceholders"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_replacePlaceholders (rule, template, data)](#apidoc.element.validatorjs.messages.prototype._replacePlaceholders)
- description and source-code
```javascript
_replacePlaceholders = function (rule, template, data) {
  var message, attribute;

  data.attribute = this._getAttributeName(rule.attribute);
  data[rule.name] = rule.getParameters().join(',');

  if (typeof template === 'string' && typeof data === 'object') {
    message = template;

    for (attribute in data) {
      message = message.replace(new RegExp(':' + attribute, 'g'), data[attribute]);
    }
  }

  return message;
}
```
- example usage
```shell
...
 *
 * @param  {string} template
 * @param  {Rule} rule
 * @return {string}
 */
between: function(template, rule) {
  var parameters = rule.getParameters();
  return this._replacePlaceholders(rule, template, {
    min: parameters[0],
    max: parameters[1]
  });
},

/**
 * Required_if replacement.
...
```

#### <a name="apidoc.element.validatorjs.messages.prototype._setAttributeFormatter"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setAttributeFormatter (func)](#apidoc.element.validatorjs.messages.prototype._setAttributeFormatter)
- description and source-code
```javascript
_setAttributeFormatter = function (func) {
  this.attributeFormatter = func;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.messages.prototype._setAttributeNames"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setAttributeNames (attributes)](#apidoc.element.validatorjs.messages.prototype._setAttributeNames)
- description and source-code
```javascript
_setAttributeNames = function (attributes) {
  this.attributeNames = attributes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.messages.prototype._setCustom"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>_setCustom (customMessages)](#apidoc.element.validatorjs.messages.prototype._setCustom)
- description and source-code
```javascript
_setCustom = function (customMessages) {
  this.customMessages = customMessages || {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.messages.prototype.all"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>all ()](#apidoc.element.validatorjs.messages.prototype.all)
- description and source-code
```javascript
all = function () {
  return this.messages;
}
```
- example usage
```shell
...

returns the first error message for an attribute, false otherwise

#### .get(attribute)

returns an array of error messages for an attribute, or an empty array if there are no errors

#### .all()

returns an object containing all error messages for all failing attributes

#### .has(attribute)

returns true if error messages exist for an attribute, false otherwise
...
```

#### <a name="apidoc.element.validatorjs.messages.prototype.constructor"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>constructor (lang, messages)](#apidoc.element.validatorjs.messages.prototype.constructor)
- description and source-code
```javascript
constructor = function (lang, messages) {
  this.lang = lang;
  this.messages = messages;
  this.customMessages = {};
  this.attributeNames = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.messages.prototype.render"></a>[function <span class="apidocSignatureSpan">validatorjs.messages.prototype.</span>render (rule)](#apidoc.element.validatorjs.messages.prototype.render)
- description and source-code
```javascript
render = function (rule) {
  if (rule.customMessage) {
    return rule.customMessage;
  }
  var template = this._getTemplate(rule);

  var message;
  if (Attributes.replacements[rule.name]) {
    message = Attributes.replacements[rule.name].apply(this, [template, rule]);
  } else {
    message = this._replacePlaceholders(rule, template, {});
  }

  return message;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validatorjs.rules"></a>[module validatorjs.rules](#apidoc.module.validatorjs.rules)

#### <a name="apidoc.element.validatorjs.rules.isAsync"></a>[function <span class="apidocSignatureSpan">validatorjs.rules.</span>isAsync (name)](#apidoc.element.validatorjs.rules.isAsync)
- description and source-code
```javascript
isAsync = function (name) {
  for (var i = 0, len = this.asyncRules.length; i < len; i++) {
    if (this.asyncRules[i] === name) {
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
...
 * Get rule by name
 *
 * @param  {string} name
 * @param {Validator}
 * @return {Rule}
 */
make: function(name, validator) {
  var async = this.isAsync(name);
  var rule = new Rule(name, rules[name], async);
  rule.setValidator(validator);
  return rule;
},

/**
 * Determine if given rule is async
...
```

#### <a name="apidoc.element.validatorjs.rules.isImplicit"></a>[function <span class="apidocSignatureSpan">validatorjs.rules.</span>isImplicit (name)](#apidoc.element.validatorjs.rules.isImplicit)
- description and source-code
```javascript
isImplicit = function (name) {
  return this.implicitRules.indexOf(name) > -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.rules.make"></a>[function <span class="apidocSignatureSpan">validatorjs.rules.</span>make (name, validator)](#apidoc.element.validatorjs.rules.make)
- description and source-code
```javascript
make = function (name, validator) {
  var async = this.isAsync(name);
  var rule = new Rule(name, rules[name], async);
  rule.setValidator(validator);
  return rule;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validatorjs.rules.register"></a>[function <span class="apidocSignatureSpan">validatorjs.rules.</span>register (name, fn)](#apidoc.element.validatorjs.rules.register)
- description and source-code
```javascript
register = function (name, fn) {
  rules[name] = fn;
}
```
- example usage
```shell
...
validation.passes(); // true

'''

### Registering Custom Validation Rules

'''js
Validator.register(name, callbackFn, errorMessage);
'''

__name__ {String} - The name of the rule.

__callbackFn__ {Function} - Returns a boolean to represent a successful or failed validation.

__errorMessage__ {String} - An optional string where you can specify a custom error message. _:attribute_ inside errorMessage will
 be replaced with the attribute name.
...
```

#### <a name="apidoc.element.validatorjs.rules.registerAsync"></a>[function <span class="apidocSignatureSpan">validatorjs.rules.</span>registerAsync (name, fn)](#apidoc.element.validatorjs.rules.registerAsync)
- description and source-code
```javascript
registerAsync = function (name, fn) {
  this.register(name, fn);
  this.asyncRules.push(name);
}
```
- example usage
```shell
...
'''

### Asynchronous validation

Register an asynchronous rule which accepts a 'passes' callback:

'''js
Validator.registerAsync('username_available', function(username, attribute, req, passes) {
	// do your database/api checks here etc
	// then call the 'passes' method where appropriate:
	passes(); // if username is available
	passes(false, 'Username has already been taken.'); // if username is not available
});
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
