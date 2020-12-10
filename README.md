# rpi-kubernetes

export GITHUB_USER=franktylerva
export GITHUB_REPO=rpi-kubernetes
export GITHUB_TOKEN=<your-token>


flux bootstrap github \
    --owner=${GITHUB_USER} \
    --repository=${GITHUB_REPO} \
    --branch=main \
    --personal \
    --path=clusters/staging \
    --arch=arm64