# Declare the local Bazel workspace.
# This is *not* included in the published distribution.
workspace(
    # see https://docs.bazel.build/versions/main/skylark/deploying.html#workspace
    name = "dev_aspect_rules_webpack",
)

# Install our "runtime" dependencies which users install as well
load("//webpack:repositories.bzl", "rules_webpack_dependencies")

rules_webpack_dependencies()

load(":internal_deps.bzl", "rules_webpack_internal_deps")

rules_webpack_internal_deps()