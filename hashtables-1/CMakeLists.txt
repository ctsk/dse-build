add_library(hashtables hashtables.cpp)

add_executable(perf.out perf.cpp)
target_link_libraries(perf.out hashtables)
target_include_directories(perf.out PRIVATE .)

add_executable(test.out test.cpp)
target_link_libraries(test.out hashtables)
target_include_directories(test.out PRIVATE .)
