ARG ENV_SOURCE_IMAGE
ARG PHP_VERSION
FROM ${ENV_SOURCE_IMAGE}:${PHP_VERSION}
USER root

RUN dnf install tmux nvim

RUN mv ~/.config/nvim ~/.config/nvim.bak && \
    mv ~/.local/share/nvim ~/.local/share/nvim.bak && \
    mv ~/.local/state/nvim ~/.local/state/nvim.bak && \
    mv ~/.cache/nvim ~/.cache/nvim.bak

RUN git clone --depth 1 https://github.com/AstroNvim/AstroNvim ~/.config/nvim

USER www-data
