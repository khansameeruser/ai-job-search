FROM mcr.microsoft.com/devcontainers/javascript-node:22-bookworm

USER root

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        poppler-utils \
        python3 \
        texlive-fonts-extra \
        texlive-fonts-recommended \
        texlive-latex-extra \
        texlive-luatex \
        texlive-xetex \
    && rm -rf /var/lib/apt/lists/*

RUN npm install --global --no-audit --no-fund @openai/codex@0.167.0 bun@1.4.4
