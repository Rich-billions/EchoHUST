cmake_minimum_required(VERSION 3.10)
project(HTTPSERVER)

set(CMAKE_CXX_STANDARD 17)

add_executable(HTTPSERVER main.cpp mysocket.h http.cpp epoll.h mysql.h)

target_link_libraries(HTTPSERVER libjsoncpp.a)
target_link_libraries(HTTPSERVER libmysqlclient.so)
