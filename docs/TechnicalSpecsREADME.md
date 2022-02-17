# Technical Specifications

The PBL is powered by an ESP32 microcontroller to which the LEDs are connected. One
ESP32 corresponds to one sparepartscontainer, multiple ESP32s are connected via WIFI
to a single Raspberry Pi which holds the Frontend and Backend software structures.

Further information can be found in the [users guide](../Documentation/PBL%20Users%20Guide.pdf).

## Our used hardware

Microcontroller: NodeMCU ESP32
LEDs: Adafruit Flora Smart NeoPixel RGB LED v2 (WS2812B controller)

As for our attachement of LEDs we designed 3D printable parts to fit specifically:

Spare parts container: 30,5cm x 15cm x 55cm

Compartment/drawer: 7cm x 14cm x 4cm

12 rows, 4 compartments per row

two 3cm wide steelflaps on the backside of the container to hold the mechanisms with neodym magnets

<img src="../Documentation/Users%20Guide/pictures/ContainerIlluminated.jpg" alt="front" width="350"/><img src="../Documentation/Users%20Guide/pictures/backsideContainer.jpg" alt="back" width="400"/>

## Wiring diagram

![Wiring Diagram](../Documentation/wiring%20diagram.png)

## Power consumption

(all specifications for Adafruit Flora Smart NeoPixel RGB LED v2)

One NeoPixel draws a maximum of 60mA if all color values are at 100%.
One sparepartscontainer with 48 compartments and so 48 LEDs draws a total of 2,9A at
3,3V.

Depending on how many compartments and LEDs you have per sparepartscontainer you
can either power the whole system via the ESP32's pins (as shown in the above wiring
diagram) or via a seperate powersupply. If you use the latter option make sure the ESP32
and the LEDs are connected to the same GROUND.

To find a suitable powersupply you can calculate the maximum power consumption of your
spare parts container with following formula:

60mA x (NumberOfLEDs) = Powerdrawage

The PBL system can only be powered by a maximum of 5V DC.

For further explanation of power consumption consult the [adafruit website](https://learn.adafruit.com/adafruit-neopixel-uberguide/powering-neopixels).