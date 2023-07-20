# ISM01A - Si4463 EZRadioPRO Transceiver

The MLAB ISM01A module is a high-performance wireless transceiver designed for long-distance data transmission. The module is based on the [Si4463 chip](https://www.silabs.com/wireless/proprietary/ezradiopro-sub-ghz-ics/device.si4463?tab=specs) from Silicon Labs, which is part of the EZRadioPRO family. With its wide frequency range and output power, it is ideal for applications that require robust and reliable wireless communication. 

ISM01A can operate on the open 433 or 868 MHz frequencies, which are popular in many applications.

![Top view on ISM01A](doc/img/ISM01A_top_big.png)


## Parameters

- Based on the Si4463 chip
- Chip frequency range: 142 to 1050 MHz, with the ability to operate on the open 433 or 868 MHz frequencies
- Chip output power: -20 to 20 dBm
- The Si4463 chip includes a programmable block capable of controlling radio settings and supports the SPI interface
- Power supply: 5-12V with integrated 3.3V stabilizer
- Communication: UART, SPI, GPIO
- Accessible GPIO signals directly from the transceiver
- Status indication: Two LED diodes controlled from the Si chip
- Antenna connectors: MCX for RX and TX antennas. For bidirectional communication with a single antenna, it is necessary to connect the [RFSWITCH module](www.mlab.cz/module/RFSWITCH01/), which serves as an RF switch and enables MIMO 2x2 support. ISM01A is able to control RFSWITCH module trought GPIO pins

## Possible Applications

The MLAB ISM01A module with the Si4463 transceiver is suitable for a wide range of applications. It can be used in areas such as:

- **Remote Control**: The module can be used for wireless control of various devices, such as drones, RC cars, or home automation.
- **Data Links**: With prepared firmware, the module can function as a [SiK data communication link](https://ardupilot.org/copter/docs/common-sik-telemetry-radio.html), which can transmit [MAVLink packets](https://mavlink.io/en/). MAVLink is a protocol designed for communication with unmanned vehicles and is supported by the most widespread autopilots Ardupilot and PX4. This is ideal for applications that require wireless data transmission.
- **Wireless Sensor Networks**: The module can be used to create wireless sensor networks in IoT applications.

> Based on this module, the company [ThunderFly](https://www.thunderfly.cz) has developed a module optimized for use on drones, which combines this ISM01A module, RFSWITCH01A and aditional RF filters and LNA. More information about this TFSIK01 module can be found [here](https://github.com/ThunderFly-aerospace/TFSIK01/).

## Links to Related Resources

- [Silicon Labs Si4463 Product Page](https://www.silabs.com/wireless/proprietary/ezradiopro-sub-ghz-ics/device.si4463?tab=specs)
- [Si4463 Datasheet](https://www.silabs.com/documents/public/data-sheets/Si4464-63-61-60.pdf)
- [MavLink Protocol](https://mavlink.io/en/)
- [SiK Radio](https://ardupilot.org/copter/docs/common-sik-telemetry-radio.html)
- [EZRADioPRO Family](https://www.silabs.com/wireless/proprietary/ezradiopro-sub-ghz-ics)
- [TFSIK01 Module by ThunderFly](https://github.com/ThunderFly-aerospace/TFSIK01/)
