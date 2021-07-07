# Codefresh plugins 

Codefresh Plugins are Docker images made especially for use in Codefresh freestyle steps. Each plugin facilitates a common task that would otherwise be difficult to achieve.
See each plugin readme for more info and usage instructions.

## Plugins

| Plugin|  Description| Tags|
| --- | --- |  --- |
| [Helm](plugins/helm/README.md) | Deploy Helm charts | `kubernetes` `helm`|
| [Codefresh Cli](plugins/codefresh-cli/README.md) | Operate on Codefresh resources | `cli` `codefresh`|
| [Slack](plugins/slack/README.md)| Send message to slack| `slack` `notify`|
| [Deploy to ECS](plugins/ecs-deploy/README.md)| Deploy docker image to ECS| `ecs` `deploy` `containers` `aws`                         |
| [Deploy Kompose](plugins/kompose/README.md)| Deploy Docker Compose to Kubernetes cluster with Kubernetes [Kompose](http://kompose.io) | `docker` `docker-compose` `kompose` `deploy` `kubernetes` |
| [GitHub PR](plugins/github-pr/README.MD)| Operates on pull requests on GitHub | `github` `pull-request` |
| [Run Jenkins Jobs](plugins/run-jenkins-job/README.md)| Run jenkins job from codefresh pipeline| `jenkins` `job`|
| [Deploy to DCOS](plugins/dcos-app-deploy/README.md) | Deploy application image to DC/OS cluster | `dcos` `deploy` `containers` |
| [Interact with Jira](plugins/jira/README.md) | Interact with Jira from codefresh pipelines| `jira` `workflow`|
| [Makisu](plugins/makisu/README.md) | Building images using the Makisu tool | `makisu` `uber`|
| [release to npm](plugins/release-to-NPM/README.md) | Release npm modules from a pipeline | `npm` |
| [Twistlock](plugins/cfstep-twistlock) | Security scanning of docker images using Twistlock | `security` |
| [Clair](plugins/clair/README.md) |  Security scanning of Docker images using Clair | `security` |
| [Import Docker Images](plugins/import-docker-images/README.md) | Import Docker images metadata into Codefresh| `docker` `codefresh`|
| [Google KMS](plugins/google-kms/README.md) | Encryption/Decryption with Google KMS| `KMS` `codefresh`|
| [Github Release](plugins/github-release/README.md) | Managing GitHub releases | `github` `release`|
| [Google GKE](plugins/gke/README.md) | GKE Clusters | `GKE` `codefresh`|
| [Vault](plugins/vault/README.md) | Export Vault Key/Value pairs as ENV variables | `Vault` `codefresh`|
