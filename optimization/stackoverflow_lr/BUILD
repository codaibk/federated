load("@rules_python//python:defs.bzl", "py_library")

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

py_library(
    name = "centralized_stackoverflow_lr",
    srcs = ["centralized_stackoverflow_lr.py"],
    srcs_version = "PY3",
    deps = [
        "//utils:centralized_training_loop",
        "//utils/datasets:stackoverflow_tag_prediction",
        "//utils/models:stackoverflow_lr_models",
    ],
)

py_library(
    name = "federated_stackoverflow_lr",
    srcs = ["federated_stackoverflow_lr.py"],
    srcs_version = "PY3",
    deps = [
        "//optimization/shared:training_specs",
        "//utils:training_utils",
        "//utils/datasets:stackoverflow_tag_prediction",
        "//utils/models:stackoverflow_lr_models",
    ],
)
