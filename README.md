Ethernet example sketches for Gadget Renesas KURUMI
========
These example skectshes allow to connect to Internet or network by using WIZ Ethernet library.  

## Supported devices
* ioShield serise, WIZ550io (used in W5500)
* W5200 Ethernet Shield, WIZ820io (used in W5200)
* Ethernet Shield and compatibles (used in W5100)

## Hardware
* ioShield  
* [W5200 Ethernet Shield](https://github.com/Wiznet/W5200-Ethernet-Shield "W5200 Ethernet Shield")  
* [Ethernet Shield](http://arduino.cc/en/Main/ArduinoEthernetShield "Ethernet Shield")  

## Software
#### Install WIZ Ethernet library
Download all files and overwrite onto the "RLduino78/libraries/Ethernet" folder in your project in sketch.  
[WIZ Ethernet Library Link](https://github.com/embeddist/Ethernet.git "Ethernet")  

#### Remove Arduino Ethernet Examples included in WIZ Ethernet library
Remove "\Ethernet\examples" folder in "RLduino78/libraries/Ethernet".

#### Select device(shield)  
Uncomment device(shiel) you want to use.  
```cpp
//Arduino\libraries\Ethernet\utility\w5100.h
#ifndef	W5100_H_INCLUDED
#define	W5100_H_INCLUDED

#include <avr/pgmspace.h>
#include <SPI.h>

typedef uint8_t SOCKET;
//#define W5100_ETHERNET_SHIELD
//#define W5200_ETHERNET_SHIELD
#define W5500_ETHERNET_SHIELD
```

## Revision History
Initial Release : 22 August 2013
