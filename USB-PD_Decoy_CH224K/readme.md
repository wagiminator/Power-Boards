# USB Power Delivery Decoy (CH224K)
With the USB PD Decoy, a USB Type-C PD power adapter can be used as a power supply with the option of selecting different output voltages via DIP switches. It is based on the cheap and easy-to-use CH224K multi fast charging protocol power receiving chip.

![USB-PD_Decoy_CH224K_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Decoy_CH224K/USB-PD_Decoy_CH224K_pic1.jpg)

# CH224K USB PD Power Receiving Chip
The CH224K is a USB PD power receiving protocol chip, which integrates PD3.0/2.0, BC1.2 and other fast charging protocols, automatically detects VCONN and analog E-Mark chips, supports up to 100W power, and has built-in PD communication module. It also integrates output voltage detection internally to support overheating and overvoltage protection. It features:

- 4V to 22V input voltage
- PD3.0/2.0, BC1.2 and other fast charging protocols
- USB Type-C PD, positive and negative insertion detection and automatic switching
- E-Mark simulation, automatically detects VCONN, supports 100W power PD request
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

# Version with Power Path Control (PPC)
A second PCB version implements an additional MOSFET for power path control, which only enables the voltage output after successful negotiation with the power supply.

![USB-PD_Decoy_PPC_CH224K_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Decoy_CH224K/USB-PD_Decoy_PPC_CH224K_pic1.jpg)

# References, Links and Notes
1. [USB PD Adapter](https://github.com/wagiminator/ATtiny814-USB-PD-Adapter)
2. [CH224K Datasheet](https://datasheet.lcsc.com/lcsc/2204251615_WCH-Jiangsu-Qin-Heng-CH224K_C970725.pdf)
3. [TI Primer on USB PD](https://www.ti.com/lit/wp/slyy109b/slyy109b.pdf)

![USB-PD_Decoy_CH224K_pic2.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Decoy_CH224K/USB-PD_Decoy_CH224K_pic2.jpg)
![USB-PD_Decoy_CH224K_pic3.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Decoy_CH224K/USB-PD_Decoy_CH224K_pic3.jpg)
