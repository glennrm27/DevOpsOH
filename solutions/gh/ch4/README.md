# Challenge 4

All workflows are implemented in the `.github/workflows` folder. There are four versions for each API: _Trips_, _POI_, _User_, and _UserJava_.

## Challenge

A _pull request_ workflow needs to be built, which builds API, unit tests the API, and publishes test results. It is triggered by pull request creation.

The solution is split into five files:

- POI
- POI v2
- Trips
- UserJava
- User

Using the `workflow_dispatch:` trigger enables this workflow to be started manually, which is useful for testing. The team no longer has to make arbitrary code changes just to trigger the workflow.

### PR

The PR trigger in YAML code automatically triggers the pull request workflow. Ensure that the branch and paths are correct:

```yml
on:
  pull_request:
    branches:
      - main
    paths:
      - "apis/poi/**"
  workflow_dispatch:
```

To test the functionality, create a new branch, push some changes in the IaC files and create a pull request against the `main` branch. After a few seconds, the automated check should trigger.
