load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "directed_acyclic.go",
        "edgeholder.go",
        "simple.go",
        "undirected.go",
    ],
    importpath = "k8s.io/kubernetes/third_party/forked/gonum/graph/simple",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/golang.org/x/tools/container/intsets:go_default_library",
        "//vendor/k8s.io/kubernetes/third_party/forked/gonum/graph:go_default_library",
    ],
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
