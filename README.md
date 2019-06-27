#Docker image for Python Datascience containers
## SOFTWARE PACKAGES
   * musl: standard C library
   * lib6-compat: compatibility libraries for glibc
   * linux-headers: commonly needed, and an unusual package name from Alpine.
   * build-base: used so we include the basic development packages (gcc)
   * bash: so we can access /bin/bash
   * git: to ease up clones of repos
   * ca-certificates: for SSL verification during Pip and easy_install
   * freetype: library used to render text onto bitmaps, and provides support font-related operations
   * libgfortran: contains a Fortran shared library, needed to run Fortran
   * libgcc: contains shared code that would be inefficient to duplicate every time as well as auxiliary helper routines and runtime support
   * libstdc++: The GNU Standard C++ Library. This package contains an additional runtime library for C++ programs built with the GNU compiler
   * openblas: open source implementation of the BLAS(Basic Linear Algebra Subprograms) API with many hand-crafted optimizations for specific processor types
   * tcl: scripting language
   * tk: GUI toolkit for the Tcl scripting language
   * libssl1.0: SSL shared libraries

## PYTHON DATA SCIENCE PACKAGES
   * numpy: support for large, multi-dimensional arrays and matrices
   * matplotlib: plotting library for Python and its numerical mathematics extension NumPy.
   * scipy: library used for scientific computing and technical computing
   * scikit-learn: machine learning library integrates with NumPy and SciPy
   * pandas: library providing high-performance, easy-to-use data structures and data analysis tools
   * nltk: suite of libraries and programs for symbolic and statistical natural language processing for English


## Command
```
# For Python 2.7 pull
$ docker pull nguyenphuongthanhf/python-datascience:2.7
# For Python 3.6 pull
$ docker pull nguyenphuongthanhf/python-datascience:3.6
$ docker container run --rm -it nguyenphuongthanhf/python-datascience:3.6 python

docker container run --rm -it -v $(pwd):app nguyenphuongthanhf/python-datascience:latest python

docker container run -v $(pwd):/app --rm -it -u www nguyenphuongthanhf/python-datascience:latest sh

```
