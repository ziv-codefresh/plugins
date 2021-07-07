# Trigger Jenkins Job


## Run locally
`go get codefresh-io/cf-run-jenkins-job`
```
NAME:
   cf-run-jenkins-job

DESCRIPTION:
   Trigger Jenkins Job

## Mandatory Parameters:

    JENKINS_URL     - Jenkins Master URL
    JENKINS_USER    - Jenkins User Name
    JENKINS_TOKEN   - Jenkins Token
    JENKINS_JOB     - Jenkins Job Name

## Usage Example:

version: '1.0'
steps:
  RunJenkins:
    title: Triggering Jenkins Job
    image: codefresh/cf-run-jenkins-job
    environment:
    - JENKINS_URL=http://<jenkins host>:<jenkins port>
    - JENKINS_USER=<jenkins user name>
    - JENKINS_TOKEN=<jenkins token>
    - JENKINS_JOB=<jenkins job name>
