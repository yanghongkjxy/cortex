load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "errors.go",
        "firsthit_restmapper.go",
        "help.go",
        "interfaces.go",
        "meta.go",
        "multirestmapper.go",
        "priority.go",
        "restmapper.go",
        "unstructured.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/api/meta/metatypes:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/api/unversioned:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/conversion:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/runtime:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/types:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/sets:go_default_library",
    ],
)
