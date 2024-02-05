# Qt's cube example (modified)

Originally, this worked for Qt 5.9.3. I made some changes previously to work with
a newer version of OpenGL. Then, I changed it to compile under Qt 6 and cmake
instead of the .pro file.

Anyway, nothing special. Just something that works out of the box with Qt6/cmake.

## How to build:
1. Highly recommedned: make your build directory. change your directory to that.
2. run cmake and build:
   ```
   CMAKE_PREFIX_PATH=<path to your qt installation> cmake <path to this sources>
   cmake --build .
   ```
3. run the executable
   ```
   ./cubeApp
   ```
   
