git_repository(
    name = "io_bazel_rules_docker",
    remote = "https://github.com/bazelbuild/rules_docker.git",
    tag = "v0.1.0",
)

load("@io_bazel_rules_docker//docker:docker.bzl", "docker_repositories")

docker_repositories()

git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    commit = "4be196cc186da9dd396d5a45a3a7f343b6abe2b0",
)

load("@io_bazel_rules_go//go:def.bzl", "go_repositories")

go_repositories()

# If i get rid of this section it's still broken?
# ERROR: error loading package '': Extension file not found. Unable to load package for '@io_bazel_rules_docker//docker/contrib/go:image.bzl': BUILD file not found on package path.
load(
    "@io_bazel_rules_docker//docker/contrib/go:image.bzl",
    _go_image_repos = "repositories",
)

_go_image_repos()
