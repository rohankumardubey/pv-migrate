# Contributing

Contributing to the project is simple. Just do the following:

1. Be nice :)

2. If you are not sure about something (e.g. if something is a bug, on how to solve it, if a feature makes sense etc.),
   before starting to work on it, create an issue for it, so that we can discuss beforehand - maybe saving your time.

3. Fork the repo, do your changes, create a PR.

4. Make sure the build succeeds. Do the changes from after the review if needed.

That's it.

## Creating Releases

- To make a release of `pv-migrate` itself, push an annotated tag. Example:
  ```bash
  git tag -a v0.5.3 -m "Release v0.5.3"
  git push
  git push --tags
  ```

- To make a release of docker images, use their special tag prefixes, followed by the version. Example:
  ```bash
  git tag -a "docker-sshd-1.0.0" -m "Docker Sshd Image Release 1.0.0"
  git tag -a "docker-rsync-1.0.0" -m "Docker Rsync Image Release 1.0.0"
  git push
  push --tags
  ```
  These will result in the Docker images with the following tags being pushed:
  ```
  docker.io/utkuozdemir/pv-migrate-sshd:1.0.0
  docker.io/utkuozdemir/pv-migrate-rsync:1.0.0
  ```
