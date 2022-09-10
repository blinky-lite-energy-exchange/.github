# The Blinky-Lite Energy Exchange
## Table of Contents
* [Blinky PrisSensor](#blinky-prissensor)
* [Blinky Eon Mon](#blinky-eon-mon)
* [Blinky Relay](#blinky-relay)
* [Blinky Rheostat](#blinky-rheostat)
* [Blinky Heat Pump](#blinky-heat-pump)
* [Code Repositories](#code-repositories)


## A Shock
* Currently, electricity prices have risen dramatically across Europe
* At these rates, people on fixed incomes and small business are at dire financial risk
* Sweden offers spot pricing for electricity
  - Could dramatically reduce costs by shifting usage to off peak hours
  - However, following spot prices requires constant vigilance
    * Monitoring spot price manually is exhausting and error prone
    * To be effective spot pricing monitoring <ins>must be automatic.</ins>
* There are a number of companies offering automated monitoring
  - Most of these services <ins>**require the user to purchase expensive new equipment**</ins> (such as heating systems) that can be connected to the internet.
* Throwing out old systems that are still functioning is <ins>***UNSUSTAINABLE!***</ins>
  - And financially not possible for fixed income families
  - And small businesses

## A Sustainable Open Source Approach
* We have harnessed Blinky-Lite to provide low cost retrofits <ins>to existing equipment</ins> using ***Edge computing***
* We have built a number of devices that easily interface with the scalable Blinky-Lite system that operate with three different modes
  - Manual control
  - Schedule control
  - Spot Price sensitive control

## Blinky PrisSensor
[(contents)](#table-of-contents)<br>
* A virtual device with an open API that can be used by any system to monitor the spot price
* It comes with a non-native web app so it can be monitored on any device with no installation.
  - Mobile and Desktop Web App
    * [DK1 Price Area](https://www.blinky-lite.se/espotPrice?name=DK1)
    * [DK2 Price Area](https://www.blinky-lite.se/espotPrice?name=DK2)
    * [NO2 Price Area](https://www.blinky-lite.se/espotPrice?name=NO2)
    * [SE3 Price Area](https://www.blinky-lite.se/espotPrice?name=SE3)
    * [SE4 Price Area](https://www.blinky-lite.se/espotPrice?name=SE4)
  - [Smart Watch Web App](https://www.blinky-lite.se/esps) (not Apple) 

<img src="https://github.com/blinky-lite-energy-exchange/.github/raw/master/profile/blinkyPrice.png"/><br>

## Blinky Eon Mon
[(contents)](#table-of-contents)<br>
A P1-HAN compatible electricity monitor with intuitive displays
* Secure, reliable, high rate Bluetooth connection to any network network.
* It comes with a non-native web app so it can be monitored on any device with no installation.

<img src="https://github.com/blinky-lite-energy-exchange/.github/raw/master/profile/blinkyEonMon.png"/><br>

## Blinky Relay
[(contents)](#table-of-contents)<br>
Many old heating systems have no way to remotely turn them on and off so it is not possible to interface a spot price device directly to an old heating system. Replacing the entire heating system just because the heating system is manually controlled  but is otherwise functioning perfectly would be very wasteful. 

It is not advised to power control a heating system by just turning it on and off with an electrical switch (relay). Instead an electrical switch (relay) can be used to control the  small pump that is used to pump hot water though the radiators.

With Blinky Power Relay, a an electrical relay is placed in series with the power to the radiator water pump. The relay is directly controlled with [Blinky Power Relay cube](https://github.com/blinky-lite-energy-exchange/blinky-power-relay-cube). The Blinky Power Relay cube can be remotely controlled via a Blinky Power Relay tray which has access to the electric spot price and can talk and be controlled with an web app on the Blinky-Lite application box.

<img src="https://github.com/blinky-lite-energy-exchange/.github/raw/master/profile/blinkyRelay.png"/><br>

## Blinky Rheostat
[(contents)](#table-of-contents)<br>
Many old heating systems use manual dials to control the temperature or the flow so it is not possible to interface a spot price device directly to an old heating system. Replacing the entire heating system just because the heating system is manually controlled would be very wasteful . Even just replacing the heating elements could cause damage to the old heating system. 

With Blinky-Rheostat, a small stepper motor is placed on the knob stem. This stepper motor is directly controlled with [Blinky Rheostat Cube](https://github.com/blinky-lite-energy-exchange/blinky-rheostat-cube). The Blinky Rheostat cube can be remotely controlled via a Blinky-Rheostat tray which has access to the electric spot price and can talk and be controlled with an web app on the Blinky-Lite application box. 

Source code at [Blinky Rheostat Tray](https://github.com/blinky-lite-energy-exchange/blinky-rheostat-tray)

<img src="https://github.com/blinky-lite-energy-exchange/.github/raw/master/profile/blinkyRheostat.png"/><br>

## Blinky Heat Pump
[(contents)](#table-of-contents)<br>
Just like many heat pumps, the IVT Heat pump web interface API is closed so it is not possible to interface a spot price device directly to this heat pump. In additon many older but perfectly functioning heat pumps do not even have an internet interface. Replacing the  heat pump just because the heat pump cannot connect to the internet would be very wasteful.

However, as with most heat pumps, this heat pump is controlled with a infra-red remote control. As a workaround, the an infra-red remote control can be substituted with an [Blinky IVT Cube](https://github.com/blinky-lite-energy-exchange/blinky-ivt-cube) that is equipped with a an infra-red diode that can send the appropriate pulse sequence to the heat pump. A list of different pulse sequences can be found at [ToniA/arduino-heatpumpir](https://github.com/ToniA/arduino-heatpumpir). The [ToniA/arduino-heatpumpir](https://github.com/ToniA/arduino-heatpumpir) project contains pulse sequences for 29 different models of heat pumps so it possible to easily extend the Blinky IVT Cube to many different models of heat pumps. The Blinky IVT cube can be remotely controlled via a Blinky-IVT tray which has access to the electric spot price and can talk and be controlled with an web app on the Blinky-Lite application box.

Source code at [Blinky IVT Tray](https://github.com/blinky-lite-energy-exchange/blinky-ivt-tray)

<img src="https://github.com/blinky-lite-energy-exchange/.github/raw/master/profile/blinkyIvt.png"/><br>

# Code Repositories
[(contents)](#table-of-contents)<br>
