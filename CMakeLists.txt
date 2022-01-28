cmake_minimum_required(VERSION "3.21")

project("HelloWorld")

add_executable("${PROJECT_NAME}" main.cpp  day1.cpp StringHelper.cpp FileLoader.cpp day1-gtests.cpp)

install(TARGETS "${PROJECT_NAME}" DESTINATION bin)
install(FILES "main.cpp" DESTINATION src)
