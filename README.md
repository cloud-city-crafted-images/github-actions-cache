# Cloud City Crafted GitHub Actions Container Images

This repository contains the configuration and scripts needed to create container images to emulate GitHub Actions for Cloud City Crafted test and continuous integration (CI) environments.

## ✨ Quick Start

Ensure you have [Docker](https://docs.docker.com/get-docker/) installed.

> Note: All runner images are compatible with [act](https://github.com/nektos/act) as alternative runner images.

To pull container images, run:

```shell
docker pull ghcr.io/cloud-city-crafted-images/github-actions-<ACTION>:latest
```

And ta-da 🎉! You're ready to use Cloud City Crafted GitHub Actions images locally!

## 📦 Images

| Image                                                                                                                   | Available Tags | Included Packages                                  |
| ----------------------------------------------------------------------------------------------------------------------- | -------------- | -------------------------------------------------- |
| [github-actions-cache](https://github.com/cloud-city-crafted-images/github-actions/pkgs/container/github-actions-cache) | `latest`, `v1` | [GitHub Actions Cache Packages](./cache#-packages) |

## 🪪 License

This repository is [MIT licensed](./LICENSE).

Base images are subject to their respective open source license(s):

- [Debian](https://www.debian.org/legal/licenses/)
