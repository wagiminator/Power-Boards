# USB Power Delivery Source (IP6520)
With the USB-PD Source, old power supplies can be transformed into modern fast charging adapters with a USB Type-C output port and an output power of up to 18W. The device masters the most common fast charging protocols (PD2.0, BC1.2, QC2.0, QC3.0, FCP, AFC e.g. for Apple, Samsung, Huawei) and can offer different voltages with high currents (5V/3A, 9V/2A, 12V/1.5A).

![USB-PD_Source_IP6520_pic1.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Source_IP6520/USB-PD_Source_IP6520_pic1.jpg)

# IP6520 Fast Charge Protocol Buck Converter
IP6510 is a synchronized switch buck regulator and supports 9 fast charge output standards, supports Type-C and PD output, providing solutions for car charger, fast charge adapter and smart power strip. It features:
- Synchronized Switch Regulator
  - Built-in power MOSFET
  - Input voltage range: 4.5V~32V
  - Output voltage range: 3V~12V, adjust along with fast charge negotiation
  - Output power: up to 18W (5V/3.1A, 7V/2.4A, 9V/2A, 12V/1.5A)
  - Output voltage line compensation: 50mV/A
  - Output CV/CC characteristic: CV—output - current lower than preset value; CC—output - current higher than preset value
  - Conversion efficiency: up to 97%
  - Soft start function
- Fast Charge Output
  - Support 5V, 9V, 12V USB Type-C PD output
  - Support BC1.2, Apple, Samsung
  - Support Qualcomm QC2.0, QC3.0
  - Support Huawei fast charge: FCP
  - Support Samsung fast charge: AFC
- Multi-protection and high reliability
  - Input overvoltage, input under voltage, output short circuit, output overcurrent protection
  - Whole system over temperature protection
  - ESD 4KV, DC voltage withstand 48V

# References, Links and Notes
1. [IP6520 Datasheet](http://www.injoinic.com/wwwroot/uploads/files/20200220/fd3ea4b1827198c71de61ee2b60a1079.pdf)
2. [TI Primer on USB PD](https://www.ti.com/lit/wp/slyy109b/slyy109b.pdf)

![USB-PD_Source_IP6520_pic2.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Source_IP6520/USB-PD_Source_IP6520_pic2.jpg)
![USB-PD_Source_IP6520_pic3.jpg](https://raw.githubusercontent.com/wagiminator/Power-Boards/master/USB-PD_Source_IP6520/USB-PD_Source_IP6520_pic3.jpg)
