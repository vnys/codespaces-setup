# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.158.0/containers/debian/.devcontainer/base.Dockerfile

# [Choice] Debian version: buster, stretch
ARG VARIANT="buster"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

RUN echo "deb http://deb.debian.org/debian buster-backports main" >> /etc/apt/sources.list
RUN echo "deb http://ftp.be.debian.org/debian unstable main contrib non-free" >> /etc/apt/sources.list

# ** [Optional] Uncomment this section to install additional packages. **
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends git/buster-backports exa/unstable

