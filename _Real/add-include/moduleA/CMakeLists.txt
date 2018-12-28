add_library(A STATIC classA.h classA.cpp)
target_include_directories(A PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})