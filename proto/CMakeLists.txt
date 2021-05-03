find_package(Protobuf REQUIRED)
protobuf_generate_cpp(PROTO_SRC PROTO_HEADER message.proto)
add_library(proto STATIC ${PROTO_HEADER} ${PROTO_SRC})
