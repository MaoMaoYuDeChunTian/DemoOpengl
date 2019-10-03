set(GL_SOURCES 
    ${CMAKE_CURRENT_LIST_DIR}/stdafx.h
    ${CMAKE_CURRENT_LIST_DIR}/targetver.h

    ${CMAKE_CURRENT_LIST_DIR}/stdafx.cpp
    ${CMAKE_CURRENT_LIST_DIR}/GL.cpp
    ${PROJECT_SOURCE_DIR}/ThirdPart/glfw/include/glad/glad.c)

ADD_EXECUTABLE(GL ${GL_SOURCES})

target_include_directories(GL PUBLIC 
)

target_link_libraries(GL PUBLIC
opengl32.lib
glfw3.lib
)