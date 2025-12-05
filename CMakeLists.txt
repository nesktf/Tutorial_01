# Template / barebone settings :3
cmake_minimum_required(VERSION 3.23)
project(Tutorial_01)

# Adds subdirectories.
# Adds an executable target called "OpenGL_Window_Tutorial" to the project.
add_subdirectory(src)
add_subdirectory(external)
add_subdirectory(external/glew/include)
add_subdirectory(external/glfw3/include)
