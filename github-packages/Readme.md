This is my New repo
export GH_USERNAME="venkatsh0812"
export GH_TOKEN=""
GH_IMAGE_NAME="hello-world"
export GH_VER="1.0.0"

echo $GH_TOKEN | docker login ghcr.io -u $GH_USERNAME --password-stdin

docker tag hello-world:latest ghcr.io/venkatsh0812/hello-world:1.0.0

docker push ghcr.io/venkatsh0812/hello-world:1.0.0


LABEL org.opencontainers.image.source https://github.com/OWNER/REPO
