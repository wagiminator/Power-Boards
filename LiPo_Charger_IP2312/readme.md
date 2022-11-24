# IP2312 LiPo Charger
Single cell Li-Ion/LiPo battery synchronous switch-mode fast charging board (up to 3A) with USB Type-C port.

![LiPo_Charger_IP2312_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Charger_IP2312/LiPo_Charger_IP2312_pic1.jpg)

The [IP2312](https://datasheet.lcsc.com/lcsc/2101081834_INJOINIC-IP2312-4V35_C605433.pdf) is a synchronous switch step-down battery charging IC. It features:
- Synchronous switch step-down charging
- Charging efficiency 94% (3.7V/2A)
- Maximum charge current 3A
- Charging current external resistance can be adjusted
- Automatically adjust the input current, compatible with small current adapters
- Support 4.20V/4.30V/4.35V/4.4V battery
- Support charging NTC temperature protection
- Support LED charging status indication
- Built-in power MOS
- 750KHz switching frequency, can support 1uH inductor
- Input overvoltage and undervoltage protection
- IC over temperature protection
- Charging overtime protection

The maximum charging current can be set by resistor R4 (ISET):
ISET = R4 = 135kV / I_CHARGE
|Max Charging Current|R4 (ISET)|
|-:|-:|
|1A|135k|
|1.5A|91k|
|2.1A|n.c.|
|3A|45k|

The maximum charging voltage can be set by resistor R6 (VSET):
|Max Charging Voltage|R6 (VSET)|
|-:|-:|
|4.2V|n.c.|
|4.3V|43k|
|4.35V|75k|
|4.4V|100k|

![LiPo_Charger_IP2312_pic2.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Charger_IP2312/LiPo_Charger_IP2312_pic2.jpg)
![LiPo_Charger_IP2312_pic3.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Charger_IP2312/LiPo_Charger_IP2312_pic3.jpg)
