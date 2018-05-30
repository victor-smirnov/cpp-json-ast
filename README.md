Facebook Clang Plugins
======================

This [repository](https://github.com/facebook/facebook-clang-plugins) aims to share some useful clang plugins developed at Facebook.

It contains two kinds of plugins to the [clang compiler](http://clang.llvm.org/):

- frontend plugins process the syntax of source files directly to accomplish more general tasks; specifically, we have developed a clang-to-ocaml bridge to make code analyses easier.

Most of the plugins here have been written with iOS in mind. However, different platforms may be considered in the future.

Structure of the repository
---------------------------

- [`libtooling`](https://github.com/facebook/facebook-clang-plugins/tree/master/libtooling) : frontend plugins (currently a clang-to-json AST exporter),

Quick start
-----------

General instructions to compile clang can be found here: http://clang.llvm.org/get_started.html

Mac users may create an Xcode project as follows:
```
export CLANG_PREFIX=/usr/local #should be the same as above
make xcode
```

Additional configuration options are available in `Makefile.config` (and possibly `CMakeLists.txt`).
