# CMakeList.txt : CMake project for ModernOpenGLUdemy, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Required packages
find_package(glew REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

# Add source to this project's executable.
add_executable (ModernOpenGLUdemy "main.cpp")

target_link_libraries(ModernOpenGLUdemy PRIVATE GLEW::GLEW glfw)

# TODO: Add tests and install targets if needed.
