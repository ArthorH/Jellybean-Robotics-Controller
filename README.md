# ESP8266 Multipurpose robotics controller 
 made from certified jellybean components!
 
![ANGRY_JELLO](https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/7de418ee-ddb1-43e5-bd05-e77bc901d56c)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)


## Features

- Jelly Bean Components
- Universal footprints
- All usefull gpios has been broken out to connectors
- Additional I2C expander
- Battery voltage measurement
- Integrated easy to solder BMS module footprint (HW341)

## BOM
***
***
POWER SECTION
***
***
- L7805 Version (up to 500mA on all gpio-s 5v line)

| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ |------ | 
|Tantal Capacitor | 10uF 20v | Size D | 3| 
|Electrolytic Capacitor | 100uF 20v | Universal 10 - 5 mm | 1| 
|MLCC Capacitor | 100nF 20v | 0805 (2012 metric) | 6|
|L7805 IC| 5v | TO220|1|

***
- TPS56320X Version (up to 3A on all gpio-s 5v line)

| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ |------ |
|Resistor| 10k| 0603| 2
|Resistor| 54K9 1%| 0603| 1
|Inductor| 2R2| 6.6 x 7 mm SMD| 1
|If smd inductor not avaliable| 2R2| 7.5mm D THT| 1
|TPS56320X |H8v input or higher|sot6|1
|Tantal Capacitor | 10uF 20v | Size D | 3| 
|Electrolytic Capacitor | 100uF 20v | Universal 10 - 5 mm | 1| 
|MLCC Capacitor | 100nF 20v | 0805 (2012 metric) | 6|
***
***
EXPANDER IO
***
***
- SMD (PCF8754T) Version. For desoldered PCF from old broken or unused lcd backpacks.

| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ | ------ |
|Resistor| 10k| 0603| 5
|PCF8574T| n/a| SSOP20| 1
|MLCC Capacitor | 100nF 20v | 0805 (2012 metric) | 1|

***
- THT (PCF8754) Version. If lcd backpacks are not avaliable or used in other projects.

| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ | ------ |
|Resistor| 10k| 0603| 5
|PCF8574| n/a| DIL16| 1
|MLCC Capacitor | 100nF 20v | 0805 (2012 metric) | 1|
***
***
NOT GATE
***
***
 - THT version

| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ | ------ |
|Resistor| 10k| 0603| 4
|BC547| n/a| to92| 2
***
 - SMD version


| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ | ------ |
|Resistor| 10k| 0603| 4
|BC847| n/a| sot3| 2
***
***
NON OPTIONAL
***
***
- Non optional components


| Component | VALUE | PACKAGE | QTY |
| ------ | ------ |  ------ | ------ |
|Resistor| 10k| 0603| 7
|Resistor| 330R| 0603| 5
|Resistor| 100k| 0603| 6
|Capacitor| 100n| 0805| 4
|Electrolytic Capacitor | 100uF 20v | Universal 10 - 5 mm | 2| 
|TB6612FNG | Most valuable component| SSOP24| 1 (or 2)
|Random THT diode| unknown| 4007 compatible|8
|LED| random color| 5mm THT |3



## License

MIT

