# frigate-synology-dsm7
![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/DismissedGuy/frigate-synology-dsm7/docker-publish.yml)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/DismissedGuy/frigate-synology-dsm7/main)

A fork of @weltenwort's [frigate-synology-dsm7](https://github.com/weltenwort/frigate-synology-dsm7) that follows the latest frigate stable tag.

This repository provides a Docker image for [frigate](https://github.com/blakeblackshear/frigate) that supports using a Google Coral USB TPU. It is based on the official upstream frigate image but recompiles `libusb1` without `udev` support.

## Usage
Follow the [official installation instructions](https://docs.frigate.video/frigate/installation/#docker), **making sure to replace the image name:**
```diff
- ghcr.io/blakeblackshear/frigate:stable
+ ghcr.io/dismissedguy/frigate-synology-dsm7:stable
```

There is also a [docker-compose.yml](./docker-compose.yml) file which you can use as reference.
