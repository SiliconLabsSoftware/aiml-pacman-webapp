# Pac-Man

> **_NOTE:_**
> Unless otherwise specified in the specific directory, all examples are considered to be **EXPERIMENTAL QUALITY**, which implies that the code provided in this repository has not been formally tested and is provided as-is. It is not suitable for production environments. In addition, this code will not be maintained and there may be no bug maintenance planned for these resources. Silicon Labs may update projects from time to time.

Pac-Man game written in HTML5 + CSS3 + jQuery with Canvas. This WebApp is a Responsive Web Design (RWD) website.

Open `index.html` in a Chromium-based browser (Chrome or Edge) to play locally
with a BRD2601 board. Connect to `BLE_AIML_KWS`. The firmware does not depend
on this page; it can run on its own (VCOM / LEDs). BLE notifications can also
drive this demo.

Keywords: left, right, up, down, stop, go.

The webpage uses the [p5.ble.js](https://itpnyu.github.io/p5ble-website/) library for communicating with the development board via Bluetooth Low Energy.

The webpage uses "vanilla" javascript+css+html. No special build systems required.
Simply double-click the `index.html` to view the webpage locally.

## Firmware

A BRD2601 image is in this repo:

`firmware/brd2601b/aiml_ble_soc_audio_classifier_efr32_micriumos.s37`

Flash it with Simplicity Commander. To rebuild or modify the firmware, use the
AI/ML SDK sample `aiml_ble_soc_audio_classifier_efr32_micriumos` for `brd2601b`.
The firmware works with this web page over BLE and can run without it (VCOM / LEDs).

## Changes

This was adapted from a game created by Lucio Panpinto.
View original source code on [GitHub](https://github.com/luciopanepinto/pacman).

The following changes were made to the source code:

- Removed google analytics
- Removed www.putchu.be links
- Added Silicon Lab's branding
- Added Bluetooth Low Energy support

## License

This repository uses multiple licenses. See [LICENSE](LICENSE) for the full
terms.

- **Pac-Man web application** (`index.html`, `css/`, `img/`, `sound/`, and
  Silicon Labs-modified game JavaScript under `js/`):
  [GNU General Public License v3.0](LICENSE)
- **Third-party JavaScript** under `js/` (for example jQuery components):
  original licenses in the file headers (MIT)
- **Prebuilt firmware** under `firmware/`: Silicon Laboratories
  [Master Software License Agreement (MSLA)](https://www.silabs.com/about-us/legal/master-software-license-agreement);
  see [firmware/LICENSE](firmware/LICENSE)

The firmware is independent of this web page. Build or obtain firmware from
the AI/ML SDK sample `aiml_ble_soc_audio_classifier_efr32_micriumos` under the
SDK license terms.
