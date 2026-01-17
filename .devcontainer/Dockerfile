ARG UV_VER=0.5.5
ARG DEBIAN_VER=bookworm

FROM ghcr.io/astral-sh/uv:$UV_VER AS uv
FROM mcr.microsoft.com/vscode/devcontainers/base:$DEBIAN_VER

COPY --from=uv --chown=vscode: /uv /uvx /bin/
