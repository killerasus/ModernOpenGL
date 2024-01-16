# Building

## Dependencies

This code depends on the following libraries that can be easily installed with `vcpkg` or with your distribution package manager:

1. GLEW
1. GLFW (glfw3)
1. OpenGL

Dependencies are already configured in [`CMakeLists.txt`](ModernOpenGLUdemy/CMakeLists.txt).

## Windows

In Windows the process is very simple using [vcpkg](https://github.com/microsoft/vcpkg) and [Visual Studio 2019](https://visualstudio.microsoft.com/) with [CMake](https://cmake.org/) support. Follow `vcpkg` instructions on how to configure and install libraries. Don't forget to integrate vcpkg with `.\vcpkg integrate install`.

After cloning the repository, open the project directory in Visual Studio. The CMakeLists parsing should start immediately.
