add_library(B STATIC classB.h classB.cpp)
target_include_directories(B PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})