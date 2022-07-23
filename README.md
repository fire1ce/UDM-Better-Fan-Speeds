# UDM-Better-Fan-Speeds

## What it does

It stops the build in service that monitors the thermal values, fan speed and connection of a HDD/SSD. After that it sets the thermal/fan chip (adt7475) to automatic mode. Once that is done it changes the thermal and fan threshold values specified in the script. If you like, you can change the values to your own preferences.

## Compatibility

- Tested on UDM PRO

## WARNING

USE THIS ON YOUR OWN RISK.
If you apply inappropriate settings with this script, you will possibly (soft- or hard-) brick your equipment.

## Requirements

Persistence on Reboot is required.  
This can be accomplished with a boot script. Flow this guide: [UDM / UDMPro Boot Script](https://github.com/unifi-utilities/unifios-utilities/tree/main/on-boot-script)

## Installation

```shell

```

## Installation

- Copy [`on_boot.d/11-ubnt-auto-fan-speed.sh`](https://github.com/renedis/ubnt-auto-fan-speed/raw/main/on_boot.d/11-ubnt-auto-fan-speed.sh) to your UDM (Pro) in `/mnt/data/on_boot.d`
- `chmod +x /mnt/data/on_boot.d/11-ubnt-auto-fan-speed.sh`
- Adjust the settings if you want (or use mine)
- Run the script: `sh /mnt/data/on_boot.d/11-ubnt-auto-fan-speed.sh`

It will survive a reboot thanks to @boostchicken 's bootscript. The OLED screen does show correct percentage and RPM. But it does not respond to changes anymore (the "slide" trick).

## Credit

Based on [renedis/ubnt-auto-fan-speed][renedis-ubnt-auto-fan-speed-github-url] by [ReneDIS][renedis-github-url]. Thanks

<!-- --- -->

[renedis-ubnt-auto-fan-speed-github-url]: https://github.com/renedis/ubnt-auto-fan-speed 'ubnt-auto-fan-speed renedis github'
[renedis-github-url]: https://github.com/renedis 'ReneDIS github'

<!-- --- -->
