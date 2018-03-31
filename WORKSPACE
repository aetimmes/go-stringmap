http_archive(
    name = "io_bazel_rules_go",
    sha256 = "4b2c61795ac2eefcb28f3eb8e1cb2d8fb3c2eafa0f6712473bc5f93728f38758",
    url = "https://github.com/bazelbuild/rules_go/releases/download/0.10.2/rules_go-0.10.2.tar.gz",
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "d03625db67e9fb0905bbd206fa97e32ae9da894fe234a493e7517fd25faec914",
    url = "https://github.com/bazelbuild/bazel-gazelle/releases/download/0.10.1/bazel-gazelle-0.10.1.tar.gz",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains", "go_repository")

go_repository(
    name = "com_github_go_redis_redis",
    importpath = "github.com/go-redis/redis",
    tag = "v6.10.2",
)

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

gazelle_dependencies()
