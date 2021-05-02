# widecore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install widecore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var widecoreTasks = require('widecore-build');

widecoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var widecoreTasks = require('widecore-build');
widecoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/widecoin-project/widecore) on the main widecore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/litecoin-project/litecore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2020 The Widecoin Core Developers

