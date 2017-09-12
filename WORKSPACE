git_repository(
    name = "io_bazel_rules_docker",
    remote = "https://github.com/bazelbuild/rules_docker.git",
    commit = "65df68f4f64e9c59eb571290eb86bf07766393b6",
)

load("@io_bazel_rules_docker//docker:docker.bzl", "docker_repositories")

docker_repositories()

git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    tag = "0.5.4",
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
