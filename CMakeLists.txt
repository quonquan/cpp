cmake_minimum_required(VERSION 3.10)
project(cpp)

add_executable(app app.cpp)
target_link_libraries(app ${Boost_LIBRARIES})
target_link_libraries(app ${CMAKE_THREAD_LIBS_INIT})

include_directories("${CMAKE_SOURCE_DIR}/include")

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -std=c++1y -pedantic -Wextra")
