cmake_minimum_required(VERSION 3.16)

project(Hello)

add_executable(${PROJECT_NAME} Hello.cpp)

install(TARGETS 
    ${PROJECT_NAME}
)
