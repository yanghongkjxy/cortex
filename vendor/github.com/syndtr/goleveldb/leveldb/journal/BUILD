load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["journal.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/syndtr/goleveldb/leveldb/errors:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/storage:go_default_library",
        "//vendor/github.com/syndtr/goleveldb/leveldb/util:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["journal_test.go"],
    library = ":go_default_library",
)
