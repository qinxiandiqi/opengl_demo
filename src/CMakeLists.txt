aux_source_directory(. DIR_SRCS)

include_directories(glfw/include)
include_directories(glew/include)

add_executable(OpenGL_Demo ${DIR_SRCS})

target_link_libraries(OpenGL_Demo glfw)
target_link_libraries(OpenGL_Demo glew)