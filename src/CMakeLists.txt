add_executable(OpenGL_Window_Tutorial)


# Adds the "Main.cpp" source file to the Tutorial target
target_sources(Tutorial_01
    PRIVATE
        "main.cpp"
)

# Adds the Window, GLEW and GLFW libraries as linked dependencies
# to the Tutorial_01 target

target_link_libraries(Tutorial_01
    PRIVATE
        Window
        glew
        glfw3
)


add_library(Window)
add_library(glew)
add_library(glfw3)


# TODO6: Add the source and header file located in Step1/MathFunctions to the
#        MathFunctions target, note that the intended way to include the
#        MathFunctions header is:
#          #include <MathFunctions.h>

target_sources(Tutorial_01
    PRIVATE
        Window.cpp

    PUBLIC
        FILE_SET HEADERS
        FILES
            Window.h
            glew.h
            glfw3.h
)
