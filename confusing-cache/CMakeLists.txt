cmake_minimum_required(VERSION 2.8)
project(foo NONE)

function(set_a_globally)
    message("Variable a [before] set globally: a = '${a}'")
    set(a "789" CACHE STRING "")
    message("Variable a [after] set globally: a = '${a}'")
endfunction()

set(a "123")

set_a_globally()

message("[TOP LEVEL] a = '${a}'")
