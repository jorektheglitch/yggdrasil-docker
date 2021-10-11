# jorektheglitch / yggdrasil-docker

Run [Yggdrasil](https://yggdrasil-network.github.io/) node in a Docker container

This repository is a fork of [luzifer-docker / yggdrasil](https://github.com/luzifer-docker/yggdrasil) that was archived.

## Usage

```bash
## Build container (optional)
$ docker build -t jorektheglitch/yggdrasil .

## Create config and action file (if you don't the config will be
## generated on first run)
$ tree
.
└── yggdrasil.conf

0 directories, 2 files

## Execute yggdrasil node
$ docker run --rm -ti --net=host --cap-add=NET_ADMIN --device=/dev/net/tun -v $(pwd):/config jorektheglitch/yggdrasil
```

## Notes

### travis-ci

travis was disabled for some time in this repository.

## Special thanks

- [Котя](https://github.com/StalkerMeyr) Guy who modifies original docker image
