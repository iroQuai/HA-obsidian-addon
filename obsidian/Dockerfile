# ==============================
# Home Assistant Obsidian Add-on
# ==============================

# Base image (LinuxServer Obsidian)
ARG BUILD_FROM=lscr.io/linuxserver/obsidian:latest
FROM ${BUILD_FROM}

# Set maintainer label
LABEL maintainer="ha.addons@stijnbiemans.nl"
LABEL org.opencontainers.image.title="Home Assistant Add-on: Example"
LABEL org.opencontainers.image.description="Web-based Obsidian Markdown editor integrated into Home Assistant"
LABEL org.opencontainers.image.source="https://github.com/iroQuai/HA-obsidian-addon/tree/main/example"

# Install Bashio library for HA add-ons
RUN apk add --no-cache bash curl \
    && curl -sL https://raw.githubusercontent.com/home-assistant/addons/develop/bashio/bashio.sh -o /usr/bin/bashio.sh \
    && chmod +x /usr/bin/bashio.sh

# Copy service scripts
COPY rootfs/ /

# Set working directory
WORKDIR /config

# Expose the internal container port
EXPOSE 3000

# Set default command (s6 will handle execution)
CMD ["/init"]
