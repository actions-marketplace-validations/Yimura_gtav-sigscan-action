cmake_minimum_required(VERSION 3.10)
include_directories(
    ${PROJECT_SOURCE_DIR}/src
    ${PROJECT_SOURCE_DIR}/vendor/AES/src
    ${PROJECT_SOURCE_DIR}/vendor/httprequest/include
    ${PROJECT_SOURCE_DIR}/vendor/rapidjson/include)
set(CMAKE_CXX_STANDARD 20)
add_executable(sigscan main.cpp ${PROJECT_SOURCE_DIR}/vendor/AES/src/AES.cpp)
target_link_libraries(sigscan)
