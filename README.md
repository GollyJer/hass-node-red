# Node-RED Companion Integration

[![hacs][hacsbadge]][hacs] [![releasebadge]][release] ![buildbadge] [![License][license-shield]](LICENSE.md)

[![BuyMeCoffee][buymecoffeebadge]][buymecoffee]

_Companion Component to [node-red-contrib-home-assistant-websocket](https://github.com/zachowj/node-red-contrib-home-assistant-websocket) to integrate Node-RED with Home Assistant._

## Features
* Create and update binary sensors, buttons, sensors, and switches from Node-RED
* Disable and enable Node-RED flows from Home Assistant UI
* Create Home Assistant webhooks and handle them in Node-RED
* Use Device triggers and action from Node-RED

## Minimum Requirements

* [node-red-contrib-home-assistant-websocket](https://github.com/zachowj/node-red-contrib-home-assistant-websocket) v0.20+
* [Home Assistant](https://github.com/home-assistant/core) 2021.12.0

## Installation

1. Install via [HACS](https://hacs.xyz) (Home Assistant Community Store) or manually.

    HACS
    - Go to HACS -> Integrations -> "+ Explore & Download Repos"
    - Find "Node-RED Companion".
    - Open the search result and click "Download this Repository with HACS".

    Manual Steps
    
    - Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
    - If you do not have a `custom_components` directory (folder) there, you need to create it.
    - In the `custom_components` directory (folder) create a new folder called `nodered`.
    - Download _all_ the files from the `custom_components/nodered/` directory (folder) in this repository.
    - Place the files you downloaded in the new directory (folder) you created.
    - Restart Home Assistant
    - Refresh your browser window (bug in HA where it doesn't update the integration list after a reboot)


    Using your HA configuration directory (folder) as a starting point you should have this:

    ```text
    custom_components/nodered/translations/en.json
    custom_components/nodered/__init__.py
    custom_components/nodered/binary_sensor.py
    custom_components/nodered/config_flow.py
    custom_components/nodered/const.py
    custom_components/nodered/discovery.py
    custom_components/nodered/manifest.json
    custom_components/nodered/sensor.py
    custom_components/nodered/services.yaml
    custom_components/nodered/switch.py
    custom_components/nodered/websocket.py
    ```

2. In the HA UI go to "Configuration" -> "Devices & Services" -> "+ Add Integration" and search for "Node-RED Companion"



## Configuration

Once installed and added via Integrations all configuration is done from Node-RED.

## Contributions are welcome!

If you want to contribute to this please read the [Contribution guidelines](CONTRIBUTING.md)

***

[buymecoffee]: https://www.buymeacoffee.com/zachowj
[buymecoffeebadge]: https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png
[license-shield]: https://img.shields.io/github/license/zachowj/hass-node-red.svg?style=for-the-badge
[hacs]: https://github.com/zachowj/hass-node-red
[hacsbadge]: https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge
[release]: https://github.com/zachowj/hass-node-red/releases
[releasebadge]: https://img.shields.io/github/v/release/zachowj/hass-node-red?style=for-the-badge
[buildbadge]: https://img.shields.io/github/workflow/status/zachowj/hass-node-red/pre-commit?style=for-the-badge
