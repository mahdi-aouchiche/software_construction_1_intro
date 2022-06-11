cmake_minimum_required(VERSION 3.0.0)
project(CS100_Lab1 VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(hello_world 
    src/main1.cpp
)

add_executable(area_calculator 
    src/main2.cpp 
    src/rectangle.cpp
)

add_executable(standard_area_calculator 
    src/main3.cpp 
    src/rectangle.cpp
)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
