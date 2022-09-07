# Onboard Layouts
This repository contains custom layouts for the [OnBoard](https://launchpad.net/onboard) on-screen-keyboard. The layout may be useful to set up a kiosk with no mouse and keyboard and only touchscreen.

## Getting Started
Self reminder guide to ease up setup, especially on Raspberry Pi OS where some components are required.

### Installing onboard
Installing onboard on debian-based system is as easy as
```sh
sudo apt install onboard
```

### Rasbperry Pi OS Specifics
On Raspberry Pi OS Bullsye, auto-open automatically does not work. This is possibly because the Pi OS runs LXDE desktop environment as opposed to GNOME.
Some packages those are required to run OnBoard optimally is missing on Raspberry Pi OS.

Install following packages to allow OnBoard to open automatically when any text entry is focused.
- at-spi2-core
- gir1.2-appindicator3-0.1
- gir1.2-atspi-2.0
- onboard-data
- mousetweaks

Or one liner:
```sh
sudo apt install at-spi2-core gir1.2-appindicator3-0.1 gir1.2-atspi-2.0 onboard-data mousetweaks
```



## Getting Layouts from this Repository
Simply clone this repository to user OnBoard folder.

```sh
git clone https://github.com/seikosantana/onboard-layouts ~/.local/share/onboard/layouts
```