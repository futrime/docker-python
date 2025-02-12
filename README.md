# docker-python

Docker in Docker with Python

This image is [python](https://hub.docker.com/_/python) built upon [docker](https://hub.docker.com/_/docker).

## Usage

This image is available on GitHub Container Registry.

```sh
docker pull ghcr.io/futrime/docker-python:latest
```

If you are create image from this image, remember to run `dockerd-entrypoint.sh` in the background before running any Python script that uses Docker. Here is an example of entrypoint script (assume the Python script is named `script.py`):

```sh
#!/bin/sh

dockerd-entrypoint.sh &

python script.py
```

## Tags

- [`27.5-py3.11`, `27-py3.11`, `py3.11`](27/py3.11/Dockerfile)
- [`27.5-py3.12`, `27-py3.12`, `py3.12`](27/py3.12/Dockerfile)
- [`27.5-py3.13`, `27.5-py3`, `27.5`, `27-py3.13`, `27-py3`, `27`, `py3.13`, `py3`, `latest`](27/py3.13/Dockerfile)

## Thanks

- [docker-library/python](https://github.com/docker-library/python): [MIT License](https://github.com/docker-library/python/blob/master/LICENSE)

## Contributing

PRs accepted.

## License

MIT © Zijian Zhang
