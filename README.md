# Meson build for CImg

URL: 

- [github repo](https://github.com/dtschump/CImg);

The subfolder "src" is a clone of git repository of a specified release version. 
unit-tests are not built as part of the meson-build.

## Versions

The "revision" of cimg.wrap and the version of this meson-build project matches the embedded submodule GSL version as following:

Meson-Build |  CPP-HTTPLIB 
------------|-----------
v1.0         | v.3.1.2


## Usage

copy cimg.wrap to "subprojects" sub-folder of your main project directory.


in meson.build:

```
# import

cimg_dep = dependency('cimg')

# use
srcs = ['main.c', ...]

executable('test', srcs, dependencies: [cimg_dep, ...])

```

in main.c:

```c
#include <cimg>

void foo(){
}
```



