# Docker electrs

Dockerfile of the public image [catalogfi/electrs](https://ghcr.io/catalogfi/electrs)

## Electrs

Pull the image:

```bash
$ docker pull ghcr.io/catalogfi/electrs
```

Run the container:

```bash
$ docker run -p 3002:3002 -d ghcr.io/catalogfi/electrs
```

## Release

To tag a new image with a new version:

1) Create a new folder with `COMMIT` as directory name and change the `Dockerfile`s ARG `COMMIT`
2) Modify the GH Action in `.github/workflows/docker-publish.yml` changing the `COMMIT` env var
3) Push in master
