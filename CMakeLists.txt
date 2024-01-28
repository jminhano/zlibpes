cmake_minimum_required (VERSION 3.27.2)
project(zlibpes VERSION 0.5.0)

# c++ 20 is required
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# third party libraries
find_package(ZLIB REQUIRED)

# add zlibes list
add_subdirectory(src)