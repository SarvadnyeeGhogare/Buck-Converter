GROUP - E2 B10

BUCK CONVERTER

This project focuses on the design, simulation, and hardware implementation of a Buck (step-down) DC-DC converter using the TL494 PWM controller IC.
The main objective was to realize a functioning converter capable of delivering a regulated lower voltage output from a higher input supply, using pulse-width modulation (PWM) control and verify its operation through both simulation and hardware testing.

SPECIFICATIONS:

Input Voltage : 25V
Output Voltage : 17.5V
Switching Frequency : 15kHz
Output Current : 1A

OVERVIEW:

The following steps were carried out:

MATLAB Simulink Simulation
1. Designed and simulated the Buck converter topology using MATLAB Simulink.
2.Verified key waveforms in Continuous Conduction Mode (CCM):
Inductor current
Diode voltage
3.Increased load resistance to observe Discontinuous Conduction Mode (DCM).

HARDWARE IMPLEMENTATION:

1.Built the Buck converter using discrete components and used TL494 as the PWM generator.
2.Observed real-time waveforms on an oscilloscope to validate:
Output voltage regulation
Diode switching
Inductor current shape
3.Fine-tuned the duty cycle through TL494 to achieve the desired output voltage for different load conditions.

PCB DESIGN:
1.Designed a custom PCB layout tailored for the Buck converter circuit.
2.Soldered and tested the complete system on the fabricated PCB board to ensure reliable operation under various input and load conditions.


