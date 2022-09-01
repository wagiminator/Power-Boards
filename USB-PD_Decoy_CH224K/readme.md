# USB Power Delivery Decoy (CH224K)
With the USB-PD Decoy, a USB-C power adapter can be used as a power supply with the option of selecting different output voltages via DIP switches. It is based on the cheap and easy-to-use CH224K multi-fast charging protocol power receiving chip.

![USB-PD_Decoy_CH224K_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Decoy_CH224K/USB-PD_Decoy_CH224K_pic1.jpg)

The CH224K integrates multiple fast charging protocols such as USB PD3.0/2.0, BC1.2 and other boost fast charging protocols on a single chip. It features:

- 4V to 22V input voltage
- PD3.0/2.0, BC1.2 and other fast charging protocols
- USB Type-C PD, positive and negative insertion detection and automatic switching
- E-Mark simulation, automatically detect VCONN, support 100W power PD request
- requested voltage can be dynamically adjusted through a variety of methods
- high integration of single chip, simplified peripheral and low cost
- built-in over-voltage and over-temperature protection module

The output voltage can be selected via the DIP switches as follows:

|Output Voltage|SW1|SW2|SW3|
|-|-|-|-|
|5V|0|-|-|
|9V|1|1|1|
|12V|1|1|0|
|15V|1|0|0|
|20V|1|0|1|

The Power-Good LED lights up when the selected voltage has been successfully negotiated with the USB-C power adapter and is present at the output. The voltage can also be changed during operation.

1. [CH224K Datasheet](https://datasheet.lcsc.com/lcsc/2204251615_WCH-Jiangsu-Qin-Heng-CH224K_C970725.pdf)
