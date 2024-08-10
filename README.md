# Github Actions: App 1
working demo of a github action ci-cd

## What is YAML?
Yet Another Markup Language
YAML is a human-readable data serialization format that uses indentation and key-value pairs.

CI is the practice of frequently merging code changes into a shared repository and automatically building and testing the application.
CD extends CI by automating the deployment process, ensuring that tested and validated code is delivered to production environments.

It typically includes stages like building, testing, and deploying the application, often triggered by changes in the code repository.

## How to build a pipeline?

**Define stages**: Start by outlining the different stages of your pipeline, such as build, test, and deploy.

**Specify tasks**: Within each stage, define the tasks or commands to be executed. For example, running tests, building artifacts, or deploying to a server.

**Set dependencies**: Configure dependencies between stages and tasks. For instance, the deploy stage should depend on the successful completion of the test stage.

**Configure triggers**: Specify the conditions that trigger pipeline execution, such as a new commit pushed to the repository or a manual trigger.

**Define environment variables**: If required, define environment-specific variables like API keys or database connections.

Tools that support CI/CD: 

**Jenkins**: A widely used open-source automation server.

**GitLab CI/CD**: An integrated DevOps platform with built-in CI/CD capabilities.

**GitHub Actions**: Native CI/CD workflows integrated with GitHub repositories.

## Events of GitHub Actions

- Events
  - Pull, Push, Issue (create, close etc.)
  - tied to workflows
- Jobs
  - composed of steps
  - associated with runners
    - Runners come in different flavors (GitHub hosted runners OR self-hosted runners)
- Step
  - composed of actions


What is a context in actions?
dumping the github event payload inside the pipeline run.

If you are getting the following error when you run these aciton codes:
 
`Resource not accessible by integration.` 

Following these steps may solve the problem.
1- Go to repository "Settings".
2- After that it will show you a left pane where you will find "Actions"
3- Expand "Actions" tab
4- Click on "General" under options tab.
5- Now on new page scroll down and you will fine "Workflow Permissions"
6- Select "Read and Write" under "Workflow Permissions".


