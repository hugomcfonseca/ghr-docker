# ghr-docker

[ghr](https://github.com/tcnksm/ghr) running on the top of a Docker container.

## Usage

```bash
$ docker run --rm \
    --volumes /path/to/repo/:/app \
    -e GITHUB_TOKEN=$TOKEN \
    hugomcfonseca/ghr:0.12.0 \
      -n "<RELEASE_TITLE>" \
      -b "<RELEASE_DESCRIPTION>" \
      -soft \
      <TAG> <OUTPUT_DIRECTORY>
```
