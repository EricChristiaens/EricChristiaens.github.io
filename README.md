# MGR PROJECT

This is the repository of the MGR project

**MGR** is an application running on ESP32 and designed to control a modelrailroad network.

> [!CAUTION]
> MGR is still under development and cannot be considered as stable


## Main features

MGR offers the following features to manage a modelrailroad network:
- Communications with SAT devices (satellites) over CAN bus 
- Management of control pannels over WiFi webSockets, based on a JSON configuration file
- Management, based on JSON configuration file, of following types of modelrailway devices:
  - Signal (and its corresponding LEDs)
  - Point (and its corresponding servo motors)
  - Block (and its presence detectors)
  - Switch 
  
- Management, based on JSON configuration file, of rules in order to:
  - Allow the switch of a Point
  - Allow the set of a Signal to Green
  - Decide when a signal must be set to Red, Orange or Green

## Architecture

> [!WARNING]
> To be completed.

## Hardware

> [!WARNING]
> To be completed.

 
## Limitations

In its current version, MGR has some limitations:
- No interaction with DCC or Loconet.
- A theoretical maximum of **128** SAT devices can be managed. Exact limitation in terms of performance is to be confirmed.
- A SAT devices can be connected to a maximum of **11** components (Servo motors, LEDs, switches, detectors)
- All LEDs of a Signal must be located on the same SAT device
- All servo motors of a Point must be connected on the same SAT device
- Only a limitted number of types of signals can be managed (mainly German signals)
