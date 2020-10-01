# Power Boards
Collection of DC/DC converters, battery chargers and power supplies.

# Power Bank 3A

Powerbank based on FP6277 boost converter with 5V and 3.3V output up to 3A. Choose a good 18650 Li-Ion battery with a low internal resistance which is capable of delivering up to 7A!

|Parameter|Value|
|-|-|
|Battery Charge Current|max 1000 mA|
|Battery Discharge Current|max 7000 mA|
|Continuous Output Current|max 2500 mA|
|Peak Output Current|max 3200 mA|
|Quiescent Current|< 3 uA|

![IMG_20200614_131700_x.jpg](https://image.easyeda.com/pullimage/919dwwwVmEnrJDwjf5GN63aevVNBjDQ9nd0qLIZs.jpeg)
![IMG_20200614_131738_x.jpg](https://image.easyeda.com/pullimage/bBlxwvgvj511PKvi4o0TkMSiLXCxyM22GjvZIyPd.jpeg)

# Solar Charger

Solar powered switch-mode charger (CN3801), protector (HY2112) and 5V booster (MT3608) for LiFePO4 batteries. The charger provides maximum power point tracking (MPPT) and can easily be modified to work with LiPo batteries.

![IMG_20200119_095551_x.jpg](https://image.easyeda.com/pullimage/Ui9qe2Je15IpZDE19nuDCwFDMZIlMCXtmcegueQM.jpeg)

![IMG_20200119_145247.jpg](https://image.easyeda.com/pullimage/buIbtVveY68K2ZP84XXalirPuXEVamQoe3MyrAS6.jpeg)

# LiPo Charger (TP4056)

LiPo battery charging and protection circuit.

![LiPoCharger.jpg](https://image.easyeda.com/pullimage/1AFRDXL18TS9FlEvhszar0sCkHfKe3Lg5W7eNZ97.jpeg)

# LiPo Power Board (IP5306)

LiPo battery charger, protector and 5V booster based on the IP5306 with MicroUSB or USB-C port featuring:
- synchronous switch-mode charging with up to 2.1A / 91% efficiency,
- discharging with up to 2.4A,
- 5V boost converter with up to 92% efficiency,
- integrated power-path management (charging battery and 5V output at the same time),
- voltage based fuel gauge indication with 4 LEDs,
- on/off key,
- smart load detector (switching to standby mode automatically),
- less than 100uA standby current,
- charging/boosting with a single inductor,
- output over-current, over-voltage, short-circuit protection,
- input over-voltage, over-current protection,
- battery over-charge, over-drain, over-current protection,
- thermal shutdown.

Key functions:
- If button is pushed longer than 30ms but shorter than 2s, IP5306 will identify the action as short push. Short push will activate state of charge (SOC) indicator LEDs and step-up converter.
- If two short pushes are detected within 1s, IP5306 will deactivate step-up converter, SOC indicator LEDs and PWR LED (flashlight).
- If button is pushed longer than 2s, IP5306 will identify the action as long push. Long push will enable or disable PWR LED (flashlight).
- If button is pushed shorter than 30ms, IP5306 will ignore the action.

![IMG_20200111_160606_x.jpg](https://image.easyeda.com/pullimage/rxdgYDNxoOJD6VvLInlVP580dBqVBJwm64oJ3WG0.jpeg)
![IMG_20200806_170113_x.jpg](https://image.easyeda.com/pullimage/29fr5i6Ls9qVSXgj1bzG9rKqmmX9oJmnZgL4GFrm.jpeg)

# LiPo Power Board (FP6277)

Li-Ion battery charger (TP4056), protector (DW01A) and 5V/3A booster (FP6277). Use unprotected Li-Ion batteries with low internal resistance which are rated for a discharge current of at least 7A! Connect the battery with short wires of 20AWG or thicker! Attach a heatsink on the back side of the PCB when drawing more than 2A of current continuously! Use a slide switch that can withstand a current of 6A!

![IMG_20200416_162630_x.jpg](https://image.easyeda.com/pullimage/ZtWrjAydPL3rpFxg8FzVYH4KKxGVADAqohTF13Yd.jpeg)

# LiPo Power Board (FP6298)

Li-Ion battery charger (TP4056), protector (DW01A) and 5V/2A booster (FP6298). Use unprotected Li-Ion batteries which are rated for a discharge current of at least 5A !

![IMG_20200330_124927_x.jpg](https://image.easyeda.com/pullimage/bRBb8FD9yUtVva9H7F6e39vb6Yv6SrIVKecqImYC.jpeg)

# LIR2032 Charger (TP4056)

Charger for LIR2032 Li-Ion batteries.

![IMG_20200111_160350_x.jpg](https://image.easyeda.com/pullimage/EShLyzT9JReVfZoNtx9tAFyMHE65saIXZoaC6Sfo.jpeg)

# LiFePO4 Charger (CN35058)

One cell LiFePO4 battery charger and protector.

![IMG_20190721_164209.jpg](https://image.easyeda.com/pullimage/4ykMOFt3d5ls7DusMjOq662KOYd00YjNfU30758B.jpeg)

# LiFePO4 Power Board LS 3V3

Single cell LiFePO4 charging (CN3058E) and protection (HY2112) board with load sharing power path management, 3.3V output und an additional switchable output. 

The board was developed for 3.3V projects that are operated both by battery and external power. The load sharing system interrupts the connection between the battery and the load when an external power supply is connected. In this case, the project is powered by the external power supply and the 3.3V voltage regulator while the battery is being charged. This protects the battery and increases its lifespan. Without an external power supply, the project is powered directly by the battery, which means that the output voltage depends on the battery charge level (about 2.7 - 3.5V). Furthermore the board is equipped with an additional output port (SL) that can be switched via the built-in MOSFET. If the EN pin is pulled to ground, for example via a GPIO pin of a microcontroller, then the SL output is activated. The maximum output current is 1A.

![IMG_20200717_181709_x.jpg](https://image.easyeda.com/pullimage/xZenRbHvMLCdmepBq4AwWu1916SgY7jjzBTp54yF.jpeg)

# LiFePO4 Power Board LS 5V

Single cell LiFePO4 charger (CN3058E), protector (HY2112) and 5V booster (MT3608) board with load sharing power path management.

The board was developed for 5V projects that are operated both by battery and external power. The load sharing system interrupts the connection between the battery and the load when an external power supply is connected. In this case, the project is powered by the external power supply while the battery is being charged. This protects the battery and increases its lifespan. The maximum output current is 1A.

![IMG_20200717_181618_x.jpg](https://image.easyeda.com/pullimage/Wa2umGI3BfJwbjposDb5Fg25JV4E4ipz6PLd5LOi.jpeg)

# USB-C PD Max Trigger

Very simple USB-C Power Delivery trigger board based on the IP2721 that requests the maximum voltage (up to 20V) from the power supply.

![IMG_20200712_130242_x.jpg](https://image.easyeda.com/pullimage/KhicZ02sJj8aRwT7HONIKgJYQr7za6HGb05xTSOy.jpeg)

# USB-C PD Buck Converter

A slightly different approach to USB-C power delivery by combining a PD maximum voltage trigger (IP2721, up to 20V) and a buck converter (MP2307). The output voltage can be selected via the voltage divider (R5 + R6). The maximum output current is 3A.

![IMG_20200712_130214_x.jpg](https://image.easyeda.com/pullimage/EQfjEryWefvVntioPtvdtKiLcoezcSjCVIvwx2Gj.jpeg)

# Buck Converter (MP2307)

3A buck converter based on MP2307. Fixed output voltage can be defined via the voltage divider.

![IMG_20190726_133342.jpg](https://image.easyeda.com/pullimage/rahd7Wc1zkiYGPVX175igG8T43oeKwF9p2yL1J9w.jpeg)

# Buck Converter (LM2596)

5V/4A Buck Converter based on the LM2596.

![IMG_20200111_160419_x.jpg](https://image.easyeda.com/pullimage/u7gXdgO6U9UGPXfZC9cimWuZ6az31SlvdAqcG5HZ.jpeg)

# Boost Converter (MT3608)

Boost converter with USB plug. Fixed output voltage can be defined via the voltage divider.

![IMG_20200112_124304_x.jpg](https://image.easyeda.com/pullimage/K8Bdxui2yqWwZzSk6TuPmTPbPUSVSljN5FRV8h00.jpeg)

# Boost Converter (TPS61169)

Constant current boost converter and LED Driver with USB Plug.

![IMG_20200315_151415_x.jpg](https://image.easyeda.com/pullimage/hsKdiqPm0A75mJzs1EiWkaLzdW4FENb6iK2JoRHU.jpeg)

# SEPIC (MT3608)

Simple single ended primary inductance converter (SEPIC) based on the MT3608 with a fixed output voltage selectable by the resistor values of the voltage divider.

![IMG_20200806_170226_q.jpg](https://image.easyeda.com/pullimage/Voqvhdh1PErloHANypPeMHkhQYi1d9WUSHJrtioN.jpeg)
