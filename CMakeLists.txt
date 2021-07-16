project(glad C)

set(SOURCES 
    include/glad/glad.h 
    include/KHR/khrplatform.h
    src/glad.c
)

add_library(glad STATIC ${SOURCES})
target_include_directories(glad PUBLIC 
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)