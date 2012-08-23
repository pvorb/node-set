[![build status](https://secure.travis-ci.org/pvorb/node-set.png)](http://travis-ci.org/pvorb/node-set)
# Set

string sets for javascript

This library can be used as a shim for [EcmaScript Harmony’s Set
class](http://wiki.ecmascript.org/doku.php?id=harmony:simple_maps_and_sets#set).

## Installation

For the server:

```
npm install Set
```

For the browser:

```
ender build Set
```

## Usage

```js
var Set = require('Set');

var alpha = new Set([ 'a', 'b', 'c' ]);

console.log(alpha.toString());

alpha.add('d');

console.log(alpha.toString());

alpha.remove('a', 'b');

console.log(alpha.toString());

console.log(alpha.contains('c'));
```

## API

```js
Set(obj)
```

Create a set from an array or object.

```js
set.add(val, ...)
```

Add one or more elements to the set.

```js
set.addAll(array)
```

Add all elements from array to the set.

```js
set.remove(val, ...)
set.delete(val)
```

Remove one or more elements from the set.

```js
set.contains(val)
set.has(val)
```

Check if the set contains `val`.

```js
set.size()
```

Returns the size of the set.

```js
set.toArray()
set['*values']()
```

Returns the elements of the set as an Array.

```js
set.toString()
```

Serialize the set.

## License

Copyright © 2012 Paul Vorbach

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the “Software”), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
