project(capnpc-C)

add_executable(${PROJECT_NAME} capnpc-c.c schema.capnp.c str.c)
target_link_libraries(${PROJECT_NAME} capnp_c::lib)