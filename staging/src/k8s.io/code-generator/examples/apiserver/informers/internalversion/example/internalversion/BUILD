load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "interface.go",
        "testtype.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/k8s.io/code-generator/examples/apiserver/informers/internalversion/example/internalversion",
    importpath = "k8s.io/code-generator/examples/apiserver/informers/internalversion/example/internalversion",
    visibility = ["//visibility:public"],
    deps = [
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/apiserver/apis/example:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/apiserver/clientset/internalversion:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/apiserver/informers/internalversion/internalinterfaces:go_default_library",
        "//staging/src/k8s.io/code-generator/examples/apiserver/listers/example/internalversion:go_default_library",
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
