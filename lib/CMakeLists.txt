project(capnp_c)

add_library(${PROJECT_NAME} capn.c capn-malloc.c capn-stream.c)
add_library(capnp_c::lib ALIAS ${PROJECT_NAME})
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR})