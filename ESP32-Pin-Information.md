## [ESP-32 Pinout Image](https://lastminuteengineers.com/wp-content/uploads/iot/ESP32-Pinout.png)

## Which ESP32 GPIO's are safe to use?


| Pin Number    | Special Functions    | Limitations |
|     :-:       |         :-:          |       :-:   |
| 2             | On-board LED         | Must be LOW during boot |
| 4             |                      |             |
| 5             | SPI Chip Select      | Must be HIGH during boot |
| 12            |                      | Must be LOW during boot |
| 13            |                      |             |
| 14            |                      |             |
| 15            |                      | Must be HIGH during boot |
| 16            | Hardware Serial 2 RX  |             |
| 17            | Hardware Serial 2 TX  |             |
| 18            | SPI Clock            |             |
| 19            | SPI MISO             |             |
| 21            | I2C Data (SDA)       |             |
| 22            | I2C Clock (SCL)      |             |
| 23            | SPI MOSI             |             |
| 25            |                      | Baja's CAN-TX Pin |
| 26            |                      | Baja's CAN-RX Pin |
| 27            |                      |             |
| 32            |                      |             |
| 33            |                      |             |
| 34            |                      | Input only  |
| 35            |                      | Input only  |
| 36            |                      | Input only  |
| 39            |                      | Input only  |
| RX0           | Hardware Serial 0 RX  | Used for serial communication with PC/Arduino IDE |
| TX0           | Hardware Serial 0 TX  | Used for serial communication with PC/Arduino IDE |
