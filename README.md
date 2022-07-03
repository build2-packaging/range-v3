# range-v3

This is the `build2` package of `range-v3` project:

 - `range-v3` : https://github.com/ericniebler/range-v3/
 - `build2`: https://build2.org

## NOTE: CI builds failing with Clang

`build2`'s CI will build with `cxx.std = latest` which will lead to recent clang and gcc builds to use `-std=c++2b` and `-std=c++23` respectively.
In the case of clang it will lead to compilation failures. However, **C++23 is not supported yet by `range-v3`** which means that these errors should be ignored.
**You can use this package with clang-13 and higher (and emcc) without build failures with `cxx.std = 20`.**

