cmake_minimum_required(VERSION 4.0)
project(wifi_backend_plugin)
find_package(clixon REQUIRED)
find_package(cligen REQUIRED)
add_library(wifi_backend_plugin SHARED wifi_backend_plugin.c)
target_link_libraries(wifi_backend_plugin clixon::clixon cligen::cligen)

