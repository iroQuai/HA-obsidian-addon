# Home Assistant Add-on: Obsidian

## How to use

This add-on provides a web-based **Obsidian Markdown editor** integrated into Home Assistant. 

### Starting the add-on
- Start the add-on from the Home Assistant Supervisor.
- The service will run in the background using the [LinuxServer.io Obsidian Docker image](https://hub.docker.com/r/linuxserver/obsidian) as its base.

### Configuration
- Options can be set via the Home Assistant add-on configuration UI.
- Data and configuration are stored in:
  - `/addon_config/obsidian` — for add-on configuration files
  - `/data/obsidian` — for your Obsidian vault files

### Logs
- The add-on logs messages to the Supervisor log.




