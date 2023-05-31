# Edu-CIAA bluetooth driver

Bluetooth driver for a Panasonic's PAN1323ETU module on a EDU-CIAA board (NXP LPC4337)

## About this project

This is part of the 

## PAN1323ETU used pinout

| Connector | Pin |            Name | I/O |                 Description |
|----------:|----:|----------------:|----:|----------------------------:|
|        J1 | 1   | GND             |     | Connect to Ground           |
|        J1 | 3   | BT_HCI_CTS_3V3  |   I | HCI UART clear-to-send      |
|        J1 | 5   | SLOW_CLK_3V3    |   I | HCI                         |
|        J1 | 7   | BT_HCI_RX_3V3   |   I | HCI UART data receive       |
|        J1 | 9   | BT_HCI_TX_3V3   |   O | HCI UART data transmit      |
|        J2 | 2   | GND             |   I |                             |
|        J2 | 7   | +3V3            |   I |                             |
|        J2 | 9   | +3V3            |   I |                             |
|        J2 | 18  | BT_HCI_RTS_3V3  |   O | HCI UART request-to-send    |
|        J2 | 19  | BT_NSHUTD_3V3   |   I | Shutdown input (active low) |

### Relevant info

SLOW_CLK_3V3 can be a digital signal in the range of 0-1.8 V.
The slow clock's frequency accuracy must be 32.768 kHz +-250 ppm for Bluetooth
usage (according to the Bluetooth specification).
