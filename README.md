# Sunsynk-Power-Flow-Card

An animated Home Assistant card to emulate the power flow that's shown on the Sunsynk Inverter screen. You can use this to display data from many inverters e.g. Sunsynk, Deye, Solis, Lux, FoxESS, Goodwe, Huawei etc as long as you have the required sensor data. See the [wiki](https://github.com/slipx06/sunsynk-power-flow-card/wiki) for integration methods and examples.

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=slipx06&repository=sunsynk-power-flow-card&category=plugin)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/slipx06/sunsynk-power-flow-card?style=for-the-badge) 
[![Community Forum](https://img.shields.io/badge/community-forum-brightgreen.svg?style=for-the-badge)](https://community.home-assistant.io/t/sunsynk-deye-inverter-power-flow-card/562933/1)
<a href="https://www.buymeacoffee.com/slipx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="28" width="120"></a>
## Documentation

Refer to [https://slipx06.github.io/sunsynk-power-flow-card/index.html](https://slipx06.github.io/sunsynk-power-flow-card/index.html)

## Features

* Option to switch between three card styles: `compact`, `lite` or `full`.
* Wide view for 16:9 layout.
* Animated power flow based on positive/negative/zero sensor values with configurable dynamic speed. (Supports inverted battery, AUX and grid power).
* Dynamic battery image based on SOC.
* Grid connected status.
* Configurable battery size and shutdown SOC to calculate and display remaining battery runtime based on current battery usage and system time slot setting i.e. SOC, Grid Charge. Can be toggled off.
* Daily Totals that can be toggled on or off.
* Hide all solar data if not installed or specify number of mppts in use. Set custom MPPT labels.
* "Use Timer" setting and "Energy Pattern" setting (Priority Load or Priority Battery) shown as dynamic icons, with the ability to hide if not required. If setup as switches can be toggled by clicking on the card.
* Panel mode for bigger card.
* AUX and Non-essential can be hidden from the full card or assigned configurable labels.
* Customisable - Change colours and images.
* Most entities can be clicked to show more-info dialog.
* Optional data points include self sufficiency and ratio percentages, battery temperature, AC and DC temperature.
* Display additional non-essential, essential and AUX loads.
* Display energy cost per kWh and solar sell status.
* Select your inverter model for custom inverter status and battery status messages i.e. Sunsynk, Lux, Goodwe, Solis.

## Screenshots
*Compact Version*

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/b1e437a8-d1f7-4d6a-a549-1cc908950002)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/49c499c5-9d2b-43e7-8f5d-5b9da5e07fb9)




*Lite Version*

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/d25c621c-2607-445f-b3a3-865930387a05)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/5a9078ee-7375-4f1c-affa-6fe291d62f8a)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/73d6fae3-3e6b-4891-acc2-deb29156cd2d)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/54ae290d-aa5c-428e-8a00-2a75e11c2de8)


*Full Version*

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/fdcce257-e7b5-4874-926c-17e911e83eba)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/12af5b02-c456-4685-a50f-bd0044b9e9b0)


*Wide Full Version (2 batteries)*
![image](https://github.com/user-attachments/assets/2832afb0-da0a-4924-80c5-afb9d70606fa)

*Wide Lite Version (2 batteries)*
![image](https://github.com/user-attachments/assets/59161598-1eba-4daf-8588-fdf6f047f0bf)

*Wide Compact Version (2 batteries)*
![image](https://github.com/user-attachments/assets/5cec317c-d1b7-437a-9a55-1d3c6a43f311)


## Installation

The card can be installed via HACS (recommended) or manually.

### Installation using HACS
[![hacs_badge](https://img.shields.io/badge/HACS-Default-blue.svg)](https://github.com/custom-components/hacs)


1. Install HACS.
2. Search & Install sunsynk-power-flow-card or click the button below.

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=slipx06&repository=sunsynk-power-flow-card&category=plugin)

### Manual Installation

1. Create a new directory under `www` and name it `sunsynk-power-flow-card` e.g `www/sunsynk-power-flow-card/`.
2. Copy the `sunsynk-power-flow-card.js` into the directory.
3. Add the resource to your Dashboard. You can append the filename with a `?ver=x` and increment x each time you download a new version to force a reload and avoid using a cached version. It is also a good idea to clear your browser cache.

![image](https://user-images.githubusercontent.com/7227275/235441241-93ab0c7d-341d-428f-8ca8-60ec932dde2d.png)


