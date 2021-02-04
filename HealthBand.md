# Objectives:
* Health-band that would track:
- [x] ECG (Heart rate, Hear rate variability)
- [x] Body temprature
- [x] PPG (Heart rate, SPO2)
- [x] Biopotential/Bioimpedance (can be used to check body composition and respiration when strapped to chest)
- [x] Accelerometer (step count, fall detection)

# Components:
1. **ECG**:
	1. [MAX30001](https://www.maximintegrated.com/en/products/analog/data-converters/analog-front-end-ics/MAX30001.html#tech-docs): Ultra-Low-Power, Single-Channel Integrated Biopotential (ECG, R-to-R, and Pace Detection) and Bioimpedance (BioZ) AFE
		* <u>Cost</u>: ₹702
		* <u>Features</u>:
			* Clinical-Grade ECG and BioZ AFE with High Resolution Data Converter (IEC 60601-2-47:2012)
			*  CMRR > 100dB
			* Lead-On Detect 
			* Built-In Heart Rate Detection
			* Low power
	2. [MAX30003](https://www.maximintegrated.com/en/products/analog/data-converters/analog-front-end-ics/MAX30003.html)
		* <u>Cost</u>: ₹598
		* Choosing this for now.
	3.  [AD8233](https://www.analog.com/en/products/AD8233.html#product-overview): Fully integrated, single-lead ECG front end
		* <u>Cost</u>: ₹313
		* <u>Features</u>:
			* Leads on/off detection 
			* Common-mode rejection ratio: 80 dB 
2. **Body temperature**:
	1. MAX30205: Clinical Grade Temperature Sensor Offers ±0.1°C (max) Accuracy for Thermometer Applications
		* <u>Cost</u>: ₹183
3. **PPG**:
	1. [MAX86141](https://www.maximintegrated.com/en/products/interface/sensor-interface/MAX86141.html): Best-in-Class Optical Pulse Oximeter and Heart-Rate Sensor for Wearable Health
		* <u>Cost</u>: ₹583
		* Doesn't have integrated LEDs or photodiode
	2. [ADPD1081](https://www.analog.com/en/products/adpd1081.html#product-overview):
		* <u>Cost</u>: ₹421
		* photodiode costs around ₹100
		* Red, IR, Green LEDs are around ₹60 so ₹180 total 
		* Doesn't have integrated LEDs or photodiode
	3. [MAX86176](https://www.maximintegrated.com/en/products/sensors/MAX86176.html?intcid=para)
		* Not available.
		* Datasheet requires an NDA.
	4. [MAX86916](https://www.maximintegrated.com/en/products/sensors/MAX86916.html/product-details/tabs-3)
		* <u>Cost</u>: ₹798
		* Integrated LEDs or photodiode
	5. [MAXM86161EFD+](https://www.mouser.in/ProductDetail/Maxim-Integrated/MAXM86161EFD%2b/?qs=PzGy0jfpSMvG%2FmijvXlxVg%3D%3D)
		* <u>Cost</u>: ₹663.57
		* Integrated LEDs or photodiode
		* Choosing this for now because of integrated LEDs and decent price range (approximately the same if you include photodiode and LEDs with other components to other ICs).
4. Sensor Hub:
	1. [MAX32664](https://www.maximintegrated.com/en/products/interface/sensor-interface/MAX32664.html): (Version C Heart-rate, SpO2 using wrist) Low Power Sensor Hub Family which Seamlessly Communicates with Several Maxim Bio-metric Sensors [MAX32664GTGC+](https://www.mouser.in/ProductDetail/Maxim-Integrated/MAX32664GTGC%2b/?qs=vmHwEFxEFR%252B4L9bBONurNg%3D%3D)
		* <u>Cost</u>: ₹330
		* Since we are going to use Maxim stuff it makes sense to use this.
	2. [ADPD4100](https://www.analog.com/en/products/ADPD4100.html#product-overview) 
5. NRF5340: Main MCU and BLE
6. BMA456: Accelerometer
7. Biopotential/Bioimpedace:
	1. Using bioimpedance to measure blood glucose levels (https://www.hindawi.com/journals/aelc/2014/406257/)
	2. [AD5941](https://www.analog.com/en/products/ad5941.html#product-overview)
	3. 