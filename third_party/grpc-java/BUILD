package(default_visibility = ["//visibility:public"])

licenses(["unencumbered"])  # BSD

filegroup(
    name = "license",
    srcs = ["LICENSE"],
)

cc_binary(
    name = "plugin",
    srcs = [
        "compiler/src/java_plugin/cpp/java_generator.cpp",
        "compiler/src/java_plugin/cpp/java_generator.h",
        "compiler/src/java_plugin/cpp/java_plugin.cpp",
    ],
    deps = ["@protobuf//:protoc_lib"],
)

java_library(
    name = "grpc-all",
    visibility = ["//visibility:public"],
    exports = [
        "@com_google_auth_google_auth_library_credentials//jar",
        "@com_google_code_findbugs_jsr305//jar",
        "@com_google_code_gson_gson//jar",
        "@com_google_guava_guava//jar",
        "@com_google_protobuf_nano_protobuf_javanano//jar",
        "@com_google_protobuf_protobuf_java//jar",
        "@com_google_protobuf_protobuf_java_util//jar",
        "@com_google_protobuf_protobuf_lite//jar",
        "@com_squareup_okhttp_okhttp//jar",
        "@com_squareup_okio_okio//jar",
        "@io_grpc_grpc_all//jar",
        "@io_grpc_grpc_auth//jar",
        "@io_grpc_grpc_core//jar",
        "@io_grpc_grpc_netty//jar",
        "@io_grpc_grpc_okhttp//jar",
        "@io_grpc_grpc_protobuf//jar",
        "@io_grpc_grpc_protobuf_lite//jar",
        "@io_grpc_grpc_protobuf_nano//jar",
        "@io_grpc_grpc_stub//jar",
        "@io_netty_netty_buffer_grpc//jar",
        "@io_netty_netty_codec_grpc//jar",
        "@io_netty_netty_codec_http_grpc//jar",
        "@io_netty_netty_codec_http2_grpc//jar",
        "@io_netty_netty_common_grpc//jar",
        "@io_netty_netty_handler_grpc//jar",
        "@io_netty_netty_resolver_grpc//jar",
        "@io_netty_netty_transport_grpc//jar",
    ],
)

java_library(
    name = "grpc-stub",
    visibility = ["//visibility:public"],
    exports = [
        "@com_google_code_findbugs_jsr305//jar",
        "@com_google_code_gson_gson//jar",
        "@com_google_guava_guava//jar",
        "@com_google_protobuf_protobuf_java//jar",
        "@com_google_protobuf_protobuf_java_util//jar",
        "@io_grpc_grpc_core//jar",
        "@io_grpc_grpc_protobuf//jar",
        "@io_grpc_grpc_protobuf_lite//jar",
        "@io_grpc_grpc_stub//jar",
    ],
)

java_library(
  name="grpc-netty",
  visibility = ["//visibility:public"],
  exports = [
    "@com_google_code_findbugs_jsr305//jar",
    "@com_google_guava_guava//jar",
    "@io_grpc_grpc_core//jar",
    "@io_grpc_grpc_netty//jar",
    "@io_netty_netty_buffer_grpc//jar",
    "@io_netty_netty_codec_grpc//jar",
    "@io_netty_netty_codec_http_grpc//jar",
    "@io_netty_netty_codec_http2_grpc//jar",
    "@io_netty_netty_common_grpc//jar",
    "@io_netty_netty_handler_grpc//jar",
    "@io_netty_netty_resolver_grpc//jar",
    "@io_netty_netty_transport_grpc//jar",
  ],
)

java_library(
  name="grpc-okhttp",
  visibility = ["//visibility:public"],
  exports = [
    "@com_google_code_findbugs_jsr305//jar",
    "@com_google_guava_guava//jar",
    "@com_squareup_okhttp_okhttp//jar",
    "@com_squareup_okio_okio//jar",
    "@io_grpc_grpc_core//jar",
    "@io_grpc_grpc_okhttp//jar",
  ],
)