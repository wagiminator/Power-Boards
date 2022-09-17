# FP6277 LiPo Power Board

Li-Ion battery charger, protector and 5V/3A booster. Use unprotected Li-Ion batteries with low internal resistance which are rated for a discharge current of at least 7A! Connect the battery with short wires of 20AWG or thicker! Attach a heatsink on the back side of the PCB when drawing more than 2A of current continuously! Use a slide switch that can withstand a current of 6A!

![LiPo_Power_Board_FP6277_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Power_Board_FP6277/LiPo_Power_Board_FP6277_pic1.jpg)

# Working Principle
For battery charging the [TP4056](https://datasheet.lcsc.com/szlcsc/1904031009_TPOWER-TP4056_C382139.pdf) (U1) is used. The TP4056 is a complete constant-current/constant-voltage linear charger for single cell lithium-ion batteries. The charge voltage is fixed at 4.2V and the charge current (max 1000mA) can be programmed externally with a single resistor (R3). The TP4056 automatically terminates the charge cycle when the charge current drops to 1/10th the programmed value after the final float voltage is reached. Other features include current monitor, under voltage lockout and automatic recharge.

For the battery protection (overcharge, overdischarge, overcurrent and short circuit protection) the [DW01A](https://datasheet.lcsc.com/szlcsc/1901091236_PUOLOP-DW01A_C351410.pdf) (U2) is used in combination with two [FS8205](https://datasheet.lcsc.com/szlcsc/Fortune-Semicon-FS8205_C32254.pdf) dual MOSFETs in parallel (Q1 + Q2). The DW01A is constantly measuring the voltage across the battery and the current flowing in (when charging) or coming out (when discharging). If something goes wrong it takes the battery out of the circuit by closing the MOSFETs which act like a switch between the negative side of the battery (B-) and ground. The overcurrent protection works by comparing the voltage drop across the MOSFET with the internal 150mV reference of the DW01A. As the RDS(on) of one FS8205 is around 2x25mOhm, the DW01A would close the MOSFET at 150mV/50mOhm = 3A if only one FS8205 were used. By using two FS8205 in parallel, the resistance is cut in half, so the DW01A shuts down at 150mV/25mOhm = 6A and one FS8205 must only handle half of the current (3A) which is well within its specs. In this way, up to 6 amps can flow from the battery into the boost converter with a maximum voltage drop of 150mV.

To step up the voltage to 5V the [FP6277](https://datasheet.lcsc.com/szlcsc/Feeling-Tech-FP6277XR-G1_C88312.pdf) low-cost synchronous boost converter is used (U3). Instead of a diode that is used in conventional boost converters, it switches a second built-in MOSFET in sync with the first via the PWM signal. This significantly increases efficiency and thus higher output currents are possible.

# Performance

![LiPo_Power_Board_FP6277_performance.png](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Power_Board_FP6277/LiPo_Power_Board_FP6277_performance.png)
![LiPo_Power_Board_FP6277_charge.png](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/LiPo_Power_Board_FP6277/LiPo_Power_Board_FP6277_charge.png)

# License

![license.png](https://i.creativecommons.org/l/by-sa/3.0/88x31.png)

This work is licensed under Creative Commons Attribution-ShareAlike 3.0 Unported License. 
(http://creativecommons.org/licenses/by-sa/3.0/)
