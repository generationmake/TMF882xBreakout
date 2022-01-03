# TMF882xBreakout
Breakout board for the ams TMF8820, TMF8821 and TMF8828 multi-zone time-of-flight sensors

![TMF882xBreakout rendering](docs/images/TMF882xBreakout_rendering.png)

## Pinout

### CN1 and CN2

This is a regular 0.1-inch pin header.

| pin number | signal on CN1 | signal on CN2|
|:----------:|:-------------:|:------------:|
| 1          | VCC           | VCC          |
| 2          | GND           | GND          |
| 3          | I2C_SDA       | I2C_SDA      |
| 4          | I2C_SCL       | I2C_SCL      |
| 5          | INT           | INT          |
| 6          | ENABLE        | GPIO0        |
| 7          | not available | GPIO1        |

Several TMF882xBreakout boards can be used by connecting CN1 to CN2 of the previous board. GPIO0 is used to enabled the following TMF882x and thus giving the possibility to change the I2C address of each device one after another.

### CN3 and CN4

This is Arduino ESLOV connector. JST SH 1mm 5-pin.

| pin number | signal on CN3 | signal on CN4|
|:----------:|:-------------:|:------------:|
| 1          | VCC           | VCC          |
| 2          | GND           | GND          |
| 3          | I2C_SDA       | I2C_SDA      |
| 4          | I2C_SCL       | I2C_SCL      |
| 5          | ENABLE        | GPIO0        |

Several TMF882xBreakout boards can be used by connecting CN3 to CN4 of the previous board. GPIO0 is used to enabled the following TMF882x and thus giving the possibility to change the I2C address of each device one after another.

This connector does not allow the use of interrupts.

## PCB

### Top

![TMF882xBreakout PCB top](docs/images/TMF882xBreakout_top.png)

### Bottom

![TMF882xBreakout PCB bot](docs/images/TMF882xBreakout_bot.png)

## Resources

### Datasheets

 * https://ams.com/documents/20143/6015057/TMF882X_DS000693_4-00.pdf

### Arduino Libraries

* [107-Arduino-TMF8801](https://github.com/107-systems/107-Arduino-TMF8801)
