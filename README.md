
![Rotorflight](https://github.com/rotorflight/rotorflight/blob/master/images/rotorflight2.png?raw=true)

***

Rotorflight is a Flight Control software suite for single-rotor helicopters.

It is based on Betaflight 4.2, with many advanced features added for helicopters.
Rotorflight does **NOT** support multi-rotor crafts, nor airplanes; it is only for traditinal RC helicopters.

**WARNING!** Rotorflight is **WORK-IN-PROGRESS**. It is in beta-testing at the moment.


## Information

For latest information, please see [Rotorflight Wiki](https://github.com/rotorflight/rotorflight/wiki)


## Features

Rotorflight has many features:

* PID control tuned for helicopter use
* Rotor speed governor
* Tail Torque Assist (TTA/TALY)
* Piro compensation
* Two-stage rescue
* Fully customisable feedforward between collective/cyclic/yaw
* Advanced gyro filtering for helicopters
  - Advanced dynamic LPF
  - Dynamic RPM based notch filter banks
* Fully customisable servo/motor configuration & mixer
* Irrelevant (multi-rotor) features removed
* AND MUCH MORE

Plus lots of features inherited from Betaflight:

* Black-box logging
* Configuration profiles for changing various tuning parameters
* Multi-color RGB LEDs
* Configurable buzzer sounds
* Multiple ESC protocols: DShot (150,300,600), Multishot, Oneshot, and traditional PWM
* Multiple ESC telemetry protocols: KISS, HW
* Multiple RX telemetry protocols: CSRF, FrSky, HoTT, MSP, etc.
* Voltage inputs for RSSI, battery voltage, current sensors, etc.
* Fully integrated OSD
* Fully integrated video TX control (Unify Pro, IRC Tramp, etc.)


## Hardware support

Generally speaking, Rotorflight supports all flight controller hardware that is supported by Betaflight.
With a caveat that the flight controller must have enough suitable I/O pins for connecting all the servos
and motors required by a collective pitch helicopter.

Also, the FC boards are typically labeled for multi-rotor use - thus the user needs to understand how these
functions can be used for a different purpose with helicopters. Usually this is just about using some
of the motor outputs for servos, but in some cases a more advanced remapping may be needed.

It is highly recommended to use a STM32F7 based flight controller, as Rotorflight greatly benefits from
the latest filtering algorithms and other new features that are all CPU intensive.

An absolute minimum is a STM32F4 based board, but it probably won't be able to run all the new features.


## Installation

Please see the [Wiki](https://github.com/rotorflight/rotorflight/wiki) for instructions.

For downloading the latest versions, go to the "Releases" page on each GitHub repo:
* [Firmware Releases](https://github.com/rotorflight/rotorflight-firmware/releases)
* [Configurator Releases](https://github.com/rotorflight/rotorflight-configurator/releases)
* [Blackbox Releases](https://github.com/rotorflight/rotorflight-blackbox/releases)


## Contributing

Contributions are welcome and encouraged. You can contribute in many ways:

* Testing Rotorflight with different types of helicopters
* Documentation updates and corrections
* Writing How-To guides
* Bug reports
* New ideas & suggestions
* Provide a new translation for configurator
* Implement a new feature or a fix in the firmware

Please see [Wiki](https://github.com/rotorflight/rotorflight/wiki/Contributing) for details.


## Open Source / Contributors

Rotorflight is software that is **open source** and is available free of charge without warranty to all users.

Rotorflight is forked from Betaflight, which in turn is forked from Cleanflight.
Rotorflight also borrows ideas and code from Heliflight-3D, another Betaflight fork for helis.

So thanks goes to all those whom have contributed along the way.

Origins for Rotorflight:
* **Dr.Rudder** - author, maintainer
* **pkaig** - wiki, beta-testing
* **egon** - wiki, beta-testing
* **mopatop** - wiki, beta-testing

Origins for Heliflight-3D:
* **James-T1** (author)
* **Dr.Rudder**
* **Westie**

Origins for Betaflight (Thanks!):
* **Alexinparis** (for MultiWii),
* **timecop** (for Baseflight),
* **Dominic Clifton** (for Cleanflight),
* **borisbstyle** (for Betaflight), and
* **Sambas** (for the original STM32F4 port).

The Betaflight Configurator is forked from Cleanflight Configurator and its origins.

Origins for Betaflight Configurator:
* **Dominic Clifton** (for Cleanflight configurator), and
* **ctn** (for the original Configurator).

Big thanks to current and past contributors:
* Budden, Martin (martinbudden)
* Bardwell, Joshua (joshuabardwell)
* Blackman, Jason (blckmn)
* ctzsnooze
* Höglund, Anders (andershoglund)
* Ledvina, Petr (ledvinap) - **IO code awesomeness!**
* kc10kevin
* Keeble, Gary (MadmanK)
* Keller, Michael (mikeller) - **Configurator brilliance**
* Kravcov, Albert (skaman82) - **Configurator brilliance**
* MJ666
* Nathan (nathantsoi)
* ravnav
* sambas - **bringing us the F4**
* savaga
* Stålheim, Anton (KiteAnton)

And many many others who haven't been mentioned....
