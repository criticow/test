cmake_minimum_required(VERSION 3.20)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_TOOLCHAIN_FILE "$ENV{VCPKG_ROOT}/scripts/buildsystems/vcpkg.cmake")
set(ROOT_DIR ${CMAKE_CURRENT_LIST_DIR})

project(ctc CXX)

add_subdirectory(src)
add_subdirectory(tests)