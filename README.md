# @ember/string

This Ember addon contains utility functions to deal with `String`s.

## Installation

* `ember install @ember/string`

## Usage

The following exports are available:

```javascript
import {
  camelize,
  capitalize,
  classify,
  dasherize,
  decamelize,
  underscore,
  w,
  fmt,
  loc
} from '@ember/string';
```

### `camelize`, `capitalize`, `classify`, `dasherize`, `decamelize`, `underscore`

These methods transform a string, for example:

```javascript
import { camelize } from '@ember/string';

camelize("my class") // MyClass
```

Consult the tests of the respective function to see the behaviour in more detail.

### `w`

This utility function takes a string, splits it on spaces, and returns an array with the elements.

```javascript
import { w } from '@ember/string';

w("my array of   strings") // ["my", "array", "of", "strings"]
```

### `fmt`, `loc`

These methods are deprecated and only included to ease the transition from the `Ember.String` namespace.
See [DEPRECATIONS.md](DEPRECATIONS.md) for more details on how to resolve the deprecations.
