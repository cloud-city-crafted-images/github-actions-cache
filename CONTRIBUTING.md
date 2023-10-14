# Cloud City Crafted GitHub Actions Images Contributing Guide

Cloud City Crafted stores container images via [GitHub Packages](https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages).

## 🛠️ Building Images

To build an image, run:

```shell
docker build \
    --platform linux/amd64 \
    --tag github-actions-<ACTION_NAME>:latest \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-<ACTION_NAME>:latest \
    --tag github-actions-<ACTION_NAME>:<VERSION_TAG> \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-<ACTION_NAME>:<VERSION_TAG> \
    ./<ACTION_NAME>
```

where:

- `<ACTION_NAME>`: Name of the GitHub Action being emulated (e.g., `cache`)
- `<VERSION_TAG>`: Major version of the image (e.g., `v1`)

For example, to build the `v1` version of the cache action, use:

```shell
docker build \
    --platform linux/amd64 \
    --tag github-actions-cache:latest \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-cache:latest \
    --tag github-actions-cache:v1 \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-cache:v1 \
    ./cache
```

## 🚀 Deploying Images

To deploy an image to the GitHub Container Registry, use:

```shell
docker push --all-tags ghcr.io/cloud-city-crafted-images/github-actions-<ACTION_NAME>
```

where:

- `<ACTION_NAME>`: Name of the GitHub Action being emulated (e.g., `cache`)

For example, to push all github-action-cache images, use:

```shell
docker push --all-tags ghcr.io/cloud-city-crafted-images/github-actions-cache
```
