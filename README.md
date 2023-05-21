# UDM-Better-Fan-Speeds

## Repository Deprecation Notice

**:warning: Repository Deprecation Notice: This project is now deprecated and archived due to the release of UniFi's firmware v2.x and v3.x for Dream Machnines, which natively fix the fan speed issues.**

This repository only works with **firmware 1.x. UDM-PRO** Please consider upgrading your firmware for improved functionality.

## What It Does

It stops the build in service that monitors the thermal values, fan speed and connection of a HDD/SSD. After that it sets the thermal/fan chip (adt7475) to automatic mode. Once that is done it changes the thermal and fan threshold values specified in the script. If you like, you can change the values to your own preferences.

## Compatibility

- Tested on [UDM PRO][amz-udm-pro-url]

## WARNING

USE THIS ON YOUR OWN RISK.
If you apply inappropriate settings with this script, you will possibly (soft- or hard-) brick your equipment.

## Requirements

Persistence on Reboot is required.  
This can be accomplished with a boot script. Flow this guide: [UDM Boot Script](https://github.com/unifi-utilities/unifios-utilities/tree/main/on-boot-script)

## Installation

```shell
curl -s https://raw.githubusercontent.com/fire1ce/UDM-Better-Fan-Speeds/main/install.sh | sh
```

## Configuration

You can edit the fan-speed settings at

```shell
/mnt/data/on_boot.d/11-udm-better-fan-speed.sh
```

## Credit

Based on [renedis/ubnt-auto-fan-speed][renedis-ubnt-auto-fan-speed-github-url] by [ReneDIS][renedis-github-url]. Thanks

<!-- --- -->

[renedis-ubnt-auto-fan-speed-github-url]: https://github.com/renedis/ubnt-auto-fan-speed 'ubnt-auto-fan-speed renedis github'
[renedis-github-url]: https://github.com/renedis 'ReneDIS github'
[amz-udm-pro-url]: https://amzn.to/3J4fezk 'Amazon Unifi UDM Pro'

<!-- --- -->
