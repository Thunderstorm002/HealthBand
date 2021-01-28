# Objectives:
* Health-band that would track:
- [ ] ECG (Heart rate, Hear rate variability)
- [ ] Body temprature
- [ ] PPG (Heart rate, SPO2)
- [ ] Biopotential/Bioimpedance (can be used to check body composition and respiration when strapped to chest)
- [ ] Accelerometer (step count, fall detection)

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
	2. [AD8233](https://www.analog.com/en/products/AD8233.html#product-overview): Fully integrated, single-lead ECG front end
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
	2. 
4. Sensor Hub:
	1. MAX32664: (Version C Heart-rate, SpO2 using wrist) Low Power Sensor Hub Family which Seamlessly Communicates with Several Maxim Bio-metric Sensors [MAX32664GTGC+](https://www.mouser.in/ProductDetail/Maxim-Integrated/MAX32664GTGC%2b/?qs=vmHwEFxEFR%252B4L9bBONurNg%3D%3D)
		* <u>Cost</u>: ₹330
	2. [ADPD4100](https://www.analog.com/en/products/ADPD4100.html#product-overview) 
5. NRF5340: Main MCU and BLE
6. BMA456: Accelerometer