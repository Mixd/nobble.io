# Groot
The root of all projects.

Groot is a class-based CSS Grid system derived from the amazing work Nicolas Gallagher produced with [Griddle](https://github.com/necolas/griddle). I've been using Griddle for many years professionally now and whilst I love the overall package, its not perfect and could do with a upgrade. I've started Groot with the intention of being that.

Groot prides itself on the following:

- Flexibility: Complete control to fit it into your own workflow or framework.
- Modular: Defaults to a BEM structured Grid System and keeps the [Single Responsibility Principle](https://en.wikipedia.org/wiki/Single_responsibility_principle) in mind at all times.
- Configurable: Ability to change any class names, gutter sizes or alignment declarations to your hearts desire.
- Lightweight: With its opt-in columns, you're looking at around 5kb minified and gzipped, with only the classes you're using in your project; rather than some you'll never use.

## Installation

Groot is available through a number of package managers, including:

```sh
npm install --save-dev groot
bower install --save groot
gem install --save groot
```

Alternatively, you could always download/clone this repo and use it in your own way.

## Usage

If you've used [Griddle](https://github.com/necolas/griddle) before, you'll see that the syntax is very similar. If you've not used it before, don't fear. Groot is pretty easy to get to grips with.

Once you've imported to the Groot system, use the `groot` mixin provided to build out the grids you need.

```scss
@import "groot";
@include groot($columns, $extension);
```

It takes two parameters:

- `$columns`: A space-separated list of integers, each of which results in the build of that particular grid.
- `$suffix`: The suffix for the class. This is optional and is intended when you're setting up a Groot instance within a Media Query.


## Configuration
While Groot may have defaults for the configuration, you still have a lot of freedom in how you'd like to setup your version.

Each of the following variables should be declared **above** the import of Groot.

**For example:**

```scss
// Alter Config here
@import "groot";
// Include mixin here
```

**Available options and defaults:**

```scss
// Namespace Options
$gr-grid: "grid";             // The Grid's class namespace.
$gr-item: "grid__item";       // Grid Item's class namespace.
$gr-unit: "grid__item";       // Grid Unit's class namespace.

// Sizing
$gr-gutter: 1em;              // The space between each Grid Item.

// Grid alignment
$gr-grid-direction: inherit;  // Controls the *direction* CSS property for the Grid.
$gr-grid-align-x: inherit;    // Controls the *text-align* property for the Grid.

// Item alignment
$gr-item-direction: inherit;  // Controls the *direction* CSS property for the Grid Item.
$gr-item-align-x: inherit;    // Controls the *text-align* property for the Grid Item.
$gr-item-align-y: top;        // Controls the *vertical-align* property for the Grid Item.
```

## Modifiers


## Examples


## Credits

Groot has been produced primarily by Luke Whitehouse, however, special thanks have to be given to the following:
- [Mixd](http://mixd.co.uk): Who introduced me to Griddle in the first place and without which I probably wouldn't be where I am today. If – like us – you work with WordPress then you may be interested in our Open Source project called [wp-deploy](https://github.com/Mixd/wp-deploy); a capistrano-powered deployment tool for WordPress.

## License

MIT License (MIT)

Copyright (c) 2015 Luke Whitehouse, https://github.com/lukewhitehouse/groot

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
