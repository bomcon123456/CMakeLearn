cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(10 a b c)
set(11 a;b;c)
set(12 "a b" "c")
set(13 "a;b;c")
set(14 a "b;c")

message("10 = 'a' + 'b' + 'c' = '${10}'")
message("11 = 'a;b;c' = '${11}'")
message("12 = 'a b' + 'c' = '${12}'")
message("13 = \"'a;b;c '\" = '${13}'")
message("14 = 'a' + 'b;c' = '${14}'")

message("print message: " ${13})
message("print message: " "a" "b" "c")
