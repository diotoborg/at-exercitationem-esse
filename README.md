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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# ndarray

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Multidimensional arrays.

<section class="installation">

## Installation

```bash
npm install @diotoborg/at-exercitationem-esse
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@diotoborg/at-exercitationem-esse' );
```

#### ns

ndarray namespace.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following functions to create multidimensional arrays:

<!-- <toc pattern="+(array|ctor)"> -->

<div class="namespace-toc">

-   <span class="signature">[`array( [buffer,] [options] )`][@diotoborg/at-exercitationem-esse/array]</span><span class="delimiter">: </span><span class="description">create a multidimensional array.</span>
-   <span class="signature">[`ndarray( dtype, buffer, shape, strides, offset, order[, options] )`][@diotoborg/at-exercitationem-esse/ctor]</span><span class="delimiter">: </span><span class="description">multidimensional array constructor.</span>

</div>

<!-- </toc> -->

The namespace contains the following sub-namespaces:

<!-- <toc pattern="+(base|iter)"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@diotoborg/at-exercitationem-esse/base]</span><span class="delimiter">: </span><span class="description">base ndarray.</span>
-   <span class="signature">[`iter`][@diotoborg/at-exercitationem-esse/iter]</span><span class="delimiter">: </span><span class="description">multidimensional array iterators.</span>

</div>

<!-- </toc> -->

In addition, the namespace contains the following multidimensional array utility functions:

<!-- <toc pattern="*" > -->

<div class="namespace-toc">

-   <span class="signature">[`at( x[, ...indices] )`][@diotoborg/at-exercitationem-esse/at]</span><span class="delimiter">: </span><span class="description">return an `ndarray` element.</span>
-   <span class="signature">[`broadcastArray( x, shape )`][@diotoborg/at-exercitationem-esse/broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape.</span>
-   <span class="signature">[`broadcastArrays( ...arrays )`][@diotoborg/at-exercitationem-esse/broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`castingModes()`][@diotoborg/at-exercitationem-esse/casting-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray casting modes.</span>
-   <span class="signature">[`dataBuffer( x )`][@diotoborg/at-exercitationem-esse/data-buffer]</span><span class="delimiter">: </span><span class="description">return the underlying data buffer of a provided ndarray.</span>
-   <span class="signature">[`defaults()`][@diotoborg/at-exercitationem-esse/defaults]</span><span class="delimiter">: </span><span class="description">default ndarray settings.</span>
-   <span class="signature">[`dispatch( fcns, types, data, nargs, nin, nout )`][@diotoborg/at-exercitationem-esse/dispatch]</span><span class="delimiter">: </span><span class="description">create an ndarray function interface which performs multiple dispatch.</span>
-   <span class="signature">[`dtype( x )`][@diotoborg/at-exercitationem-esse/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of a provided ndarray.</span>
-   <span class="signature">[`dtypes( [kind] )`][@diotoborg/at-exercitationem-esse/dtypes]</span><span class="delimiter">: </span><span class="description">list of ndarray data types.</span>
-   <span class="signature">[`emptyLike( x[, options] )`][@diotoborg/at-exercitationem-esse/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`empty( shape[, options] )`][@diotoborg/at-exercitationem-esse/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having a specified shape and data type.</span>
-   <span class="signature">[`FancyArray( dtype, buffer, shape, strides, offset, order[, options] )`][@diotoborg/at-exercitationem-esse/fancy]</span><span class="delimiter">: </span><span class="description">fancy multidimensional array constructor.</span>
-   <span class="signature">[`flag( x, name )`][@diotoborg/at-exercitationem-esse/flag]</span><span class="delimiter">: </span><span class="description">return a specified flag for a provided ndarray.</span>
-   <span class="signature">[`flags( x )`][@diotoborg/at-exercitationem-esse/flags]</span><span class="delimiter">: </span><span class="description">return the flags of a provided ndarray.</span>
-   <span class="signature">[`scalar2ndarray( value[, options] )`][@diotoborg/at-exercitationem-esse/from-scalar]</span><span class="delimiter">: </span><span class="description">convert a scalar value to a zero-dimensional ndarray.</span>
-   <span class="signature">[`ind2sub( shape, idx[, options] )`][@diotoborg/at-exercitationem-esse/ind2sub]</span><span class="delimiter">: </span><span class="description">convert a linear index to an array of subscripts.</span>
-   <span class="signature">[`indexModes()`][@diotoborg/at-exercitationem-esse/index-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray index modes.</span>
-   <span class="signature">[`maybeBroadcastArray( x, shape )`][@diotoborg/at-exercitationem-esse/maybe-broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape if and only if the specified shape differs from the provided ndarray's shape.</span>
-   <span class="signature">[`maybeBroadcastArrays( arrays )`][@diotoborg/at-exercitationem-esse/maybe-broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`minDataType( value )`][@diotoborg/at-exercitationem-esse/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum ndarray data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@diotoborg/at-exercitationem-esse/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`ndims( x )`][@diotoborg/at-exercitationem-esse/ndims]</span><span class="delimiter">: </span><span class="description">return the number of ndarray dimensions.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@diotoborg/at-exercitationem-esse/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger ndarray data type of the same kind.</span>
-   <span class="signature">[`numelDimension( x, dim )`][@diotoborg/at-exercitationem-esse/numel-dimension]</span><span class="delimiter">: </span><span class="description">return the size (i.e., number of elements) of a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`numel( x )`][@diotoborg/at-exercitationem-esse/numel]</span><span class="delimiter">: </span><span class="description">return the number of elements in an ndarray.</span>
-   <span class="signature">[`offset( x )`][@diotoborg/at-exercitationem-esse/offset]</span><span class="delimiter">: </span><span class="description">return the index offset specifying the underlying buffer index of the first iterated ndarray element.</span>
-   <span class="signature">[`order( x )`][@diotoborg/at-exercitationem-esse/order]</span><span class="delimiter">: </span><span class="description">return the layout order of a provided ndarray.</span>
-   <span class="signature">[`orders()`][@diotoborg/at-exercitationem-esse/orders]</span><span class="delimiter">: </span><span class="description">list of ndarray orders.</span>
-   <span class="signature">[`outputDataTypePolicies()`][@diotoborg/at-exercitationem-esse/output-dtype-policies]</span><span class="delimiter">: </span><span class="description">list of output ndarray data type policies.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@diotoborg/at-exercitationem-esse/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the ndarray data type with the smallest size and closest "kind" to which ndarray data types can be **safely** cast.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@diotoborg/at-exercitationem-esse/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@diotoborg/at-exercitationem-esse/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( x )`][@diotoborg/at-exercitationem-esse/shape]</span><span class="delimiter">: </span><span class="description">return the shape of a provided ndarray.</span>
-   <span class="signature">[`sliceAssign( x, y, ...s[, options] )`][@diotoborg/at-exercitationem-esse/slice-assign]</span><span class="delimiter">: </span><span class="description">assign element values from a broadcasted input `ndarray` to corresponding elements in an output `ndarray` view.</span>
-   <span class="signature">[`sliceDimensionFrom( x, dim, start[, options] )`][@diotoborg/at-exercitationem-esse/slice-dimension-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimensionTo( x, dim, stop[, options] )`][@diotoborg/at-exercitationem-esse/slice-dimension-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimension( x, dim, slice[, options] )`][@diotoborg/at-exercitationem-esse/slice-dimension]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray` when sliced along a specified dimension.</span>
-   <span class="signature">[`sliceFrom( x, ...start[, options] )`][@diotoborg/at-exercitationem-esse/slice-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input ndarray.</span>
-   <span class="signature">[`sliceTo( x, ...stop[, options] )`][@diotoborg/at-exercitationem-esse/slice-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input ndarray.</span>
-   <span class="signature">[`slice( x, ...s[, options] )`][@diotoborg/at-exercitationem-esse/slice]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray`.</span>
-   <span class="signature">[`stride( x, dim )`][@diotoborg/at-exercitationem-esse/stride]</span><span class="delimiter">: </span><span class="description">return the stride along a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`strides( x )`][@diotoborg/at-exercitationem-esse/strides]</span><span class="delimiter">: </span><span class="description">return the strides of a provided ndarray.</span>
-   <span class="signature">[`sub2ind( shape, ...subscripts[, options] )`][@diotoborg/at-exercitationem-esse/sub2ind]</span><span class="delimiter">: </span><span class="description">convert subscripts to a linear index.</span>
-   <span class="signature">[`ndarray2array( x )`][@diotoborg/at-exercitationem-esse/to-array]</span><span class="delimiter">: </span><span class="description">convert an ndarray to a generic array.</span>
-   <span class="signature">[`zerosLike( x[, options] )`][@diotoborg/at-exercitationem-esse/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`zeros( shape[, options] )`][@diotoborg/at-exercitationem-esse/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having a specified shape and data type.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var ns = require( '@diotoborg/at-exercitationem-esse' );

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@diotoborg/at-exercitationem-esse.svg
[npm-url]: https://npmjs.org/package/@diotoborg/at-exercitationem-esse

[test-image]: https://github.com/diotoborg/at-exercitationem-esse/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/diotoborg/at-exercitationem-esse/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/diotoborg/at-exercitationem-esse/main.svg
[coverage-url]: https://codecov.io/github/diotoborg/at-exercitationem-esse?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/diotoborg/at-exercitationem-esse.svg
[dependencies-url]: https://david-dm.org/diotoborg/at-exercitationem-esse/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/diotoborg/at-exercitationem-esse/tree/deno
[deno-readme]: https://github.com/diotoborg/at-exercitationem-esse/blob/deno/README.md
[umd-url]: https://github.com/diotoborg/at-exercitationem-esse/tree/umd
[umd-readme]: https://github.com/diotoborg/at-exercitationem-esse/blob/umd/README.md
[esm-url]: https://github.com/diotoborg/at-exercitationem-esse/tree/esm
[esm-readme]: https://github.com/diotoborg/at-exercitationem-esse/blob/esm/README.md
[branches-url]: https://github.com/diotoborg/at-exercitationem-esse/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/diotoborg/at-exercitationem-esse/main/LICENSE

<!-- <toc-links> -->

[@diotoborg/at-exercitationem-esse/at]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/at

[@diotoborg/at-exercitationem-esse/broadcast-array]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/broadcast-array

[@diotoborg/at-exercitationem-esse/broadcast-arrays]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/broadcast-arrays

[@diotoborg/at-exercitationem-esse/casting-modes]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/casting-modes

[@diotoborg/at-exercitationem-esse/data-buffer]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/data-buffer

[@diotoborg/at-exercitationem-esse/defaults]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/defaults

[@diotoborg/at-exercitationem-esse/dispatch]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/dispatch

[@diotoborg/at-exercitationem-esse/dtype]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/dtype

[@diotoborg/at-exercitationem-esse/dtypes]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/dtypes

[@diotoborg/at-exercitationem-esse/empty-like]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/empty-like

[@diotoborg/at-exercitationem-esse/empty]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/empty

[@diotoborg/at-exercitationem-esse/fancy]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/fancy

[@diotoborg/at-exercitationem-esse/flag]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/flag

[@diotoborg/at-exercitationem-esse/flags]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/flags

[@diotoborg/at-exercitationem-esse/from-scalar]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/from-scalar

[@diotoborg/at-exercitationem-esse/ind2sub]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/ind2sub

[@diotoborg/at-exercitationem-esse/index-modes]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/index-modes

[@diotoborg/at-exercitationem-esse/maybe-broadcast-array]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/maybe-broadcast-array

[@diotoborg/at-exercitationem-esse/maybe-broadcast-arrays]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/maybe-broadcast-arrays

[@diotoborg/at-exercitationem-esse/min-dtype]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/min-dtype

[@diotoborg/at-exercitationem-esse/mostly-safe-casts]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/mostly-safe-casts

[@diotoborg/at-exercitationem-esse/ndims]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/ndims

[@diotoborg/at-exercitationem-esse/next-dtype]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/next-dtype

[@diotoborg/at-exercitationem-esse/numel-dimension]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/numel-dimension

[@diotoborg/at-exercitationem-esse/numel]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/numel

[@diotoborg/at-exercitationem-esse/offset]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/offset

[@diotoborg/at-exercitationem-esse/order]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/order

[@diotoborg/at-exercitationem-esse/orders]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/orders

[@diotoborg/at-exercitationem-esse/output-dtype-policies]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/output-dtype-policies

[@diotoborg/at-exercitationem-esse/promotion-rules]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/promotion-rules

[@diotoborg/at-exercitationem-esse/safe-casts]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/safe-casts

[@diotoborg/at-exercitationem-esse/same-kind-casts]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/same-kind-casts

[@diotoborg/at-exercitationem-esse/shape]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/shape

[@diotoborg/at-exercitationem-esse/slice-assign]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-assign

[@diotoborg/at-exercitationem-esse/slice-dimension-from]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-dimension-from

[@diotoborg/at-exercitationem-esse/slice-dimension-to]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-dimension-to

[@diotoborg/at-exercitationem-esse/slice-dimension]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-dimension

[@diotoborg/at-exercitationem-esse/slice-from]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-from

[@diotoborg/at-exercitationem-esse/slice-to]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice-to

[@diotoborg/at-exercitationem-esse/slice]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/slice

[@diotoborg/at-exercitationem-esse/stride]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/stride

[@diotoborg/at-exercitationem-esse/strides]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/strides

[@diotoborg/at-exercitationem-esse/sub2ind]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/sub2ind

[@diotoborg/at-exercitationem-esse/to-array]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/to-array

[@diotoborg/at-exercitationem-esse/zeros-like]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/zeros-like

[@diotoborg/at-exercitationem-esse/zeros]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/zeros

[@diotoborg/at-exercitationem-esse/base]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/base

[@diotoborg/at-exercitationem-esse/iter]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/iter

[@diotoborg/at-exercitationem-esse/array]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/array

[@diotoborg/at-exercitationem-esse/ctor]: https://github.com/diotoborg/at-exercitationem-esse/tree/main/ctor

<!-- </toc-links> -->

</section>

<!-- /.links -->
