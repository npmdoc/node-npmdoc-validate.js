# api documentation for  [validate.js (v0.11.1)](http://validatejs.org)  [![npm package](https://img.shields.io/npm/v/npmdoc-validate.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-validate.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-validate.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-validate.js)
#### Declarative validations for JavaScript

[![NPM](https://nodei.co/npm/validate.js.png?downloads=true)](https://www.npmjs.com/package/validate.js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-validate.js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-validate.js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-validate.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-validate.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-validate.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nicklas Ansman",
        "email": "nicklas@ansman.se"
    },
    "bugs": {
        "url": "https://github.com/ansman/validate.js/issues"
    },
    "dependencies": {},
    "description": "Declarative validations for JavaScript",
    "devDependencies": {
        "coveralls": "2.11.9",
        "grunt": "1.0.1",
        "grunt-contrib-jasmine": "1.0.3",
        "grunt-contrib-jshint": "1.0.0",
        "grunt-contrib-uglify": "1.0.1",
        "grunt-contrib-watch": "1.0.0",
        "grunt-docco": "0.4.0",
        "grunt-notify": "0.4.5",
        "grunt-template-jasmine-istanbul": "0.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "f51c3c6c4a56e6380a20a7eb104245037f2a540d",
        "tarball": "https://registry.npmjs.org/validate.js/-/validate.js-0.11.1.tgz"
    },
    "gitHead": "047f315ed3369e75726a77ffc6d4f6248b10f798",
    "homepage": "http://validatejs.org",
    "keywords": [
        "validation",
        "validate",
        "server",
        "client"
    ],
    "license": "MIT",
    "main": "validate.js",
    "maintainers": [
        {
            "name": "ansman",
            "email": "nicklas@ansman.se"
        }
    ],
    "name": "validate.js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ansman/validate.js.git"
    },
    "scripts": {
        "build": "grunt build",
        "docs": "grunt docco",
        "test": "grunt test",
        "watch": "grunt watch"
    },
    "typings": "validate.d.ts",
    "version": "0.11.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module validate.js](#apidoc.module.validate.js)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>Promise ()](#apidoc.element.validate.js.Promise)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>async (attributes, constraints, options)](#apidoc.element.validate.js.async)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>capitalize (str)](#apidoc.element.validate.js.capitalize)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>cleanAttributes (attributes, whitelist)](#apidoc.element.validate.js.cleanAttributes)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>collectFormValues (form, options)](#apidoc.element.validate.js.collectFormValues)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>contains (obj, value)](#apidoc.element.validate.js.contains)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>convertErrorMessages (errors, options)](#apidoc.element.validate.js.convertErrorMessages)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>error (msg)](#apidoc.element.validate.js.error)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>expandMultipleErrors (errors)](#apidoc.element.validate.js.expandMultipleErrors)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>exposeModule (validate, root, exports, module, define)](#apidoc.element.validate.js.exposeModule)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>extend (obj)](#apidoc.element.validate.js.extend)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>flattenErrorsToArray (errors)](#apidoc.element.validate.js.flattenErrorsToArray)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>forEachKeyInKeypath (object, keypath, callback)](#apidoc.element.validate.js.forEachKeyInKeypath)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>format (str, vals)](#apidoc.element.validate.js.format)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>getDeepObjectValue (obj, keypath)](#apidoc.element.validate.js.getDeepObjectValue)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>groupErrorsByAttribute (errors)](#apidoc.element.validate.js.groupErrorsByAttribute)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isArray (value)](#apidoc.element.validate.js.isArray)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isBoolean (value)](#apidoc.element.validate.js.isBoolean)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isDate (obj)](#apidoc.element.validate.js.isDate)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isDefined (obj)](#apidoc.element.validate.js.isDefined)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isDomElement (o)](#apidoc.element.validate.js.isDomElement)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isEmpty (value)](#apidoc.element.validate.js.isEmpty)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isFunction (value)](#apidoc.element.validate.js.isFunction)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isHash (value)](#apidoc.element.validate.js.isHash)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isInteger (value)](#apidoc.element.validate.js.isInteger)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isJqueryElement (o)](#apidoc.element.validate.js.isJqueryElement)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isNumber (value)](#apidoc.element.validate.js.isNumber)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isObject (obj)](#apidoc.element.validate.js.isObject)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isPromise (p)](#apidoc.element.validate.js.isPromise)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>isString (value)](#apidoc.element.validate.js.isString)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>prettify (str)](#apidoc.element.validate.js.prettify)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>processValidationResults (errors, options)](#apidoc.element.validate.js.processValidationResults)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>pruneEmptyErrors (errors)](#apidoc.element.validate.js.pruneEmptyErrors)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>result (value)](#apidoc.element.validate.js.result)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>runValidations (attributes, constraints, options)](#apidoc.element.validate.js.runValidations)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>sanitizeFormValue (value, options)](#apidoc.element.validate.js.sanitizeFormValue)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>single (value, constraints, options)](#apidoc.element.validate.js.single)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>stringifyValue (value)](#apidoc.element.validate.js.stringifyValue)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>unique (array)](#apidoc.element.validate.js.unique)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>validate (attributes, constraints, options)](#apidoc.element.validate.js.validate)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>waitForResults (results)](#apidoc.element.validate.js.waitForResults)
1.  [function <span class="apidocSignatureSpan">validate.js.</span>warn (msg)](#apidoc.element.validate.js.warn)
1.  object <span class="apidocSignatureSpan">validate.js.</span>EMPTY_STRING_REGEXP
1.  object <span class="apidocSignatureSpan">validate.js.</span>formatters
1.  object <span class="apidocSignatureSpan">validate.js.</span>js.formatters
1.  object <span class="apidocSignatureSpan">validate.js.</span>js.validators
1.  object <span class="apidocSignatureSpan">validate.js.</span>js.version
1.  object <span class="apidocSignatureSpan">validate.js.</span>validators
1.  object <span class="apidocSignatureSpan">validate.js.</span>version

#### [module validate.js.formatters](#apidoc.module.validate.js.formatters)
1.  [function <span class="apidocSignatureSpan">validate.js.formatters.</span>constraint (errors)](#apidoc.element.validate.js.formatters.constraint)
1.  [function <span class="apidocSignatureSpan">validate.js.formatters.</span>detailed (errors)](#apidoc.element.validate.js.formatters.detailed)
1.  [function <span class="apidocSignatureSpan">validate.js.formatters.</span>flat (errors)](#apidoc.element.validate.js.formatters.flat)
1.  [function <span class="apidocSignatureSpan">validate.js.formatters.</span>grouped (errors)](#apidoc.element.validate.js.formatters.grouped)

#### [module validate.js.validators](#apidoc.module.validate.js.validators)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>date (value, options)](#apidoc.element.validate.js.validators.date)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>datetime (value, options)](#apidoc.element.validate.js.validators.datetime)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>email (value, options)](#apidoc.element.validate.js.validators.email)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>equality (value, options, attribute, attributes)](#apidoc.element.validate.js.validators.equality)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>exclusion (value, options)](#apidoc.element.validate.js.validators.exclusion)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>format (value, options)](#apidoc.element.validate.js.validators.format)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>inclusion (value, options)](#apidoc.element.validate.js.validators.inclusion)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>length (value, options, attribute)](#apidoc.element.validate.js.validators.length)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>numericality (value, options)](#apidoc.element.validate.js.validators.numericality)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>presence (value, options)](#apidoc.element.validate.js.validators.presence)
1.  [function <span class="apidocSignatureSpan">validate.js.validators.</span>url (value, options)](#apidoc.element.validate.js.validators.url)

#### [module validate.js.version](#apidoc.module.validate.js.version)
1.  [function <span class="apidocSignatureSpan">validate.js.version.</span>toString ()](#apidoc.element.validate.js.version.toString)
1.  number <span class="apidocSignatureSpan">validate.js.version.</span>major
1.  number <span class="apidocSignatureSpan">validate.js.version.</span>minor
1.  number <span class="apidocSignatureSpan">validate.js.version.</span>patch
1.  object <span class="apidocSignatureSpan">validate.js.version.</span>metadata



# <a name="apidoc.module.validate.js"></a>[module validate.js](#apidoc.module.validate.js)

#### <a name="apidoc.element.validate.js.Promise"></a>[function <span class="apidocSignatureSpan">validate.js.</span>Promise ()](#apidoc.element.validate.js.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
...
// Removes unknown attributes
if (options.cleanAttributes !== false) {
  attributes = v.cleanAttributes(attributes, constraints);
}

var results = v.runValidations(attributes, constraints, options);

return new v.Promise(function(resolve, reject) {
  v.waitForResults(results).then(function() {
    var errors = v.processValidationResults(results, options);
    if (errors) {
      reject(new WrapErrors(errors, options, attributes, constraints));
    } else {
      resolve(attributes);
    }
...
```

#### <a name="apidoc.element.validate.js.async"></a>[function <span class="apidocSignatureSpan">validate.js.</span>async (attributes, constraints, options)](#apidoc.element.validate.js.async)
- description and source-code
```javascript
async = function (attributes, constraints, options) {
  options = v.extend({}, v.async.options, options);

  var WrapErrors = options.wrapErrors || function(errors) {
    return errors;
  };

  // Removes unknown attributes
  if (options.cleanAttributes !== false) {
    attributes = v.cleanAttributes(attributes, constraints);
  }

  var results = v.runValidations(attributes, constraints, options);

  return new v.Promise(function(resolve, reject) {
    v.waitForResults(results).then(function() {
      var errors = v.processValidationResults(results, options);
      if (errors) {
        reject(new WrapErrors(errors, options, attributes, constraints));
      } else {
        resolve(attributes);
      }
    }, function(err) {
      reject(err);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.capitalize"></a>[function <span class="apidocSignatureSpan">validate.js.</span>capitalize (str)](#apidoc.element.validate.js.capitalize)
- description and source-code
```javascript
capitalize = function (str) {
  if (!v.isString(str)) {
    return str;
  }
  return str[0].toUpperCase() + str.slice(1);
}
```
- example usage
```shell
...
      ret.push(errorInfo);
      return;
    }

    if (error[0] === '^') {
      error = error.slice(1);
    } else if (options.fullMessages !== false) {
      error = v.capitalize(v.prettify(errorInfo.attribute)) + " " + error;
    }
    error = error.replace(/\\\^/g, "^");
    error = v.format(error, {value: v.stringifyValue(errorInfo.value)});
    ret.push(v.extend({}, errorInfo, {error: error}));
  });
  return ret;
},
...
```

#### <a name="apidoc.element.validate.js.cleanAttributes"></a>[function <span class="apidocSignatureSpan">validate.js.</span>cleanAttributes (attributes, whitelist)](#apidoc.element.validate.js.cleanAttributes)
- description and source-code
```javascript
cleanAttributes = function (attributes, whitelist) {
  function whitelistCreator(obj, key, last) {
    if (v.isObject(obj[key])) {
      return obj[key];
    }
    return (obj[key] = last ? true : {});
  }

  function buildObjectWhitelist(whitelist) {
    var ow = {}
      , lastObject
      , attr;
    for (attr in whitelist) {
      if (!whitelist[attr]) {
        continue;
      }
      v.forEachKeyInKeypath(ow, attr, whitelistCreator);
    }
    return ow;
  }

  function cleanRecursive(attributes, whitelist) {
    if (!v.isObject(attributes)) {
      return attributes;
    }

    var ret = v.extend({}, attributes)
      , w
      , attribute;

    for (attribute in attributes) {
      w = whitelist[attribute];

      if (v.isObject(w)) {
        ret[attribute] = cleanRecursive(ret[attribute], w);
      } else if (!w) {
        delete ret[attribute];
      }
    }
    return ret;
  }

  if (!v.isObject(whitelist) || !v.isObject(attributes)) {
    return {};
  }

  whitelist = buildObjectWhitelist(whitelist);
  return cleanRecursive(attributes, whitelist);
}
```
- example usage
```shell
...

var WrapErrors = options.wrapErrors || function(errors) {
  return errors;
};

// Removes unknown attributes
if (options.cleanAttributes !== false) {
  attributes = v.cleanAttributes(attributes, constraints);
}

var results = v.runValidations(attributes, constraints, options);

return new v.Promise(function(resolve, reject) {
  v.waitForResults(results).then(function() {
    var errors = v.processValidationResults(results, options);
...
```

#### <a name="apidoc.element.validate.js.collectFormValues"></a>[function <span class="apidocSignatureSpan">validate.js.</span>collectFormValues (form, options)](#apidoc.element.validate.js.collectFormValues)
- description and source-code
```javascript
collectFormValues = function (form, options) {
  var values = {}
    , i
    , j
    , input
    , inputs
    , option
    , value;

  if (v.isJqueryElement(form)) {
    form = form[0];
  }

  if (!form) {
    return values;
  }

  options = options || {};

  inputs = form.querySelectorAll("input[name], textarea[name]");
  for (i = 0; i < inputs.length; ++i) {
    input = inputs.item(i);

    if (v.isDefined(input.getAttribute("data-ignored"))) {
      continue;
    }

    value = v.sanitizeFormValue(input.value, options);
    if (input.type === "number") {
      value = value ? +value : null;
    } else if (input.type === "checkbox") {
      if (input.attributes.value) {
        if (!input.checked) {
          value = values[input.name] || null;
        }
      } else {
        value = input.checked;
      }
    } else if (input.type === "radio") {
      if (!input.checked) {
        value = values[input.name] || null;
      }
    }
    values[input.name] = value;
  }

  inputs = form.querySelectorAll("select[name]");
  for (i = 0; i < inputs.length; ++i) {
    input = inputs.item(i);
    if (input.multiple) {
      value = [];
      for (j in input.options) {
        option = input.options[j];
        if (option.selected) {
          value.push(v.sanitizeFormValue(option.value, options));
        }
      }
    } else {
      value = v.sanitizeFormValue(input.options[input.selectedIndex].value, options);
    }
    values[input.name] = value;
  }

  return values;
}
```
- example usage
```shell
...
  , value
  , validators
  , validator
  , validatorOptions
  , error;

if (v.isDomElement(attributes) || v.isJqueryElement(attributes)) {
  attributes = v.collectFormValues(attributes);
}

// Loops through each constraints, finds the correct validator and run it.
for (attr in constraints) {
  value = v.getDeepObjectValue(attributes, attr);
  // This allows the constraints for an attribute to be a function.
  // The function will be called with the value, attribute name, the complete dict of
...
```

#### <a name="apidoc.element.validate.js.contains"></a>[function <span class="apidocSignatureSpan">validate.js.</span>contains (obj, value)](#apidoc.element.validate.js.contains)
- description and source-code
```javascript
contains = function (obj, value) {
  if (!v.isDefined(obj)) {
    return false;
  }
  if (v.isArray(obj)) {
    return obj.indexOf(value) !== -1;
  }
  return value in obj;
}
```
- example usage
```shell
...
  if (!v.isDefined(value)) {
    return;
  }
  if (v.isArray(options)) {
    options = {within: options};
  }
  options = v.extend({}, this.options, options);
  if (v.contains(options.within, value)) {
    return;
  }
  var message = options.message ||
    this.message ||
    "^%{value} is not included in the list";
  return v.format(message, {value: value});
},
...
```

#### <a name="apidoc.element.validate.js.convertErrorMessages"></a>[function <span class="apidocSignatureSpan">validate.js.</span>convertErrorMessages (errors, options)](#apidoc.element.validate.js.convertErrorMessages)
- description and source-code
```javascript
convertErrorMessages = function (errors, options) {
  options = options || {};

  var ret = [];
  errors.forEach(function(errorInfo) {
    var error = v.result(errorInfo.error,
        errorInfo.value,
        errorInfo.attribute,
        errorInfo.options,
        errorInfo.attributes,
        errorInfo.globalOptions);

    if (!v.isString(error)) {
      ret.push(errorInfo);
      return;
    }

    if (error[0] === '^') {
      error = error.slice(1);
    } else if (options.fullMessages !== false) {
      error = v.capitalize(v.prettify(errorInfo.attribute)) + " " + error;
    }
    error = error.replace(/\\\^/g, "^");
    error = v.format(error, {value: v.stringifyValue(errorInfo.value)});
    ret.push(v.extend({}, errorInfo, {error: error}));
  });
  return ret;
}
```
- example usage
```shell
...
    },

    // Takes the output from runValidations and converts it to the correct
    // output format.
    processValidationResults: function(errors, options) {
errors = v.pruneEmptyErrors(errors, options);
errors = v.expandMultipleErrors(errors, options);
errors = v.convertErrorMessages(errors, options);

var format = options.format || "grouped";

if (typeof v.formatters[format] === 'function') {
  errors = v.formatters[format](errors);
} else {
  throw new Error(v.format("Unknown format %{format}", options));
...
```

#### <a name="apidoc.element.validate.js.error"></a>[function <span class="apidocSignatureSpan">validate.js.</span>error (msg)](#apidoc.element.validate.js.error)
- description and source-code
```javascript
error = function (msg) {
  if (typeof console !== "undefined" && console.error) {
    console.error("[validate.js] " + msg);
  }
}
```
- example usage
```shell
...
    if (typeof console !== "undefined" && console.warn) {
      console.warn("[validate.js] " + msg);
    }
  },

  error: function(msg) {
    if (typeof console !== "undefined" && console.error) {
      console.error("[validate.js] " + msg);
    }
  }
});

validate.validators = {
  // Presence validates that the value isn't empty
  presence: function(value, options) {
...
```

#### <a name="apidoc.element.validate.js.expandMultipleErrors"></a>[function <span class="apidocSignatureSpan">validate.js.</span>expandMultipleErrors (errors)](#apidoc.element.validate.js.expandMultipleErrors)
- description and source-code
```javascript
expandMultipleErrors = function (errors) {
  var ret = [];
  errors.forEach(function(error) {
    // Removes errors without a message
    if (v.isArray(error.error)) {
      error.error.forEach(function(msg) {
        ret.push(v.extend({}, error, {error: msg}));
      });
    } else {
      ret.push(error);
    }
  });
  return ret;
}
```
- example usage
```shell
...
return results;
    },

    // Takes the output from runValidations and converts it to the correct
    // output format.
    processValidationResults: function(errors, options) {
errors = v.pruneEmptyErrors(errors, options);
errors = v.expandMultipleErrors(errors, options);
errors = v.convertErrorMessages(errors, options);

var format = options.format || "grouped";

if (typeof v.formatters[format] === 'function') {
  errors = v.formatters[format](errors);
} else {
...
```

#### <a name="apidoc.element.validate.js.exposeModule"></a>[function <span class="apidocSignatureSpan">validate.js.</span>exposeModule (validate, root, exports, module, define)](#apidoc.element.validate.js.exposeModule)
- description and source-code
```javascript
exposeModule = function (validate, root, exports, module, define) {
  if (exports) {
    if (module && module.exports) {
      exports = module.exports = validate;
    }
    exports.validate = validate;
  } else {
    root.validate = validate;
    if (validate.isFunction(define) && define.amd) {
      define([], function () { return validate; });
    }
  }
}
```
- example usage
```shell
...
  return result.validator;
}).sort();
      }
      return errors;
    }
  };

  validate.exposeModule(validate, this, exports, module, define);
}).call(this,
typeof exports !== 'undefined' ? /* istanbul ignore next */ exports : null,
typeof module !== 'undefined' ? /* istanbul ignore next */ module : null,
typeof define !== 'undefined' ? /* istanbul ignore next */ define : null);
...
```

#### <a name="apidoc.element.validate.js.extend"></a>[function <span class="apidocSignatureSpan">validate.js.</span>extend (obj)](#apidoc.element.validate.js.extend)
- description and source-code
```javascript
extend = function (obj) {
  [].slice.call(arguments, 1).forEach(function(source) {
    for (var attr in source) {
      obj[attr] = source[attr];
    }
  });
  return obj;
}
```
- example usage
```shell
...
  //     * flat - Returns a flat array of just the error messages
  //     * grouped - Returns the messages grouped by attribute (default)
  //     * detailed - Returns an array of the raw validation data
  //   - fullMessages (boolean) - If 'true' (default) the attribute name is prepended to the error.
  //
  // Please note that the options are also passed to each validator.
  var validate = function(attributes, constraints, options) {
options = v.extend({}, v.options, options);

var results = v.runValidations(attributes, constraints, options)
  , attr
  , validator;

for (attr in results) {
  for (validator in results[attr]) {
...
```

#### <a name="apidoc.element.validate.js.flattenErrorsToArray"></a>[function <span class="apidocSignatureSpan">validate.js.</span>flattenErrorsToArray (errors)](#apidoc.element.validate.js.flattenErrorsToArray)
- description and source-code
```javascript
flattenErrorsToArray = function (errors) {
  return errors
    .map(function(error) { return error.error; })
    .filter(function(value, index, self) {
      return self.indexOf(value) === index;
    });
}
```
- example usage
```shell
...
detailed: function(errors) {return errors;},
flat: v.flattenErrorsToArray,
grouped: function(errors) {
  var attr;

  errors = v.groupErrorsByAttribute(errors);
  for (attr in errors) {
    errors[attr] = v.flattenErrorsToArray(errors[attr]);
  }
  return errors;
},
constraint: function(errors) {
  var attr;
  errors = v.groupErrorsByAttribute(errors);
  for (attr in errors) {
...
```

#### <a name="apidoc.element.validate.js.forEachKeyInKeypath"></a>[function <span class="apidocSignatureSpan">validate.js.</span>forEachKeyInKeypath (object, keypath, callback)](#apidoc.element.validate.js.forEachKeyInKeypath)
- description and source-code
```javascript
forEachKeyInKeypath = function (object, keypath, callback) {
  if (!v.isString(keypath)) {
    return undefined;
  }

  var key = ""
    , i
    , escape = false;

  for (i = 0; i < keypath.length; ++i) {
    switch (keypath[i]) {
      case '.':
        if (escape) {
          escape = false;
          key += '.';
        } else {
          object = callback(object, key, false);
          key = "";
        }
        break;

      case '\\':
        if (escape) {
          escape = false;
          key += '\\';
        } else {
          escape = true;
        }
        break;

      default:
        escape = false;
        key += keypath[i];
        break;
    }
  }

  return callback(object, key, true);
}
```
- example usage
```shell
...
},

getDeepObjectValue: function(obj, keypath) {
  if (!v.isObject(obj)) {
    return undefined;
  }

  return v.forEachKeyInKeypath(obj, keypath, function(obj, key) {
    if (v.isObject(obj)) {
      return obj[key];
    }
  });
},

// This returns an object with all the values of the form.
...
```

#### <a name="apidoc.element.validate.js.format"></a>[function <span class="apidocSignatureSpan">validate.js.</span>format (str, vals)](#apidoc.element.validate.js.format)
- description and source-code
```javascript
format = function (str, vals) {
  if (!v.isString(str)) {
    return str;
  }
  return str.replace(v.format.FORMAT_REGEXP, function(m0, m1, m2) {
    if (m1 === '%') {
      return "%{" + m2 + "}";
    } else {
      return String(vals[m2]);
    }
  });
}
```
- example usage
```shell
...
// The toString function will allow it to be coerced into a string
version: {
  major: 0,
  minor: 11,
  patch: 1,
  metadata: null,
  toString: function() {
    var version = v.format("%{major}.%{minor}.%{patch}", v.version);
    if (!v.isEmpty(v.version.metadata)) {
      version += "+" + v.version.metadata;
    }
    return version;
  }
},
...
```

#### <a name="apidoc.element.validate.js.getDeepObjectValue"></a>[function <span class="apidocSignatureSpan">validate.js.</span>getDeepObjectValue (obj, keypath)](#apidoc.element.validate.js.getDeepObjectValue)
- description and source-code
```javascript
getDeepObjectValue = function (obj, keypath) {
  if (!v.isObject(obj)) {
    return undefined;
  }

  return v.forEachKeyInKeypath(obj, keypath, function(obj, key) {
    if (v.isObject(obj)) {
      return obj[key];
    }
  });
}
```
- example usage
```shell
...

if (v.isDomElement(attributes) || v.isJqueryElement(attributes)) {
  attributes = v.collectFormValues(attributes);
}

// Loops through each constraints, finds the correct validator and run it.
for (attr in constraints) {
  value = v.getDeepObjectValue(attributes, attr);
  // This allows the constraints for an attribute to be a function.
  // The function will be called with the value, attribute name, the complete dict of
  // attributes as well as the options and constraints passed in.
  // This is useful when you want to have different
  // validations depending on the attribute value.
  validators = v.result(constraints[attr], value, attributes, attr, options, constraints);
...
```

#### <a name="apidoc.element.validate.js.groupErrorsByAttribute"></a>[function <span class="apidocSignatureSpan">validate.js.</span>groupErrorsByAttribute (errors)](#apidoc.element.validate.js.groupErrorsByAttribute)
- description and source-code
```javascript
groupErrorsByAttribute = function (errors) {
  var ret = {};
  errors.forEach(function(error) {
    var list = ret[error.attribute];
    if (list) {
      list.push(error);
    } else {
      ret[error.attribute] = [error];
    }
  });
  return ret;
}
```
- example usage
```shell
...

  validate.formatters = {
detailed: function(errors) {return errors;},
flat: v.flattenErrorsToArray,
grouped: function(errors) {
  var attr;

  errors = v.groupErrorsByAttribute(errors);
  for (attr in errors) {
    errors[attr] = v.flattenErrorsToArray(errors[attr]);
  }
  return errors;
},
constraint: function(errors) {
  var attr;
...
```

#### <a name="apidoc.element.validate.js.isArray"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isArray (value)](#apidoc.element.validate.js.isArray)
- description and source-code
```javascript
isArray = function (value) {
  return {}.toString.call(value) === '[object Array]';
}
```
- example usage
```shell
...

// Whitespace only strings are empty
if (v.isString(value)) {
  return v.EMPTY_STRING_REGEXP.test(value);
}

// For arrays we use the length property
if (v.isArray(value)) {
  return value.length === 0;
}

// Dates have no attributes but aren't empty
if (v.isDate(value)) {
  return false;
}
...
```

#### <a name="apidoc.element.validate.js.isBoolean"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isBoolean (value)](#apidoc.element.validate.js.isBoolean)
- description and source-code
```javascript
isBoolean = function (value) {
  return typeof value === 'boolean';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.isDate"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isDate (obj)](#apidoc.element.validate.js.isDate)
- description and source-code
```javascript
isDate = function (obj) {
  return obj instanceof Date;
}
```
- example usage
```shell
...

// For arrays we use the length property
if (v.isArray(value)) {
  return value.length === 0;
}

// Dates have no attributes but aren't empty
if (v.isDate(value)) {
  return false;
}

// If we find at least one property we consider it non empty
if (v.isObject(value)) {
  for (attr in value) {
    return false;
...
```

#### <a name="apidoc.element.validate.js.isDefined"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isDefined (obj)](#apidoc.element.validate.js.isDefined)
- description and source-code
```javascript
isDefined = function (obj) {
  return obj !== null && obj !== undefined;
}
```
- example usage
```shell
...
}
    },

    isEmpty: function(value) {
var attr;

// Null and undefined are empty
if (!v.isDefined(value)) {
  return true;
}

// functions are non empty
if (v.isFunction(value)) {
  return false;
}
...
```

#### <a name="apidoc.element.validate.js.isDomElement"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isDomElement (o)](#apidoc.element.validate.js.isDomElement)
- description and source-code
```javascript
isDomElement = function (o) {
  if (!o) {
    return false;
  }

  if (!o.querySelectorAll || !o.querySelector) {
    return false;
  }

  if (v.isObject(document) && o === document) {
    return true;
  }

  // http://stackoverflow.com/a/384380/699304
<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof HTMLElement === "object") {
    return o instanceof HTMLElement;
  } else {
    return o &&
      typeof o === "object" &&
      o !== null &&
      o.nodeType === 1 &&
      typeof o.nodeName === "string";
  }
}
```
- example usage
```shell
...
  , validatorName
  , value
  , validators
  , validator
  , validatorOptions
  , error;

if (v.isDomElement(attributes) || v.isJqueryElement(attributes)) {
  attributes = v.collectFormValues(attributes);
}

// Loops through each constraints, finds the correct validator and run it.
for (attr in constraints) {
  value = v.getDeepObjectValue(attributes, attr);
  // This allows the constraints for an attribute to be a function.
...
```

#### <a name="apidoc.element.validate.js.isEmpty"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isEmpty (value)](#apidoc.element.validate.js.isEmpty)
- description and source-code
```javascript
isEmpty = function (value) {
  var attr;

  // Null and undefined are empty
  if (!v.isDefined(value)) {
    return true;
  }

  // functions are non empty
  if (v.isFunction(value)) {
    return false;
  }

  // Whitespace only strings are empty
  if (v.isString(value)) {
    return v.EMPTY_STRING_REGEXP.test(value);
  }

  // For arrays we use the length property
  if (v.isArray(value)) {
    return value.length === 0;
  }

  // Dates have no attributes but aren't empty
  if (v.isDate(value)) {
    return false;
  }

  // If we find at least one property we consider it non empty
  if (v.isObject(value)) {
    for (attr in value) {
      return false;
    }
    return true;
  }

  return false;
}
```
- example usage
```shell
...
version: {
  major: 0,
  minor: 11,
  patch: 1,
  metadata: null,
  toString: function() {
    var version = v.format("%{major}.%{minor}.%{patch}", v.version);
    if (!v.isEmpty(v.version.metadata)) {
      version += "+" + v.version.metadata;
    }
    return version;
  }
},

// Below is the dependencies that are used in validate.js
...
```

#### <a name="apidoc.element.validate.js.isFunction"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isFunction (value)](#apidoc.element.validate.js.isFunction)
- description and source-code
```javascript
isFunction = function (value) {
  return typeof value === 'function';
}
```
- example usage
```shell
...
isDefined: function(obj) {
  return obj !== null && obj !== undefined;
},

// Checks if the given argument is a promise. Anything with a 'then'
// function is considered a promise.
isPromise: function(p) {
  return !!p && v.isFunction(p.then);
},

isJqueryElement: function(o) {
  return o && v.isString(o.jquery);
},

isDomElement: function(o) {
...
```

#### <a name="apidoc.element.validate.js.isHash"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isHash (value)](#apidoc.element.validate.js.isHash)
- description and source-code
```javascript
isHash = function (value) {
  return v.isObject(value) && !v.isArray(value) && !v.isFunction(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.isInteger"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isInteger (value)](#apidoc.element.validate.js.isInteger)
- description and source-code
```javascript
isInteger = function (value) {
  return v.isNumber(value) && value % 1 === 0;
}
```
- example usage
```shell
...
    this.notValid ||
    this.message ||
    "is not a number";
}

// Same logic as above, sort of. Don't bother with comparisons if this
// doesn't pass.
if (options.onlyInteger && !v.isInteger(value)) {
  return options.message ||
    options.notInteger ||
    this.notInteger ||
    this.message ||
    "must be an integer";
}
...
```

#### <a name="apidoc.element.validate.js.isJqueryElement"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isJqueryElement (o)](#apidoc.element.validate.js.isJqueryElement)
- description and source-code
```javascript
isJqueryElement = function (o) {
  return o && v.isString(o.jquery);
}
```
- example usage
```shell
...
  , validatorName
  , value
  , validators
  , validator
  , validatorOptions
  , error;

if (v.isDomElement(attributes) || v.isJqueryElement(attributes)) {
  attributes = v.collectFormValues(attributes);
}

// Loops through each constraints, finds the correct validator and run it.
for (attr in constraints) {
  value = v.getDeepObjectValue(attributes, attr);
  // This allows the constraints for an attribute to be a function.
...
```

#### <a name="apidoc.element.validate.js.isNumber"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isNumber (value)](#apidoc.element.validate.js.isNumber)
- description and source-code
```javascript
isNumber = function (value) {
  return typeof value === 'number' && !isNaN(value);
}
```
- example usage
```shell
...
isFunction: function(value) {
  return typeof value === 'function';
},

// A simple check to verify that the value is an integer. Uses 'isNumber'
// and a simple modulo check.
isInteger: function(value) {
  return v.isNumber(value) && value % 1 === 0;
},

// Checks if the value is a boolean
isBoolean: function(value) {
  return typeof value === 'boolean';
},
...
```

#### <a name="apidoc.element.validate.js.isObject"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isObject (obj)](#apidoc.element.validate.js.isObject)
- description and source-code
```javascript
isObject = function (obj) {
  return obj === Object(obj);
}
```
- example usage
```shell
...
  return false;
}

if (!o.querySelectorAll || !o.querySelector) {
  return false;
}

if (v.isObject(document) && o === document) {
  return true;
}

// http://stackoverflow.com/a/384380/699304
/* istanbul ignore else */
if (typeof HTMLElement === "object") {
  return o instanceof HTMLElement;
...
```

#### <a name="apidoc.element.validate.js.isPromise"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isPromise (p)](#apidoc.element.validate.js.isPromise)
- description and source-code
```javascript
isPromise = function (p) {
  return !!p && v.isFunction(p.then);
}
```
- example usage
```shell
...

  var results = v.runValidations(attributes, constraints, options)
    , attr
    , validator;

  for (attr in results) {
    for (validator in results[attr]) {
      if (v.isPromise(results[attr][validator])) {
        throw new Error("Use validate.async if you want support for promises");
      }
    }
  }
  return validate.processValidationResults(results, options);
};
...
```

#### <a name="apidoc.element.validate.js.isString"></a>[function <span class="apidocSignatureSpan">validate.js.</span>isString (value)](#apidoc.element.validate.js.isString)
- description and source-code
```javascript
isString = function (value) {
  return typeof value === 'string';
}
```
- example usage
```shell
...
// Checks if the given argument is a promise. Anything with a 'then'
// function is considered a promise.
isPromise: function(p) {
  return !!p && v.isFunction(p.then);
},

isJqueryElement: function(o) {
  return o && v.isString(o.jquery);
},

isDomElement: function(o) {
  if (!o) {
    return false;
  }
...
```

#### <a name="apidoc.element.validate.js.prettify"></a>[function <span class="apidocSignatureSpan">validate.js.</span>prettify (str)](#apidoc.element.validate.js.prettify)
- description and source-code
```javascript
prettify = function (str) {
  if (v.isNumber(str)) {
    // If there are more than 2 decimals round it to two
    if ((str * 100) % 1 === 0) {
      return "" + str;
    } else {
      return parseFloat(Math.round(str * 100) / 100).toFixed(2);
    }
  }

  if (v.isArray(str)) {
    return str.map(function(s) { return v.prettify(s); }).join(", ");
  }

  if (v.isObject(str)) {
    return str.toString();
  }

  // Ensure the string is actually a string
  str = "" + str;

  return str
    // Splits keys separated by periods
    .replace(/([^\s])\.([^\s])/g, '$1 $2')
    // Removes backslashes
    .replace(/\\+/g, '')
    // Replaces - and - with space
    .replace(/[_-]/g, ' ')
    // Splits camel cased words
    .replace(/([a-z])([A-Z])/g, function(m0, m1, m2) {
      return "" + m1 + " " + m2.toLowerCase();
    })
    .toLowerCase();
}
```
- example usage
```shell
...
    return "" + str;
  } else {
    return parseFloat(Math.round(str * 100) / 100).toFixed(2);
  }
}

if (v.isArray(str)) {
  return str.map(function(s) { return v.prettify(s); }).join(", ");
}

if (v.isObject(str)) {
  return str.toString();
}

// Ensure the string is actually a string
...
```

#### <a name="apidoc.element.validate.js.processValidationResults"></a>[function <span class="apidocSignatureSpan">validate.js.</span>processValidationResults (errors, options)](#apidoc.element.validate.js.processValidationResults)
- description and source-code
```javascript
processValidationResults = function (errors, options) {
  errors = v.pruneEmptyErrors(errors, options);
  errors = v.expandMultipleErrors(errors, options);
  errors = v.convertErrorMessages(errors, options);

  var format = options.format || "grouped";

  if (typeof v.formatters[format] === 'function') {
    errors = v.formatters[format](errors);
  } else {
    throw new Error(v.format("Unknown format %{format}", options));
  }

  return v.isEmpty(errors) ? undefined : errors;
}
```
- example usage
```shell
...
  for (attr in results) {
    for (validator in results[attr]) {
      if (v.isPromise(results[attr][validator])) {
        throw new Error("Use validate.async if you want support for promises");
      }
    }
  }
  return validate.processValidationResults(results, options);
};

var v = validate;

// Copies over attributes from one or more sources to a single destination.
// Very much similar to underscore's extend.
// The first argument is the target object and the remaining arguments will be
...
```

#### <a name="apidoc.element.validate.js.pruneEmptyErrors"></a>[function <span class="apidocSignatureSpan">validate.js.</span>pruneEmptyErrors (errors)](#apidoc.element.validate.js.pruneEmptyErrors)
- description and source-code
```javascript
pruneEmptyErrors = function (errors) {
  return errors.filter(function(error) {
    return !v.isEmpty(error.error);
  });
}
```
- example usage
```shell
...

return results;
    },

    // Takes the output from runValidations and converts it to the correct
    // output format.
    processValidationResults: function(errors, options) {
errors = v.pruneEmptyErrors(errors, options);
errors = v.expandMultipleErrors(errors, options);
errors = v.convertErrorMessages(errors, options);

var format = options.format || "grouped";

if (typeof v.formatters[format] === 'function') {
  errors = v.formatters[format](errors);
...
```

#### <a name="apidoc.element.validate.js.result"></a>[function <span class="apidocSignatureSpan">validate.js.</span>result (value)](#apidoc.element.validate.js.result)
- description and source-code
```javascript
result = function (value) {
  var args = [].slice.call(arguments, 1);
  if (typeof value === 'function') {
    value = value.apply(null, args);
  }
  return value;
}
```
- example usage
```shell
...
      for (attr in constraints) {
        value = v.getDeepObjectValue(attributes, attr);
        // This allows the constraints for an attribute to be a function.
        // The function will be called with the value, attribute name, the complete dict of
        // attributes as well as the options and constraints passed in.
        // This is useful when you want to have different
        // validations depending on the attribute value.
        validators = v.result(constraints[attr], value, attributes, attr, options, constraints);

        for (validatorName in validators) {
validator = v.validators[validatorName];

if (!validator) {
  error = v.format("Unknown validator %{name}", {name: validatorName});
  throw new Error(error);
...
```

#### <a name="apidoc.element.validate.js.runValidations"></a>[function <span class="apidocSignatureSpan">validate.js.</span>runValidations (attributes, constraints, options)](#apidoc.element.validate.js.runValidations)
- description and source-code
```javascript
runValidations = function (attributes, constraints, options) {
  var results = []
    , attr
    , validatorName
    , value
    , validators
    , validator
    , validatorOptions
    , error;

  if (v.isDomElement(attributes) || v.isJqueryElement(attributes)) {
    attributes = v.collectFormValues(attributes);
  }

  // Loops through each constraints, finds the correct validator and run it.
  for (attr in constraints) {
    value = v.getDeepObjectValue(attributes, attr);
    // This allows the constraints for an attribute to be a function.
    // The function will be called with the value, attribute name, the complete dict of
    // attributes as well as the options and constraints passed in.
    // This is useful when you want to have different
    // validations depending on the attribute value.
    validators = v.result(constraints[attr], value, attributes, attr, options, constraints);

    for (validatorName in validators) {
      validator = v.validators[validatorName];

      if (!validator) {
        error = v.format("Unknown validator %{name}", {name: validatorName});
        throw new Error(error);
      }

      validatorOptions = validators[validatorName];
      // This allows the options to be a function. The function will be
      // called with the value, attribute name, the complete dict of
      // attributes as well as the options and constraints passed in.
      // This is useful when you want to have different
      // validations depending on the attribute value.
      validatorOptions = v.result(validatorOptions, value, attributes, attr, options, constraints);
      if (!validatorOptions) {
        continue;
      }
      results.push({
        attribute: attr,
        value: value,
        validator: validatorName,
        globalOptions: options,
        attributes: attributes,
        options: validatorOptions,
        error: validator.call(validator,
            value,
            validatorOptions,
            attr,
            attributes,
            options)
      });
    }
  }

  return results;
}
```
- example usage
```shell
...
  //     * detailed - Returns an array of the raw validation data
  //   - fullMessages (boolean) - If 'true' (default) the attribute name is prepended to the error.
  //
  // Please note that the options are also passed to each validator.
  var validate = function(attributes, constraints, options) {
options = v.extend({}, v.options, options);

var results = v.runValidations(attributes, constraints, options)
  , attr
  , validator;

for (attr in results) {
  for (validator in results[attr]) {
    if (v.isPromise(results[attr][validator])) {
      throw new Error("Use validate.async if you want support for promises");
...
```

#### <a name="apidoc.element.validate.js.sanitizeFormValue"></a>[function <span class="apidocSignatureSpan">validate.js.</span>sanitizeFormValue (value, options)](#apidoc.element.validate.js.sanitizeFormValue)
- description and source-code
```javascript
sanitizeFormValue = function (value, options) {
  if (options.trim && v.isString(value)) {
    value = value.trim();
  }

  if (options.nullify !== false && value === "") {
    return null;
  }
  return value;
}
```
- example usage
```shell
...
      for (i = 0; i < inputs.length; ++i) {
input = inputs.item(i);

if (v.isDefined(input.getAttribute("data-ignored"))) {
  continue;
}

value = v.sanitizeFormValue(input.value, options);
if (input.type === "number") {
  value = value ? +value : null;
} else if (input.type === "checkbox") {
  if (input.attributes.value) {
    if (!input.checked) {
      value = values[input.name] || null;
    }
...
```

#### <a name="apidoc.element.validate.js.single"></a>[function <span class="apidocSignatureSpan">validate.js.</span>single (value, constraints, options)](#apidoc.element.validate.js.single)
- description and source-code
```javascript
single = function (value, constraints, options) {
  options = v.extend({}, v.single.options, options, {
    format: "flat",
    fullMessages: false
  });
  return v({single: value}, {single: constraints}, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.stringifyValue"></a>[function <span class="apidocSignatureSpan">validate.js.</span>stringifyValue (value)](#apidoc.element.validate.js.stringifyValue)
- description and source-code
```javascript
stringifyValue = function (value) {
  return v.prettify(value);
}
```
- example usage
```shell
...

    if (error[0] === '^') {
      error = error.slice(1);
    } else if (options.fullMessages !== false) {
      error = v.capitalize(v.prettify(errorInfo.attribute)) + " " + error;
    }
    error = error.replace(/\\\^/g, "^");
    error = v.format(error, {value: v.stringifyValue(errorInfo.value)});
    ret.push(v.extend({}, errorInfo, {error: error}));
  });
  return ret;
},

// In:
// [{attribute: "<attributeName>", ...}]
...
```

#### <a name="apidoc.element.validate.js.unique"></a>[function <span class="apidocSignatureSpan">validate.js.</span>unique (array)](#apidoc.element.validate.js.unique)
- description and source-code
```javascript
unique = function (array) {
  if (!v.isArray(array)) {
    return array;
  }
  return array.filter(function(el, index, array) {
    return array.indexOf(el) == index;
  });
}
```
- example usage
```shell
...
      date: this.format(latest, options),
      value: this.format(value, options)
    });
    errors.push(err);
  }

  if (errors.length) {
    return v.unique(errors);
  }
}, {
  parse: null,
  format: null
}),
date: function(value, options) {
  options = v.extend({}, options, {dateOnly: true});
...
```

#### <a name="apidoc.element.validate.js.validate"></a>[function <span class="apidocSignatureSpan">validate.js.</span>validate (attributes, constraints, options)](#apidoc.element.validate.js.validate)
- description and source-code
```javascript
validate = function (attributes, constraints, options) {
  options = v.extend({}, v.options, options);

  var results = v.runValidations(attributes, constraints, options)
    , attr
    , validator;

  for (attr in results) {
    for (validator in results[attr]) {
      if (v.isPromise(results[attr][validator])) {
        throw new Error("Use validate.async if you want support for promises");
      }
    }
  }
  return validate.processValidationResults(results, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.waitForResults"></a>[function <span class="apidocSignatureSpan">validate.js.</span>waitForResults (results)](#apidoc.element.validate.js.waitForResults)
- description and source-code
```javascript
waitForResults = function (results) {
  // Create a sequence of all the results starting with a resolved promise.
  return results.reduce(function(memo, result) {
    // If this result isn't a promise skip it in the sequence.
    if (!v.isPromise(result.error)) {
      return memo;
    }

    return memo.then(function() {
      return result.error.then(function(error) {
        result.error = error || null;
      });
    });
  }, new v.Promise(function(r) { r(); })); // A resolved promise
}
```
- example usage
```shell
...
if (options.cleanAttributes !== false) {
  attributes = v.cleanAttributes(attributes, constraints);
}

var results = v.runValidations(attributes, constraints, options);

return new v.Promise(function(resolve, reject) {
  v.waitForResults(results).then(function() {
    var errors = v.processValidationResults(results, options);
    if (errors) {
      reject(new WrapErrors(errors, options, attributes, constraints));
    } else {
      resolve(attributes);
    }
  }, function(err) {
...
```

#### <a name="apidoc.element.validate.js.warn"></a>[function <span class="apidocSignatureSpan">validate.js.</span>warn (msg)](#apidoc.element.validate.js.warn)
- description and source-code
```javascript
warn = function (msg) {
  if (typeof console !== "undefined" && console.warn) {
    console.warn("[validate.js] " + msg);
  }
}
```
- example usage
```shell
...
      define([], function () { return validate; });
    }
  }
},

warn: function(msg) {
  if (typeof console !== "undefined" && console.warn) {
    console.warn("[validate.js] " + msg);
  }
},

error: function(msg) {
  if (typeof console !== "undefined" && console.error) {
    console.error("[validate.js] " + msg);
  }
...
```



# <a name="apidoc.module.validate.js.formatters"></a>[module validate.js.formatters](#apidoc.module.validate.js.formatters)

#### <a name="apidoc.element.validate.js.formatters.constraint"></a>[function <span class="apidocSignatureSpan">validate.js.formatters.</span>constraint (errors)](#apidoc.element.validate.js.formatters.constraint)
- description and source-code
```javascript
constraint = function (errors) {
  var attr;
  errors = v.groupErrorsByAttribute(errors);
  for (attr in errors) {
    errors[attr] = errors[attr].map(function(result) {
      return result.validator;
    }).sort();
  }
  return errors;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.formatters.detailed"></a>[function <span class="apidocSignatureSpan">validate.js.formatters.</span>detailed (errors)](#apidoc.element.validate.js.formatters.detailed)
- description and source-code
```javascript
detailed = function (errors) {return errors;}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.formatters.flat"></a>[function <span class="apidocSignatureSpan">validate.js.formatters.</span>flat (errors)](#apidoc.element.validate.js.formatters.flat)
- description and source-code
```javascript
flat = function (errors) {
  return errors
    .map(function(error) { return error.error; })
    .filter(function(value, index, self) {
      return self.indexOf(value) === index;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.formatters.grouped"></a>[function <span class="apidocSignatureSpan">validate.js.formatters.</span>grouped (errors)](#apidoc.element.validate.js.formatters.grouped)
- description and source-code
```javascript
grouped = function (errors) {
  var attr;

  errors = v.groupErrorsByAttribute(errors);
  for (attr in errors) {
    errors[attr] = v.flattenErrorsToArray(errors[attr]);
  }
  return errors;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validate.js.validators"></a>[module validate.js.validators](#apidoc.module.validate.js.validators)

#### <a name="apidoc.element.validate.js.validators.date"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>date (value, options)](#apidoc.element.validate.js.validators.date)
- description and source-code
```javascript
date = function (value, options) {
  options = v.extend({}, options, {dateOnly: true});
  return v.validators.datetime.call(v.validators.datetime, value, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.datetime"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>datetime (value, options)](#apidoc.element.validate.js.validators.datetime)
- description and source-code
```javascript
datetime = function (value, options) {
  if (!v.isFunction(this.parse) || !v.isFunction(this.format)) {
    throw new Error("Both the parse and format functions needs to be set to use the datetime/date validator");
  }

  // Empty values are fine
  if (!v.isDefined(value)) {
    return;
  }

  options = v.extend({}, this.options, options);

  var err
    , errors = []
    , earliest = options.earliest ? this.parse(options.earliest, options) : NaN
    , latest = options.latest ? this.parse(options.latest, options) : NaN;

  value = this.parse(value, options);

  // 86400000 is the number of seconds in a day, this is used to remove
  // the time from the date
  if (isNaN(value) || options.dateOnly && value % 86400000 !== 0) {
    err = options.notValid ||
      options.message ||
      this.notValid ||
      "must be a valid date";
    return v.format(err, {value: arguments[0]});
  }

  if (!isNaN(earliest) && value < earliest) {
    err = options.tooEarly ||
      options.message ||
      this.tooEarly ||
      "must be no earlier than %{date}";
    err = v.format(err, {
      value: this.format(value, options),
      date: this.format(earliest, options)
    });
    errors.push(err);
  }

  if (!isNaN(latest) && value > latest) {
    err = options.tooLate ||
      options.message ||
      this.tooLate ||
      "must be no later than %{date}";
    err = v.format(err, {
      date: this.format(latest, options),
      value: this.format(value, options)
    });
    errors.push(err);
  }

  if (errors.length) {
    return v.unique(errors);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.email"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>email (value, options)](#apidoc.element.validate.js.validators.email)
- description and source-code
```javascript
email = function (value, options) {
  options = v.extend({}, this.options, options);
  var message = options.message || this.message || "is not a valid email";
  // Empty values are fine
  if (!v.isDefined(value)) {
    return;
  }
  if (!v.isString(value)) {
    return message;
  }
  if (!this.PATTERN.exec(value)) {
    return message;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.equality"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>equality (value, options, attribute, attributes)](#apidoc.element.validate.js.validators.equality)
- description and source-code
```javascript
equality = function (value, options, attribute, attributes) {
  if (!v.isDefined(value)) {
    return;
  }

  if (v.isString(options)) {
    options = {attribute: options};
  }
  options = v.extend({}, this.options, options);
  var message = options.message ||
    this.message ||
    "is not equal to %{attribute}";

  if (v.isEmpty(options.attribute) || !v.isString(options.attribute)) {
    throw new Error("The attribute must be a non empty string");
  }

  var otherValue = v.getDeepObjectValue(attributes, options.attribute)
    , comparator = options.comparator || function(v1, v2) {
      return v1 === v2;
    };

  if (!comparator(value, otherValue, options, attribute, attributes)) {
    return v.format(message, {attribute: v.prettify(options.attribute)});
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.exclusion"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>exclusion (value, options)](#apidoc.element.validate.js.validators.exclusion)
- description and source-code
```javascript
exclusion = function (value, options) {
  // Empty values are fine
  if (!v.isDefined(value)) {
    return;
  }
  if (v.isArray(options)) {
    options = {within: options};
  }
  options = v.extend({}, this.options, options);
  if (!v.contains(options.within, value)) {
    return;
  }
  var message = options.message || this.message || "^%{value} is restricted";
  return v.format(message, {value: value});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.format"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>format (value, options)](#apidoc.element.validate.js.validators.format)
- description and source-code
```javascript
format = function (value, options) {
  if (v.isString(options) || (options instanceof RegExp)) {
    options = {pattern: options};
  }

  options = v.extend({}, this.options, options);

  var message = options.message || this.message || "is invalid"
    , pattern = options.pattern
    , match;

  // Empty values are allowed
  if (!v.isDefined(value)) {
    return;
  }
  if (!v.isString(value)) {
    return message;
  }

  if (v.isString(pattern)) {
    pattern = new RegExp(options.pattern, options.flags);
  }
  match = pattern.exec(value);
  if (!match || match[0].length != value.length) {
    return message;
  }
}
```
- example usage
```shell
...
// The toString function will allow it to be coerced into a string
version: {
  major: 0,
  minor: 11,
  patch: 1,
  metadata: null,
  toString: function() {
    var version = v.format("%{major}.%{minor}.%{patch}", v.version);
    if (!v.isEmpty(v.version.metadata)) {
      version += "+" + v.version.metadata;
    }
    return version;
  }
},
...
```

#### <a name="apidoc.element.validate.js.validators.inclusion"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>inclusion (value, options)](#apidoc.element.validate.js.validators.inclusion)
- description and source-code
```javascript
inclusion = function (value, options) {
  // Empty values are fine
  if (!v.isDefined(value)) {
    return;
  }
  if (v.isArray(options)) {
    options = {within: options};
  }
  options = v.extend({}, this.options, options);
  if (v.contains(options.within, value)) {
    return;
  }
  var message = options.message ||
    this.message ||
    "^%{value} is not included in the list";
  return v.format(message, {value: value});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.length"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>length (value, options, attribute)](#apidoc.element.validate.js.validators.length)
- description and source-code
```javascript
length = function (value, options, attribute) {
  // Empty values are allowed
  if (!v.isDefined(value)) {
    return;
  }

  options = v.extend({}, this.options, options);

  var is = options.is
    , maximum = options.maximum
    , minimum = options.minimum
    , tokenizer = options.tokenizer || function(val) { return val; }
    , err
    , errors = [];

  value = tokenizer(value);
  var length = value.length;
  if(!v.isNumber(length)) {
    v.error(v.format("Attribute %{attr} has a non numeric value for 'length'", {attr: attribute}));
    return options.message || this.notValid || "has an incorrect length";
  }

  // Is checks
  if (v.isNumber(is) && length !== is) {
    err = options.wrongLength ||
      this.wrongLength ||
      "is the wrong length (should be %{count} characters)";
    errors.push(v.format(err, {count: is}));
  }

  if (v.isNumber(minimum) && length < minimum) {
    err = options.tooShort ||
      this.tooShort ||
      "is too short (minimum is %{count} characters)";
    errors.push(v.format(err, {count: minimum}));
  }

  if (v.isNumber(maximum) && length > maximum) {
    err = options.tooLong ||
      this.tooLong ||
      "is too long (maximum is %{count} characters)";
    errors.push(v.format(err, {count: maximum}));
  }

  if (errors.length > 0) {
    return options.message || errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.numericality"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>numericality (value, options)](#apidoc.element.validate.js.validators.numericality)
- description and source-code
```javascript
numericality = function (value, options) {
  // Empty values are fine
  if (!v.isDefined(value)) {
    return;
  }

  options = v.extend({}, this.options, options);

  var errors = []
    , name
    , count
    , checks = {
        greaterThan:          function(v, c) { return v > c; },
        greaterThanOrEqualTo: function(v, c) { return v >= c; },
        equalTo:              function(v, c) { return v === c; },
        lessThan:             function(v, c) { return v < c; },
        lessThanOrEqualTo:    function(v, c) { return v <= c; },
        divisibleBy:          function(v, c) { return v % c === 0; }
      };

  // Strict will check that it is a valid looking number
  if (v.isString(value) && options.strict) {
    var pattern = "^(0|[1-9]\\d*)";
    if (!options.onlyInteger) {
      pattern += "(\\.\\d+)?";
    }
    pattern += "$";

    if (!(new RegExp(pattern).test(value))) {
      return options.message ||
        options.notValid ||
        this.notValid ||
        this.message ||
        "must be a valid number";
    }
  }

  // Coerce the value to a number unless we're being strict.
  if (options.noStrings !== true && v.isString(value) && !v.isEmpty(value)) {
    value = +value;
  }

  // If it's not a number we shouldn't continue since it will compare it.
  if (!v.isNumber(value)) {
    return options.message ||
      options.notValid ||
      this.notValid ||
      this.message ||
      "is not a number";
  }

  // Same logic as above, sort of. Don't bother with comparisons if this
  // doesn't pass.
  if (options.onlyInteger && !v.isInteger(value)) {
    return options.message ||
      options.notInteger ||
      this.notInteger ||
      this.message ||
      "must be an integer";
  }

  for (name in checks) {
    count = options[name];
    if (v.isNumber(count) && !checks[name](value, count)) {
      // This picks the default message if specified
      // For example the greaterThan check uses the message from
      // this.notGreaterThan so we capitalize the name and prepend "not"
      var key = "not" + v.capitalize(name);
      var msg = options[key] ||
        this[key] ||
        this.message ||
        "must be %{type} %{count}";

      errors.push(v.format(msg, {
        count: count,
        type: v.prettify(name)
      }));
    }
  }

  if (options.odd && value % 2 !== 1) {
    errors.push(options.notOdd ||
        this.notOdd ||
        this.message ||
        "must be odd");
  }
  if (options.even && value % 2 !== 0) {
    errors.push(options.notEven ||
        this.notEven ||
        this.message ||
        "must be even");
  }

  if (errors.length) {
    return options.message || errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.presence"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>presence (value, options)](#apidoc.element.validate.js.validators.presence)
- description and source-code
```javascript
presence = function (value, options) {
  options = v.extend({}, this.options, options);
  if (options.allowEmpty ? !v.isDefined(value) : v.isEmpty(value)) {
    return options.message || this.message || "can't be blank";
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.validate.js.validators.url"></a>[function <span class="apidocSignatureSpan">validate.js.validators.</span>url (value, options)](#apidoc.element.validate.js.validators.url)
- description and source-code
```javascript
url = function (value, options) {
  if (!v.isDefined(value)) {
    return;
  }

  options = v.extend({}, this.options, options);

  var message = options.message || this.message || "is not a valid url"
    , schemes = options.schemes || this.schemes || ['http', 'https']
    , allowLocal = options.allowLocal || this.allowLocal || false;

  if (!v.isString(value)) {
    return message;
  }

  // https://gist.github.com/dperini/729294
  var regex =
    "^" +
    // protocol identifier
    "(?:(?:" + schemes.join("|") + ")://)" +
    // user:pass authentication
    "(?:\\S+(?::\\S*)?@)?" +
    "(?:";

  var tld = "(?:\\.(?:[a-z\\u00a1-\\uffff]{2,}))";

  if (allowLocal) {
    tld += "?";
  } else {
    regex +=
      // IP address exclusion
      // private & local networks
      "(?!(?:10|127)(?:\\.\\d{1,3}){3})" +
      "(?!(?:169\\.254|192\\.168)(?:\\.\\d{1,3}){2})" +
      "(?!172\\.(?:1[6-9]|2\\d|3[0-1])(?:\\.\\d{1,3}){2})";
  }

  regex +=
      // IP address dotted notation octets
      // excludes loopback network 0.0.0.0
      // excludes reserved space >= 224.0.0.0
      // excludes network & broacast addresses
      // (first & last IP address of each class)
      "(?:[1-9]\\d?|1\\d\\d|2[01]\\d|22[0-3])" +
      "(?:\\.(?:1?\\d{1,2}|2[0-4]\\d|25[0-5])){2}" +
      "(?:\\.(?:[1-9]\\d?|1\\d\\d|2[0-4]\\d|25[0-4]))" +
    "|" +
      // host name
      "(?:(?:[a-z\\u00a1-\\uffff0-9]-*)*[a-z\\u00a1-\\uffff0-9]+)" +
      // domain name
      "(?:\\.(?:[a-z\\u00a1-\\uffff0-9]-*)*[a-z\\u00a1-\\uffff0-9]+)*" +
      tld +
    ")" +
    // port number
    "(?::\\d{2,5})?" +
    // resource path
    "(?:[/?#]\\S*)?" +
  "$";

  var PATTERN = new RegExp(regex, 'i');
  if (!PATTERN.exec(value)) {
    return message;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.validate.js.version"></a>[module validate.js.version](#apidoc.module.validate.js.version)

#### <a name="apidoc.element.validate.js.version.toString"></a>[function <span class="apidocSignatureSpan">validate.js.version.</span>toString ()](#apidoc.element.validate.js.version.toString)
- description and source-code
```javascript
toString = function () {
  var version = v.format("%{major}.%{minor}.%{patch}", v.version);
  if (!v.isEmpty(v.version.metadata)) {
    version += "+" + v.version.metadata;
  }
  return version;
}
```
- example usage
```shell
...
}

if (v.isArray(str)) {
  return str.map(function(s) { return v.prettify(s); }).join(", ");
}

if (v.isObject(str)) {
  return str.toString();
}

// Ensure the string is actually a string
str = "" + str;

return str
  // Splits keys separated by periods
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
