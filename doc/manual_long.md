| /do/2b3l/allBlink   |                                                           |
|:--------------------|:----------------------------------------------------------|
| Info                | [beta] [gpio] [led] [electronics]                         |
| Description         | Blink all leds                                            |
| Usage               | /do/2b3l/allBlink                                         |
| Modules             | /do/led/blink 21 &, /do/led/blink 20 &, /do/led/blink 16, |

| /do/2b3l/allOff   |                                                 |
|:------------------|:------------------------------------------------|
| Info              | [beta] [gpio] [led] [electronics]               |
| Description       | Turn off all leds                               |
| Usage             | /do/2b3l/allOff                                 |
| Modules           | /do/led/off 21, /do/led/off 20, /do/led/off 16, |

| /do/2b3l/allOn   |                                              |
|:-----------------|:---------------------------------------------|
| Info             | [beta] [gpio] [led] [electronics]            |
| Description      | Turn on all leds                             |
| Usage            | /do/2b3l/allOn                               |
| Modules          | /do/led/on 21, /do/led/on 20, /do/led/on 16, |

| /do/2b3l/allPulse   |                                                           |
|:--------------------|:----------------------------------------------------------|
| Info                | [beta] [gpio] [led] [electronics] [pwm]                   |
| Description         | Turn on/off all leds slowly                               |
| Usage               | /do/2b3l/allPulse                                         |
| Modules             | /do/led/pulse 21 &, /do/led/pulse 20 &, /do/led/pulse 16, |

| /do/2b3l/button1State   |                                                 |
|:------------------------|:------------------------------------------------|
| Info                    | [beta] [gpio] [buttons] [electronics] [pull-up] |
| Description             | Check state of button on pin 26                 |
| Usage                   | /do/2b3l/button1State                           |
| Modules                 | /do/buttons/state 26,                           |

| /do/2b3l/button2State   |                                                 |
|:------------------------|:------------------------------------------------|
| Info                    | [beta] [gpio] [buttons] [electronics] [pull-up] |
| Description             | Check state of button on pin 19                 |
| Usage                   | /do/2b3l/button2State                           |
| Modules                 | /do/buttons/state 19,                           |

| /do/2b3l/greenOff   |                                   |
|:--------------------|:----------------------------------|
| Info                | [beta] [gpio] [led] [electronics] |
| Description         | Turn off green led (pin 16)       |
| Usage               | /do/2b3l/greenOff                 |
| Modules             | /do/led/off 16,                   |

| /do/2b3l/greenOn   |                                   |
|:-------------------|:----------------------------------|
| Info               | [beta] [gpio] [led] [electronics] |
| Description        | Turn on green led (pin 16)        |
| Usage              | /do/2b3l/greenOn                  |
| Modules            | /do/led/on 16,                    |

| /do/2b3l/greenState   |                                              |
|:----------------------|:---------------------------------------------|
| Info                  | [beta] [gpio] [led] [electronics] [wiringpi] |
| Description           | get state of green led (pin 16)              |
| Usage                 | /do/2b3l/greenState                          |
| Modules               | /do/led/state 16,                            |

| /do/2b3l/install                     |                                                        |
|:-------------------------------------|:-------------------------------------------------------|
| Info                                 | [alpha] [undocumented]                                 |
| Modules                              | /do/2b3l/logoGreen, /do/2b3l/pinOut, /do/2b3l/logoRed, |
| 1. Test : /do/2b3l/test              |                                                        |
| 2. Setup : /do/2b3l/setup            |                                                        |
| 3. Security Mode : /do/2b3l/security |                                                        |

| /do/2b3l/logoGreen   |                        |
|:---------------------|:-----------------------|
| Info                 | [alpha] [undocumented] |

| /do/2b3l/logoRed   |                        |
|:-------------------|:-----------------------|
| Info               | [alpha] [undocumented] |

| /do/2b3l/pinOut   |                                                                                                                                 |
|:------------------|:--------------------------------------------------------------------------------------------------------------------------------|
| Info              | [beta] [gpio] [led] [electronics] [schematics] [buttons]                                                                        |
| Description       | Display how to plug leds and buttons                                                                                            |
| Usage             | /do/2b3l/pinOut                                                                                                                 |
| Variables         | r=$(tput setaf 1), y=$(tput setaf 3), b=$(tput setaf 6), p=$(tput setaf 5), n=$(tput sgr 0), w=$(tput bold), g=$(tput setaf 2), |

| /do/2b3l/redOff   |                                   |
|:------------------|:----------------------------------|
| Info              | [beta] [gpio] [led] [electronics] |
| Description       | Turn off red led (pin 21)         |
| Usage             | /do/2b3l/redOff                   |
| Modules           | /do/led/off 21,                   |

| /do/2b3l/redOn   |                                   |
|:-----------------|:----------------------------------|
| Info             | [beta] [gpio] [led] [electronics] |
| Description      | Turn on red led (pin 21)          |
| Usage            | /do/2b3l/redOn                    |
| Modules          | /do/led/on 21,                    |

| /do/2b3l/redState   |                                              |
|:--------------------|:---------------------------------------------|
| Info                | [beta] [gpio] [led] [electronics] [wiringpi] |
| Description         | get state of red led (pin 21)                |
| Usage               | /do/2b3l/redState                            |
| Modules             | /do/led/state 21,                            |

| /do/2b3l/security                        |                                                                                                                                                                                                                                                                 |
|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Info                                     | [alpha] [undocumented]                                                                                                                                                                                                                                          |
| Modules                                  | /do/2b3l/logoRed, /do/2b3l/allOff, /do/2b3l/scripts/samba/remove, /do/2b3l/scripts/ssh/remove, /do/2b3l/scripts/ssh/add, /do/2b3l/scripts/samba/add, cp /do/2b3l/config/security.cfg /user/config/buttons/buttons.cfg, /do/buttons/restart, /do/2b3l/logoGreen, |
| 1. Red Led: Terminal                     |                                                                                                                                                                                                                                                                 |
| 2. Yellow Led: Filesharing in use        |                                                                                                                                                                                                                                                                 |
| 3. Green Led: Filesharing active         |                                                                                                                                                                                                                                                                 |
| 4. Button 1: Toggle Filesharing $PICOLOR |                                                                                                                                                                                                                                                                 |
| 5. Button 2: Shutdown                    |                                                                                                                                                                                                                                                                 |

| /do/2b3l/securityOff   |                                                                                            |
|:-----------------------|:-------------------------------------------------------------------------------------------|
| Info                   | [alpha] [undocumented]                                                                     |
| Modules                | /do/2b3l/allOff, /do/2b3l/scripts/samba/stop, /do/2b3l/scripts/ssh/stop, /do/buttons/stop, |

| /do/2b3l/securityOn   |                                                                                               |
|:----------------------|:----------------------------------------------------------------------------------------------|
| Info                  | [alpha] [undocumented]                                                                        |
| Modules               | /do/2b3l/allOff, /do/2b3l/scripts/samba/start, /do/2b3l/scripts/ssh/start, /do/buttons/start, |

| /do/2b3l/securityRestart   |                                            |
|:---------------------------|:-------------------------------------------|
| Info                       | [alpha] [undocumented]                     |
| Modules                    | /do/2b3l/securityOff, /do/2b3l/securityOn, |

| /do/2b3l/setButtons   |                        |
|:----------------------|:-----------------------|
| Info                  | [alpha] [undocumented] |
| Modules               | /do/buttons/settings,  |

| /do/2b3l/setup   |                                            |
|:-----------------|:-------------------------------------------|
| Info             | [alpha] [undocumented]                     |
| Modules          | /show/commandMenu /do/2b3l/menu/menu.conf, |

| /do/2b3l/state   |                                                                                                                                                                                      |
|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Info             | [alpha] [undocumented]                                                                                                                                                               |
| Variables        | redState=$(/do/2b3l/redState), greenState=$(/do/2b3l/greenState), yellowState=$(/do/2b3l/yellowState), button1State=$(/do/2b3l/button1State), button2State=$(/do/2b3l/button2State), |
| Modules          | redState=$(/do/2b3l/redState), greenState=$(/do/2b3l/greenState), yellowState=$(/do/2b3l/yellowState), button1State=$(/do/2b3l/button1State), button2State=$(/do/2b3l/button2State), |

| /do/2b3l/test                |                                                                                                                          |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------|
| Info                         | [alpha] [undocumented]                                                                                                   |
| Modules                      | /do/2b3l/logoRed, cp /do/2b3l/config/leds.cfg /user/config/buttons/buttons.cfg, /do/buttons/restart, /do/2b3l/logoGreen, |
| 1. Button 1 to turn leds ON  |                                                                                                                          |
| 2. Button 2 to turn leds OFF |                                                                                                                          |

| /do/2b3l/yellowOff   |                                   |
|:---------------------|:----------------------------------|
| Info                 | [beta] [gpio] [led] [electronics] |
| Description          | Turn off yellow led (pin 20)      |
| Usage                | /do/2b3l/yellowOff                |
| Modules              | /do/led/off 20,                   |

| /do/2b3l/yellowOn   |                                   |
|:--------------------|:----------------------------------|
| Info                | [beta] [gpio] [led] [electronics] |
| Description         | Turn on yellow led (pin 20)       |
| Usage               | /do/2b3l/yellowOn                 |
| Modules             | /do/led/on 20,                    |

| /do/2b3l/yellowState   |                                              |
|:-----------------------|:---------------------------------------------|
| Info                   | [beta] [gpio] [led] [electronics] [wiringpi] |
| Description            | get state of yellow led (pin 20)             |
| Usage                  | /do/2b3l/yellowState                         |
| Modules                | /do/led/state 20,                            |
