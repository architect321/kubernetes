load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "debug_disable.go",
        "diff.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/google/go-cmp/cmp/internal/diff",
    importpath = "github.com/google/go-cmp/cmp/internal/diff",
    visibility = ["//vendor/github.com/google/go-cmp/cmp:__subpackages__"],
    deps = ["//vendor/github.com/google/go-cmp/cmp/internal/flags:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
