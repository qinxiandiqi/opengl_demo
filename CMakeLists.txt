cmake_minimum_required(VERSION 3.0.0)
project(OpenGL_Demo VERSION 0.1.0)

add_subdirectory(src bin)
add_subdirectory(glfw glfw/bin)
add_subdirectory("glew/build/cmake" glew/bin)

include(CTest)
enable_testing()

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
