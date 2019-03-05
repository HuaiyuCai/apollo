package(default_visibility = ["//visibility:public"])

licenses(["notice"])

cc_library(
    name = "pytorch",
    hdrs = glob(["*"]),
    srcs = glob(["lib/*.so"]),
    includes = [
        "include",
        "include/torch/csrc/api/include",
        "include/torch/csrc/api/include/torch"
    ],
    copts = [
        "-Iinclude",
        "-Iinclude/torch",
        "-Iinclude/torch/csrc/api/include/torch",
    ],
    linkopts = [
        "-Llib",
    ],
    deps = [
        "@gtest",
        "@python27",
        "@cuda",
    ]
)
