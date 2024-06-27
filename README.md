# ESP8266 Multipurpose robotics controller 
 made from certified jellybean components!
 
![ANGRY_JELLO](https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/7de418ee-ddb1-43e5-bd05-e77bc901d56c)



![Boards in different configuration](https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/a95e0b77-833b-45b5-ba12-bc03fe4b9c9f)

## Features
- Jelly Bean Components
- Universal footprints
- All usefull gpios has been broken out to connectors
- Additional I2C expander
- Battery voltage measurement
- Integrated easy to solder BMS module footprint (HW341)

## Jelly Bean components 
Board designed to allow manufacture of simple but capable wifi enabled robotics controller from most common avaliable components.
<img src="https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/870d1798-7d06-496b-857a-838cff4b0baf" alt="drawing" class="center" width="600"/>
## Universal footprints
Board is designed to handle multiple packages of same components:
<img src="https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/e16e0b2b-58ce-4670-914a-09cb1b465ec5" alt="drawing" class="center" width="600"/>

Also some components that are scarse or just rare to have in immediate reach are made bypassable by common ones:

<img src="https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/30bb8dbb-6476-472a-85b1-8336f08cd703" alt="drawing" class="center" width="600"/>

## Integrated BMS controller 
Integrated easy to solder BMS module footprint (HW341)

<img src="https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/ed76d0cf-df7e-45dd-ad3e-9812ceb95d15" alt="drawing" class="center" width="600"/>

## !Warning! Due to me forgetting to add on/off switch after BMS it needs to be bodged in order to work:

<img src="https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/c6ee41a9-91cb-4c0b-abe2-fa80d1e70d5e" alt="drawing" class="center" width="600"/>

# BOM

## POWER SECTION

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

## EXPANDER IO

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

## NOT GATE

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

## NON OPTIONAL

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

## PCB mounted on simple moving robot
![IMG_0362](https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/4bbba17c-744e-43c4-b807-a25a3b7f5d0e)
![IMG_0365](https://github.com/ArthorH/ESP8266_JELLYBEAN_CONTROLLER/assets/101933781/fa5a6c7f-f3f3-4ea1-a3cd-ba3d0b119b93)

## License

MIT

