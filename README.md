# SDKMAN! website

## Releases

The SBT release plugin performs the release process. _semver_ is used as versioning scheme.

### Patch release

Pull requests merged to `master` branch will result in a patch version bump. A new image of the version will be built
and pushed to Docker Hub.

### Major and minor releases

A minor release can be achieved by updating the `version.sbt` file. Update the version to the next minor version
snapshot. For example, if the current version is `0.76.3-SNAPSHOT`, change it to be `0.77.0-SNAPSHOT`. The next
published Docker image will be `0.77.0`, and the corresponding Git tag `v0.77.0`.

You can achieve a major release in much the same way.