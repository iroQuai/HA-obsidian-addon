# Obsidian Home Assistant add-on repository

This repository contains a Home Assistant add-on for the **Obsidian Markdown editor**.

Add-on documentation: <https://developers.home-assistant.io/docs/add-ons>

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2F<your-username>%2FHA-obsidian-addon)

## Add-ons

This repository contains the following add-on:

### [Obsidian add-on](./obsidian)

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armv7 Architecture][armv7-shield]

_Obsidian add-on to run a web-based Markdown editor integrated into Home Assistant._

<!--
Notes to developers after forking or using this repository:

- While developing, comment out the 'image' key from 'obsidian/config.yaml' to make the supervisor build the addon.
  - Remember to put this back when pushing up your changes.
- When merging to the 'main' branch of your repository a new build will be triggered.
  - Update the 'version' key in 'obsidian/config.yaml'.
  - Update 'obsidian/CHANGELOG.md'.
  - Ensure GitHub Container Registry settings allow public access if needed.
- Adjust the 'image' key in 'obsidian/config.yaml' to point to your GitHub username.
- The 'slug' key in 'obsidian/config.yaml' should match the directory name.
- Adjust any URLs pointing to 'home-assistant' to point to your fork.
- Share your repository on the forums: https://community.home-assistant.io/c/projects/9
- Have fun building awesome stuff!
-->

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
