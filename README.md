Fork of https://github.com/swagger-api/swagger-ui

This to make a proper package to have the Ultimaker 3 serve it's own API documentation.
The actual documentation file is supplied by the opinicus package.

This is just the support package to properly format and display the documentation.


=Modifications
* Cleaned out everything except the "dist" folder that we need.
* Modified dist/index.html to match our needs.
* Created CMake files to build a package

Building the package:

```
rm -rf build/ dir (if it already exists)
mkdir build
cmake -DRELEASE_VERSION="x.y.z" ..
cpack
```
If the `-DRELEASE_VERSION` value is not passed via the command line then a default of `1.0.0` is used instead.
