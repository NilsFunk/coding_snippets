subprojectA/CMakeLists.txt:

project(SubProjectA)
add_library(subprojectA STATIC src/libraryA.cpp)
# PUBLIC adds both:
#     1) include directories for compile library and
#     2) include directories for library's interface
target_include_directories(subprojectA PUBLIC include)