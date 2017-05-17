# example-cmake-helloworld-cpp

This is an example of how to use CMake to build a Hello World C++ program.

## Getting and Running this Example

To get and run this example on Mac or Ubuntu

```bash
git clone https://github.com/ibrahimelfar/example-cmake-helloworld-cpp.git
cmake . && make && ./hello
```

## Elements

After making sure [cmake is installed](https://cmake.org/install/), there are three pieces to this example.

First, there is the hello world C++ file.

```cpp
#include<iostream>

int main(int argc, char *argv[]){
   std::cout << "hello" << std::endl;
   return 0;
}
```

Second, there is the CMakeLists.txt which tells cmake how to build this simple project.

```
cmake_minimum_required(VERSION 3.6.2)

project (hello)
add_executable(hello hello.cpp)
```

Third, simply run cmake, followed by make, and then the hello world executable itself.

```bash
cmake . && make && ./hello
```
