<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Seconds in a Minute

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> Number of seconds in a minute.

<section class="installation">

## Installation

```bash
npm install @stdlib/constants-time-seconds-in-minute
```

</section>

<section class="usage">

## Usage

```javascript
var SECONDS_IN_MINUTE = require( '@stdlib/constants-time-seconds-in-minute' );
```

#### SECONDS_IN_MINUTE

Number of seconds in a minute.

```javascript
var bool = ( SECONDS_IN_MINUTE === 60 );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The value is a generalization and does **not** take into account inaccuracies arising due to complications with time and dates. 

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var randu = require( '@stdlib/random-base-randu' );
var roundn = require( '@stdlib/math-base-special-roundn' );
var SECONDS_IN_MINUTE = require( '@stdlib/constants-time-seconds-in-minute' );

var secs;
var mins;
var i;

function mins2secs( mins ) {
    return mins * SECONDS_IN_MINUTE;
}

for ( i = 0; i < 10; i++ ) {
    mins = roundn( randu()*20.0, -2 );
    secs = mins2secs( mins );
    console.log( '%d minutes => %d seconds', mins, secs );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-time-seconds-in-minute.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-time-seconds-in-minute

[test-image]: https://github.com/stdlib-js/constants-time-seconds-in-minute/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/constants-time-seconds-in-minute/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-time-seconds-in-minute/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-time-seconds-in-minute?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-time-seconds-in-minute
[dependencies-url]: https://david-dm.org/stdlib-js/constants-time-seconds-in-minute/main

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-time-seconds-in-minute/main/LICENSE

</section>

<!-- /.links -->
