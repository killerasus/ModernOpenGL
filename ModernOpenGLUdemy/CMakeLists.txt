# CMakeList.txt : CMake project for ModernOpenGLUdemy, include source and define
# project specific logic here.
#
cmake_minimum_required(VERSION 3.21)

# Required packages
find_package(GLEW REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
find_package(OpenGL REQUIRED)

# Add source to this project's executable.
add_executable(ModernOpenGLUdemy)

target_sources(ModernOpenGLUdemy
    PRIVATE
      main.cpp
)

set_target_properties(ModernOpenGLUdemy
    PROPERTIES
      CXX_STANDARD 17
      CXX_STANDARD_REQUIRED ON
)

target_link_libraries(ModernOpenGLUdemy PRIVATE GLEW::GLEW glfw OpenGL::GL)

# TODO: Add tests and install targets if needed.
