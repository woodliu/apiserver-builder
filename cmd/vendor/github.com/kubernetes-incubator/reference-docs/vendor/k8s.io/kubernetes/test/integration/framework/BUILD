package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "etcd.go",
        "master_utils.go",
        "perf_utils.go",
        "serializer.go",
        "util.go",
    ],
    data = [
        "@com_coreos_etcd//:etcd",
    ],
    importpath = "k8s.io/kubernetes/test/integration/framework",
    deps = [
        "//vendor/github.com/go-openapi/spec:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/pborman/uuid:go_default_library",
        "//vendor/k8s.io/api/apps/v1beta1:go_default_library",
        "//vendor/k8s.io/api/autoscaling/v1:go_default_library",
        "//vendor/k8s.io/api/certificates/v1beta1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1alpha1:go_default_library",
        "//vendor/k8s.io/api/storage/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/serializer/versioning:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/authenticator:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/authenticatorfactory:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/union:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authorization/authorizer:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authorization/authorizerfactory:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authorization/union:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/options:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/storage:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/storage/storagebackend:go_default_library",
        "//vendor/k8s.io/client-go/informers:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/client-go/tools/record:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/testapi:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/batch:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/policy/v1alpha1:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/clientset_generated/internalclientset:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/controller:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/controller/replication:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/generated/openapi:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubelet/client:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/master:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/env:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/version:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/admit:go_default_library",
        "//vendor/k8s.io/kubernetes/test/e2e/framework:go_default_library",
        "//vendor/k8s.io/kubernetes/test/utils:go_default_library",
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
)
