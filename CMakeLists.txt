cmake_minimum_required(VERSION 3.0)
project(c_opcua_test C)

add_executable(${PROJECT_NAME} src/main.c)

add_subdirectory(libs/open62541)

target_link_libraries(${PROJECT_NAME} open62541)