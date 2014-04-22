*This repository is a mirror of the [component](http://component.io) module [bredele/mapify](http://github.com/bredele/mapify). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/bredele-mapify`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# mapify

  Turns any function into an array mapping

## Installation

  Install with [component(1)](http://component.io):

    $ component install bredele/mapify

## Usage

```js
var mapify = require('mapify');
var square = mapify(function(n){return n * n;});

square([1,2,3]);
// [1,4,9]

```

Mapify get nicer when use with [get](https://github.com/timoxley/get).

```js
var arr = [{
  name: 'olivier',
  age: '27'
},{
  name: 'amy'
  age: '26'
}];
mapify(get('name'))(arr);
// ['olivier', 'amy']

```

## License

  MIT
