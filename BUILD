load("@rules_rust//rust:defs.bzl", "rust_binary")

rust_binary(
    name = "bin",
    srcs = ["src/main.rs"],
    deps = ["@external//rust:lib-with-gen"],
)

