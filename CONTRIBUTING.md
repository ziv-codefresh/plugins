# Contributing Guidelines

The Codefresh Plugins project accepts contributions via GitHub pull requests. This document outlines the process to help get your contribution accepted.


### Reporting a Bug in Plugin

This repository is used by Plugin developers for maintaining the official plugins for Codefresh. 

### How to Contribute a Plugin

1. Develop and test your plugin
2. Fork this repository
2. Choose the correct folder for your plugin based on the information in the [Repository Structure](docs/plugin.md#plugin-file-structure) section
3. Ensure your Plugin follows the [technical](#technical-requirements) and [documentation](#documentation-requirements) guidelines, described below
4. Update [Plugin Catalog](CATALOG.md)
5. Submit a pull request

***NOTE***: In order to make testing and merging of PRs easier, please submit changes to multiple plugins in separate PRs.

#### Technical requirements

* The Plugin with all its dependencies should be packaged into a single Docker container
* The Plugin code must be available as public GitHub repository
* It should be possible to build the Plugin using single `Dockerfile` (use *multi-stage* build if needed)
* The Plugin Docker Image should not have any major security vulnerabilities
* It should be possible to run the Plugin with simple `docker run` command, providing all required environment variables and volumes

#### Documentation requirements

* Must include an in-depth `README.md`, including:
    * Short description of the Plugin
    * Customization: explaining all required variables and their defaults
* Must include a short `NOTES.txt`, including:
    * Any relevant post/pre-installation information for the Plugin
    * Instructions on how to access the application or service provided by the Plugin

#### Merge approval and release process

A Codefresh Plugins maintainer will review the Plugin submission, and start a validation job in the CI to verify the technical requirements of the Plugin. A maintainer may add "LGTM" (Looks Good To Me) or an equivalent comment to indicate that a PR is acceptable. Any change requires at least one LGTM. No pull requests can be merged until at least one maintainer signs off with an LGTM.

Once the Plugin has been merged, the release job will automatically run in the CI to package and release the Plugin in the [`gs://codefresh-plugins` Google Storage bucket](https://console.cloud.google.com/storage/browser/codefresh-plugins/).

### Support Channels

Whether you are a user or contributor, official support channels include:

- GitHub issues: https://github.com/codefresh-io/plugins/issues
- Slack: *TBD*

Before opening a new issue or submitting a new pull request, it's helpful to search the project - it's likely that another user has already reported the issue you're facing, or it's a known issue that we're already aware of.
