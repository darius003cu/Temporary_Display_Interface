# Temporary Interface for the FT813 Display

## Display interface
This module implements a display driver for the FT813 screen, interfaced with the NXP S32K144 microcontroller via SPI. It is designed for EVR Tuiasi's formula-style race car dashboard, displaying critical vehicle parameters in real time

### Hardware
- **MCU**: NXP S32K144
- **Display**: NHD-7.0-800480FT-CSXP-CTP
- **Communication**: LPSPI0

### Features
- Full-color TFT LCD rendering driven by the S32K144 LPSPI peripheral.
- Intuitive graphical UI designed for at-a-glance readability at racing speeds.
- Manual lap timing via steering wheel button (testing use only).

### Displayed Parameters
| Parameter                 | Description                          |
|---------------------------|--------------------------------------|
| Speedometer               | Real-time vehicle speed              |
| Brake & Acceleration      | Driver input monitoring              |
| Battery Percentage        | State of charge                      |
| Total Current & Voltage   | Overall pack electrical readings     |
| Highest BMS Cell Voltage  | Per-cell peak voltage monitoring     |
| Highest BMS Cell Temp     | Per-cell peak temperature monitoring |
| Inverter & Motor Temp     | Drivetrain thermal monitoring        |
| Warning Lights            | Visual alerts for out-of-range values|
| Critical Errors           | Fault indicators requiring attention |
