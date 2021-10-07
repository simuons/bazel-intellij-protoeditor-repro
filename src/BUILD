package(default_visibility = ["//visibility:public"])

proto_library(
    name = "a_proto",
    srcs = ["a.proto"],
)

proto_library(
    name = "b_proto",
    srcs = ["b.proto"],
    deps = [":a_proto"],
)

proto_library(
    name = "c_proto",
    srcs = ["c.proto"],
    import_prefix = "prefix",
)

proto_library(
    name = "d_proto",
    srcs = ["d.proto"],
    strip_import_prefix = "/src",
)

proto_library(
    name = "e_proto",
    srcs = ["e.proto"],
    import_prefix = "prefix",
    strip_import_prefix = "/src",
)

proto_library(
    name = "x_proto",
    srcs = ["nested/x.proto"],
    strip_import_prefix = "nested",
)

proto_library(
    name = "y_proto",
    srcs = ["nested/y.proto"],
    strip_import_prefix = "/src/nested",
)

proto_library(
    name = "z_proto",
    srcs = ["nested/z.proto"],
    strip_import_prefix = "/src",
)
