## CMOS Differential Amplifier Design using Cadence Virtuoso
A differential amplifier is an analog electronic circuit that amplifies the voltage difference between two input signals while rejecting any voltage common to both. It is a fundamental building block in analog circuit design and widely used in systems like operational amplifiers, analog-to-digital converters (ADCs), and sensors.
I have used a PMOS current mirror in this design.

## Simulation Results

- **Technology**: GPDK 90nm CMOS  
- **Differential Gain**: 29.54 dB (Ratio of differential output to input (in dB): 20*log10(Vo/Vi)) 
- **Common-Mode Rejection Ratio (CMRR)**: ~60 dB  (Ability to reject common input signals: CMRR = 20*log10(Ad/Acm))
- **Slew Rate**: ~1.5 V/µs (estimated)  (Maximum rate of change of output voltage with time: SR = dV/dt)
- **Output Voltage Swing**: 0.996 V to 1.0345 V (~38.5 mV peak-to-peak)  (Output voltage range without distortion)
- **Supply Voltage (VDD)**: 1.2 V

- 
### Schematic
![Screenshot 2025-06-06 150605](https://github.com/user-attachments/assets/a61ccbef-bbb0-4f62-a366-f5f7b87c6995)

### Testbench
![Screenshot 2025-06-06 150615](https://github.com/user-attachments/assets/a4040de4-292f-4bd4-a224-385e8d8e6a96)

### Transient Response
![Screenshot 2025-06-06 154037](https://github.com/user-attachments/assets/0015c980-8b38-4840-95bd-87acda24bb7d)

### AC Response
![Screenshot 2025-06-06 154300](https://github.com/user-attachments/assets/2f3ad280-6fc9-4665-9f62-8bd728dd1c24)

### DC Response
![Screenshot 2025-06-06 154356](https://github.com/user-attachments/assets/4037c37c-add5-4406-ac40-fd7d72c2b26a)

### LVS and DRC Reports
![LVS](https://github.com/user-attachments/assets/c8bc9de3-622a-483e-a22b-847d4bf77387)

![DRC](https://github.com/user-attachments/assets/f23dd4ee-c33f-4255-b74c-3ba2d65692c8)
