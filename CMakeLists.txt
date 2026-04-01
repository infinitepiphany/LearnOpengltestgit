cmake_minimum_required(VERSION 3.0)

project(LearnOpenGL001)

include_directories(include)



add_executable(LearnOpenGL001 src/main.cpp src/glad.c)


# 建议改为小写的 GL，或者使用更健壮的写法
target_link_libraries(LearnOpenGL001 glfw GL dl pthread m)