load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "cel",
    srcs = [
        "compile.go",
        "composition.go",
        "filter.go",
        "interface.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/k8s.io/apiserver/pkg/admission/plugin/cel",
    importpath = "k8s.io/apiserver/pkg/admission/plugin/cel",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/google/cel-go/cel",
        "//vendor/github.com/google/cel-go/common/types",
        "//vendor/github.com/google/cel-go/common/types/ref",
        "//vendor/github.com/google/cel-go/interpreter",
        "//vendor/k8s.io/api/admission/v1:admission",
        "//vendor/k8s.io/api/authentication/v1:authentication",
        "//vendor/k8s.io/api/core/v1:core",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:meta",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured",
        "//vendor/k8s.io/apimachinery/pkg/runtime",
        "//vendor/k8s.io/apimachinery/pkg/util/version",
        "//vendor/k8s.io/apiserver/pkg/admission",
        "//vendor/k8s.io/apiserver/pkg/apis/cel",
        "//vendor/k8s.io/apiserver/pkg/authorization/authorizer",
        "//vendor/k8s.io/apiserver/pkg/cel",
        "//vendor/k8s.io/apiserver/pkg/cel/environment",
        "//vendor/k8s.io/apiserver/pkg/cel/lazy",
        "//vendor/k8s.io/apiserver/pkg/cel/library",
    ],
)
