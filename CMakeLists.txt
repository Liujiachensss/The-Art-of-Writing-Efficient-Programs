cmake_minimum_required(VERSION 3.16.0)
project(test VERSION 0.1.0)

include_directories(${CMAKE_HOME_DIRECTORY}/helper)

# include(CTest)
# enable_testing()

# set(LIB_HOME )
if(NOT CMAKE_C_COMPILER)
    set(CMAKE_C_COMPILER /root/miniconda3/envs/opc/bin/gcc)
endif()
if(NOT CMAKE_CXX_COMPILER)
    set(CMAKE_CXX_COMPILER /root/miniconda3/envs/opc/bin/g++)
endif()

# set(CPACK_PROJECT_NAME ${PROJECT_NAME})
# set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
# include(CPack)
# set(CMAKE_MAKE_PROGRAM /home/usr/anaconda3/envs/opc/bin/ninja)
# set(CMAKE_MAKE_PROGRAM ~/.conda/envs/torchenv/bin/ninja)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/test_bin)
# generate compile_commands.json
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# if(__INTEL_COMPILER)
# message(STATUS "Using Intel compiler")
# else()
# message(STATUS "Not Using Intel compiler")
# endif()

if (CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
message(STATUS "Using GCC compiler")
elseif (CMAKE_CXX_COMPILER_ID STREQUAL "Clang")
message(STATUS "Using Clang compiler")
elseif (CMAKE_CXX_COMPILER_ID STREQUAL "IntelLLVM")
message(STATUS "Using Intel compiler")
elseif (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
message(STATUS "Using MSVC compiler")
else()
message(STATUS "${CMAKE_CXX_COMPILER_ID}")
endif()

find_library(Benchmark_LIB benchmark PATHS /home/usr/software/benchmark/lib REQUIRED)
set(Benchmark_INCLUDE_DIR /home/usr/software/benchmark/include)

include_directories(${Benchmark_INCLUDE_DIR})

add_subdirectory(Chapter02)
