# Demos
Short overview for all examples in this directory

## How to use
Each directory contains `README.md` file with description about particular part of Jenkins configuration and `*.yaml` examples for correct setup. To use provided example just add that YAML configurations in your main configuration file at the proper level. If additional files are required it will be described in `README.md` file.

## Contributing
To add new demo prepare `README.md` file with description for your example and YAML configuration which allows bring it to work. Provide all not obvious tricks and tips.

If your configuration has multiple options it would be perfect if you could provide full and minimal versions in two different `*.yaml` files. If configuration requires additional files (like Kubernetes) add them too.

**All provided configurations in demo have to be tested:**
* create test class for your demo
* use `JenkinsConfiguredWithReadmeRule` to get configuration from your `README.md` file
* implement test cases for your demo to cover whole configuration
* for example check `ArtifactoryTest` and others. See also [PR #1055](https://github.com/jenkinsci/configuration-as-code-plugin/pull/1055)

## Notice
* Some options are supported from a specific version - some of them may not be applicable to all JCasC plugin versions.