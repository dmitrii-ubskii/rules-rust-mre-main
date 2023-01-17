load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
git_repository(
    name = "external",
    remote = "https://github.com/dmitrii-ubskii/rules-rust-mre-external",
    commit = "f75b1d025fe57bccfb7f3710403f9b1d82910654",
)

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
http_archive(
    name = "rules_rust",
    sha256 = "aaaa4b9591a5dad8d8907ae2dbe6e0eb49e6314946ce4c7149241648e56a1277",
    urls = ["https://github.com/bazelbuild/rules_rust/releases/download/0.16.1/rules_rust-v0.16.1.tar.gz"],
)

load("@rules_rust//rust:repositories.bzl", "rules_rust_dependencies", "rust_register_toolchains")
rules_rust_dependencies()
rust_register_toolchains(edition = "2021")
