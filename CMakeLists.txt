# ========= #
# DSE TASKS #
# ========= #
cmake_minimum_required(VERSION 3.25)
project(dse-tasks)

# =============== #
# COMPILE OPTIONS #
# =============== #
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -Wall -Wconversion -Wextra -Wshadow -fsanitize=address,undefined")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -flto")

# ======= #
# HEADERS #
# ======= #
include_directories(include)

# ===== #
# TASKS #
# ===== #
add_subdirectory(debugging)
add_subdirectory(hashtables-1)