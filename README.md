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

# ENV

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Object containing the user environment.



<section class="usage">

## Usage

To use in Observable,

```javascript
ENV = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/process-env@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var ENV = require( 'path/to/vendor/umd/process-env/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/process-env@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.ENV;
})();
</script>
```

#### ENV

`Object` containing the user environment.

```javascript
var user = ENV.USER;
// returns <string>
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   See [environ(7)][man-environ].
-   Modifications to `ENV` are local to the process in which `ENV` is modified.
-   On Windows systems, environment variables are case insensitive.
-   In browser environments, `ENV` is an **empty** object.
-   Be careful when modifying environment variables as the environment variable object represents shared state. Accordingly, modifications affect all environment variable consumers. 

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/process-env@umd/browser.js"></script>
<script type="text/javascript">
(function () {

console.dir( ENV );

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/process/argv`][@stdlib/process/argv]</span><span class="delimiter">: </span><span class="description">array containing command-line arguments passed when launching the calling process.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/process-env.svg
[npm-url]: https://npmjs.org/package/@stdlib/process-env

[test-image]: https://github.com/stdlib-js/process-env/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/process-env/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/process-env/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/process-env?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/process-env.svg
[dependencies-url]: https://david-dm.org/stdlib-js/process-env/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/process-env/tree/deno
[umd-url]: https://github.com/stdlib-js/process-env/tree/umd
[esm-url]: https://github.com/stdlib-js/process-env/tree/esm
[branches-url]: https://github.com/stdlib-js/process-env/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/process-env/main/LICENSE

[man-environ]: http://man7.org/linux/man-pages/man7/environ.7.html

<!-- <related-links> -->

[@stdlib/process/argv]: https://github.com/stdlib-js/process-argv/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
