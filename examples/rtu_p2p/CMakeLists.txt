cmake_minimum_required(VERSION 3.0)

project(p2p)

add_executable(p2p_master p2p_master.c)
add_executable(p2p_slave p2p_slave.c)

target_link_libraries(p2p_master PRIVATE Threads::Threads)
target_link_libraries(p2p_slave PRIVATE Threads::Threads)
