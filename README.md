# gh-action-runner

A containerised GitHub Action runner, currently only applicable to
the [github-actions-learning](https://github.com/matthewwjones/github-actions-learning) repo.

## Docker Build

To run a Docker build for the GH Action runner:

```bash
$ docker build --build-arg gh_token=<your GitHub runner registration token> -t gh-agent:latest .
```

## Docker Run

To run in the foreground following a successful build and registration:

```bash
$ docker run -it gh-agent:latest
```