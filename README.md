# Kotlin + SpringBoot Parent POM

This repository is one of two components demonstrating how to use a git submodule as a parent POM.

### Example Usage

A template repository which uses this repository as a parent POM can be found 
[here](https://github.com/tajacks/kotlin-spring-boot-template).

### Releasing a Version

The release process for this POM uses GitHub Actions.

1. Ensure all changes to be committed as a version are on the `main` branch
   1. The `main` branch should be a `SNAPSHOT` release
2. Run the 'Release Parent POM' workflow from the Actions tab, specifying the version to release and the
next development version
3. Once the run is completed, there should be a Pull Request open if all went well. Merge it using the `rebase`
strategy
4. Double-check the tag was created for the version you released