project(LearnOpenGLOne)




include_directories(ext/glfw/include)
add_subdirectory(ext/glfw)

include_directories(include/glad/include)

cmake_minimum_required(VERSION 3.2.0)

add_executable(lessonOne src/main.cpp src/glad.c)
target_link_libraries(lessonOne glfw)
