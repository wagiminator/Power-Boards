1. Overview
-----------
Powerbank based on FP6277 boost converter with 5V and 3.3V output up to 3A. Choose a good 18650 Li-Ion battery with a low internal resistance which is capable of delivering up to 7A!

2. Working Principle
--------------------
For battery charging the TP4056 (U1) is used. The TP4056 is a complete constant-current/constant-voltage linear charger for single cell lithium-ion batteries. The charge voltage is fixed at 4.2V and the charge current (max 1000mA) can be programmed externally with a single resistor (R3). The TP4056 automatically terminates the charge cycle when the charge current drops to 1/10th the programmed value after the final float voltage is reached. Other features include current monitor, under voltage lockout and automatic recharge.

For the battery protection (overcharge, overdischarge, overcurrent and short circuit protection) the DW01A (U2) is used in combination with two FS8205 dual MOSFETs in parallel (Q1 + Q2). The DW01A is constantly measuring the voltage across the battery and the current flowing in (when charging) or coming out (when discharging). If something goes wrong it takes the battery out of the circuit by closing the MOSFETs which act like a switch between the negative side of the battery (B-) and ground. The overcurrent protection works by comparing the voltage drop across the MOSFET with the internal 150mV reference of the DW01A. As the RDS(on) of one FS8205 is around 2x25mOhm, the DW01A would close the MOSFET at 150mV/50mOhm = 3A if only one FS8205 were used. By using two FS8205 in parallel, the resistance is cut in half, so the DW01A shuts down at 150mV/25mOhm = 6A and one FS8205 must only handle half of the current (3A) which is well within its specs. In this way, up to 6 amps can flow from the battery into the boost converter with a maximum voltage drop of 150mV.

To step up the voltage to 5V the FP6277 low-cost synchronous boost converter is used (U3). Instead of a diode that is used in conventional boost converters, it switches a second built-in MOSFET in sync with the first via the PWM signal. This significantly increases efficiency and thus higher output currents are possible.

The UZ1085L low dropout voltage regulator (U4) provides a voltage of 3.3V with a current of up to 3A.

3. Performance
--------------
Parameter	                Value
---------------------------------------
Battery Charge Current	    max 1000 mA
Battery Discharge Current	max 7000 mA
Continuous Output Current	max 2500 mA
Peak Output Current	        max 3200 mA
Quiescent Current	        < 3 uA

