# Dual Active Bridge (DAB) DC-DC Converter Simulation (MATLAB/Simulink)

A Simulink model of a Dual Active Bridge (DAB) DC-DC converter that steps up a 10 V DC input to about 127 V across a 1 kΩ load.

## System modeled

- 10 V DC input source
- Two H-bridges (8 MOSFETs) and a high-frequency step-up transformer
- Series inductor and output capacitor
- 1 kΩ resistive load

## How it works

Both bridges switch at 1 kHz with 50% duty. The secondary bridge is delayed by a phase shift compared to the primary bridge, which makes current flow through the inductor and transfers power to the load. Changing the phase shift changes the power delivered.

## Results

- Load voltage: about 127 V
- Load current: about 0.127 A
- Settling time: about 0.3 s

## How to run

1. Open `DAB1_1_2024b.slx` in MATLAB/Simulink (R2024b).
2. Click **Run** and open the scopes to view the waveforms.

## Author

**Bolleboina Karthikeya**
