cmake_minimum_required(VERSION 2.8.12)
project(B)

include_directories(../a/)
include_directories(../a_src/)
file(GLOB SOURCES_0 ../a_src/*.cpp)

file(GLOB SOURCES "*.cpp")
#add_library(elm_lib ${ELMLIB})
add_executable(test_chong ${SOURCES_0} ${SOURCES} )
#target_link_libraries(BaseHWDecoder elm_lib)
