# Cloud City Crafted GitHub Actions Container Images

This repository contains the configuration and scripts needed to create container images for Cloud City Crafted continuous integration (CI) and runtime environments.

## ✨ Quick Start

Ensure you have [Docker](https://docs.docker.com/get-docker/) installed.

> Note: All runner images are compatible with [act](https://github.com/nektos/act) as alternative runner images.

To pull container images, run:

```shell
docker pull ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>:latest
```

And ta-da 🎉! You're ready to run Cloud City Crafted GitHub Actions images locally!

## 📦 Images

| Image                | Available Tags | Included Packages                                            |
| -------------------- | -------------- | ------------------------------------------------------------ |
| github-actions-cache | `latest`, `v1` | [GitHub Actions Cache Packages](./cache/README.md#-packages) |

## 🪪 License

This repository is [MIT licensed](./LICENSE).

Base images are subject to their respective open source license(s):

- [Debian](https://www.debian.org/legal/licenses/)
