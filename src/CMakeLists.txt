set(Protobuf_USE_STATIC_LIBS ON)
find_package(Protobuf REQUIRED)

add_executable(main main.cpp)
message(STATUS "hello ${Protobuf_LIBRARY}")
target_link_libraries(main proto ${Protobuf_LIBRARY})
target_include_directories(main PUBLIC ${CMAKE_BINARY_DIR})

