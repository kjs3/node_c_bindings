### Playing with Node C bindings and [node-gyp] [1] 

Make sure you have node-gyp installed

``` bash
$ npm install -g node-gyp
```

For node-gyp you also need:

  * `python` (`v2.7` recommended, `v3.x.x` is __*not*__ supported)
  * `make`
  * C/C++ compiler toolchain, like GCC


To compile:

``` bash
$ node-gyp configure
```

Then:

``` bash
$ node-gyp build
```

Now you can require in your node files like normal:

```javascript
var binding = require('./build/Release/binding');
```

[1]: https://github.com/TooTallNate/node-gyp "node-gyp"
