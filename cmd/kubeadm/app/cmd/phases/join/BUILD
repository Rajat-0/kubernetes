load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "checketcd.go",
        "controlplane.go",
        "preflight.go",
    ],
    importpath = "k8s.io/kubernetes/cmd/kubeadm/app/cmd/phases/join",
    visibility = ["//visibility:public"],
    deps = [
        "//cmd/kubeadm/app/apis/kubeadm:go_default_library",
        "//cmd/kubeadm/app/cmd/options:go_default_library",
        "//cmd/kubeadm/app/cmd/phases/workflow:go_default_library",
        "//cmd/kubeadm/app/cmd/util:go_default_library",
        "//cmd/kubeadm/app/constants:go_default_library",
        "//cmd/kubeadm/app/phases/certs:go_default_library",
        "//cmd/kubeadm/app/phases/controlplane:go_default_library",
        "//cmd/kubeadm/app/phases/etcd:go_default_library",
        "//cmd/kubeadm/app/phases/kubeconfig:go_default_library",
        "//cmd/kubeadm/app/preflight:go_default_library",
        "//pkg/util/normalizer:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/github.com/lithammer/dedent:go_default_library",
        "//vendor/github.com/pkg/errors:go_default_library",
        "//vendor/k8s.io/klog:go_default_library",
        "//vendor/k8s.io/utils/exec:go_default_library",
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
