load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "expansion_generated.go",
        "runtimeclass.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/k8s.io/node-api/pkg/client/listers/node/v1alpha1",
    importpath = "k8s.io/node-api/pkg/client/listers/node/v1alpha1",
    visibility = ["//visibility:public"],
    deps = [
        "//staging/src/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/node-api/pkg/apis/node/v1alpha1:go_default_library",
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
