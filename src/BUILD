load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library", "go_test")
load("@io_bazel_rules_docker//docker/contrib/go:image.bzl", "go_image")

go_binary(
    name = "hello_world",
    srcs = ["main.go"],
)

go_image(
    name = "hello_world_image",
    srcs = ["main.go"],
)
