workspace(name = "bazel_intellij_protoeditor_repro")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_proto",
    sha256 = "8e7d59a5b12b233be5652e3d29f42fba01c7cbab09f6b3a8d0a57ed6d1e9a0da",
    strip_prefix = "rules_proto-7e4afce6fe62dbff0a4a03450143146f9f2d7488",
    urls = [
        "https://mirror.bazel.build/github.com/bazelbuild/rules_proto/archive/7e4afce6fe62dbff0a4a03450143146f9f2d7488.tar.gz",
        "https://github.com/bazelbuild/rules_proto/archive/7e4afce6fe62dbff0a4a03450143146f9f2d7488.tar.gz",
    ],
)

load("@rules_proto//proto:repositories.bzl", "rules_proto_dependencies", "rules_proto_toolchains")

rules_proto_dependencies()

rules_proto_toolchains()

http_archive(
    name = "google_api_protos",
    sha256 = "9ecae675e5f169f93bf07d8ff80b51444c8eb57b10beba2e0657a317bdf378a4",
    strip_prefix = "googleapis-c911062bb7a1c41a208957bed923b8750f3b6f28",
    urls = ["https://github.com/googleapis/googleapis/archive/c911062bb7a1c41a208957bed923b8750f3b6f28.zip"],
)
