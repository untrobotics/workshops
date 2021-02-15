This was our workshop from 14 Feb, 2021

## Cellular (SMS + DATA) with GPS

If you are not familiar with working with an ESP32, please see this guide: 

Parts list:
- LILYGO TTGO T-Call V1.4 ESP32 (with SIM800L module)
    - Manufacturer Info: http://www.lilygo.cn/prod_view.aspx?TypeId=50033&Id=1127&FId=t3:50033:3
    - Amazon Purchase: https://www.amazon.com/gp/product/B07VL9Z1SJ
- Adafruit Ultimate GPS Breakout (ADA746)
    - Manufactuerer Info: https://learn.adafruit.com/adafruit-ultimate-gps
    - Amazon Purchase: https://www.amazon.com/gp/product/B01H1R8BK0

### Wiring/Setup

The wiring for this workshop is very straightfoward, it needs only 4 wires. For additional debugging, you can [wire up two LEDs to the serial connections](https://github.com/untrobotics/workshops/blob/main/esp32/cellular%2Bgps/diagrams/serial-leds.jpg)
 to ensure communication is working as expected. This is a good idea if you're unsure if your soldering or pin connections are sound.
 
The first step is to add your SIM card to the ESP32 Dev board, the slot is on the bottom of the board, and the holder tab must be slid forward before it can be raised up to insert the SIM card, like below:
![Inserted SIM Card](diagrams/inserted-sim.jpg)


Now all we need to do is connect the GPS module to the ESP32's 3.3V and GND pins, as well as the TX/RX pins, as shown in the diagram below:
![Wiring Diagram](diagrams/esp32-ttgo%2Bgps.jpg)

And last, connect the USB to your computer!
