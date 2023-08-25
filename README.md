# EXQS

Learning to create a compiler using C.
There is an example of code that can be compiled in example file.
We are basically trying to convert the code written in exqs to C, which would then be compiled to the Machine code using C compilers. 

## Usage
Run the executable from a shell with a path to some source code as the only argument. Currently, we print out the furthest progess we are able to make. Eventually the output will be the compiled source code.

## Building
NOTE: Shell commands shown assusme a working directory of this repository.

Dependencies:
- CMake >= 3.14
- Any C Compiler

First, generate a build tree using CMake.
```shell
    cmake -B bld
```
OR
```shell
    cmake -G Ninja -B bld -DCMAKE_BUILD_TYPE=Release
```
Finally, build an executable from the build tree.
```shell
    cmake --build bld
```