cmake_minimum_required(VERSION "3.21")

project("HelloWorld")

add_executable("${PROJECT_NAME}" "main.cpp")
add_library( # Sets the name of the library.
        native-lib

        # Sets the library as a shared library.
        SHARED

        # Provides a relative path to your source file(s).
        day1.cpp StringHelper.cpp FileLoader.cpp day1-gtests.cpp)
)
install(TARGETS "${PROJECT_NAME}" DESTINATION bin)
install(FILES "main.cpp" DESTINATION src)
