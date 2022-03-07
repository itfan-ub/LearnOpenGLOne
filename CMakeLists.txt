project(LearnOpenGLOne)

cmake_minimum_required(VERSION 3.2.0)

include_directories(ext/stb)

include_directories(ext/glm)
add_subdirectory(ext/glm)

include_directories(ext/glfw/include)
add_subdirectory(ext/glfw)

include_directories(include/glad/include)
include_directories(include)

cmake_minimum_required(VERSION 3.2.0)

add_executable(lessonOne src/main.cpp src/glad.c)
target_link_libraries(lessonOne glfw glm)
