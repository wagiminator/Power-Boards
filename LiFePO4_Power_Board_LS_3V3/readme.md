# LiFePO4 Power Board LS 3V3

Single cell LiFePO4 charging ([CN3058E](https://datasheet.lcsc.com/szlcsc/ShangHai-Consonance-Elec-CN3058E_C112011.pdf)) and protection ([HY2112](https://datasheet.lcsc.com/szlcsc/1810010241_HYCON-Tech-HY2112-BB_C161942.pdf)) board with load sharing power path management, 3.3V output und an additional switchable output. 

The board was developed for 3.3V projects that are operated both by battery and external power. The load sharing system interrupts the connection between the battery and the load when an external power supply is connected. In this case, the project is powered by the external power supply and the 3.3V voltage regulator while the battery is being charged. This protects the battery and increases its lifespan. Without an external power supply, the project is powered directly by the battery, which means that the output voltage depends on the battery charge level (about 2.7 - 3.5V). Furthermore the board is equipped with an additional output port (SL) that can be switched via the built-in MOSFET. If the EN pin is pulled to ground, for example via a GPIO pin of a microcontroller, then the SL output is activated. The maximum output current is 1A.

![LiFePO4_Power_Board_LS_3V3_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiFePO4_Power_Board_LS_3V3/LiFePO4_Power_Board_LS_3V3_pic1.jpg)
