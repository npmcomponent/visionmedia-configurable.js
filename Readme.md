*This repository is a mirror of the [component](http://component.io) module [visionmedia/configurable.js](http://github.com/visionmedia/configurable.js). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/visionmedia-configurable.js`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# configurable

  Configuration mixin.

## API

 Make something configurable:

```js
var Configurable = require('configurable');

// plain obj
var obj = {};
Configurable(obj);

// returns the obj itself
var obj = Configurable({});

// make a prototype configurable
Configurable(MyThing.prototype);
```

The object will then have the following methods available:

```js
.get(name)
.set(name, val)
.set(obj)
.enable(name)
.disable(name)
.enabled(name)
.disabled(name)
```

__NOTE__: when assigning to a `.prototype` make sure to re-define `.settings = {}`
in the constructor so objects do not share these values.

## License 

(The MIT License)

Copyright (c) 2012 TJ Holowaychuk &lt;tj@vision-media.ca&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.