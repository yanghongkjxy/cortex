load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "collector.go",
        "tracer.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/apache/thrift/lib/go/thrift:go_default_library",
        "//vendor/github.com/opentracing/opentracing-go:go_default_library",
        "//vendor/github.com/openzipkin/zipkin-go-opentracing:go_default_library",
        "//vendor/github.com/openzipkin/zipkin-go-opentracing/_thrift/gen-go/zipkincore:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["collector_test.go"],
    library = ":go_default_library",
    deps = [
        "//vendor/github.com/davecgh/go-spew/spew:go_default_library",
        "//vendor/github.com/openzipkin/zipkin-go-opentracing/_thrift/gen-go/zipkincore:go_default_library",
        "//vendor/github.com/pmezard/go-difflib/difflib:go_default_library",
    ],
)
