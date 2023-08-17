# doxygen-sphinx-breath-cmake

CMake project documentation with Doxygen, Sphinx and Breathe.
This repo is based on the following tutorial:
https://devblogs.microsoft.com/cppblog/clear-functional-c-documentation-with-sphinx-breathe-doxygen-cmake/

## Install dependencies

Install [conda](https://docs.conda.io/en/latest/miniconda.html) to manage dependencies first.
Then create a conda environment and then do the following:
```sh
conda create -n doxygen-sphinx-breathe-cmake python=3.10
conda activate doxygen-sphinx-breathe-cmake
pip install sphinx sphinx_rtd_theme breathe
conda install -c conda-forge doxygen cmake
```

## Build the project with documentation

```sh
mkdir build; cd build; cmake -DCMAKE_INSTALL_PREFIX=../install ..; make install; cd -
```

## Open installed documentation

```sh
open install/share/doc/cc/sphinx/index.html
```
