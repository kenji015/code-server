# Code-Server Docker Compose Setup

This repository provides a simple `docker-compose.yml` configuration for [code-server](https://github.com/coder/code-server) by LinuxServer.io.  
With this setup, you can run VS Code directly in your browser without installing it locally.

## Features
- Runs as a container via Docker Compose
- Access VS Code in your browser on port `8443`
- Fully configurable via environment variables (`PASSWORD`, `TZ`, `PUID`, `PGID`)
- Persistent storage through mounted volumes

## Requirements
- Docker
- Docker Compose

## Usage
1. Clone this repository or download the `docker-compose.yml`
2. Adjust the following variables as needed:
   - `PUID` / `PGID`: User and group IDs for file permissions
   - `TZ`: Timezone
   - `PASSWORD`: Password for web access
   - Volumes: Adapt the mount paths to your system
3. Start the container:
   ```bash
   docker-compose up -d
>[!NOTE]
>Or deploy as a stack in [portainer](https://github.com/coder/code-server](https://www.portainer.io)) web-interface
