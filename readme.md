# line-read [![Build Status](https://travis-ci.org/minhhh/line-read.svg?branch=master)](https://travis-ci.org/minhhh/line-read)

Read line by line from a stream, file or stdin lazily.


## Install

```
$ npm install --save line-read
```


## Usage

```js
    var readline = require('line-read');
    readline.readLineFromFile('filename', '\n').join(function(xs) {
        // xs is the list of lines from the file
    });
```


## API

All methods return a `lazy` instance of lines. See the [lazy](https://github.com/pkrumins/node-lazy) package for more details.

### readLine(stream, separator)

Get lines from stream. Lines are separated by separator, default to `\n`.

### readLineFromFile(filename, separator)

Get lines from file `filename`. Lines are separated by separator, default to `\n`.


## License

MIT © [Minh Ha](http://minhhh.github.io)
