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

1.Designed and simulated the Buck converter topology using MATLAB Simulink.

2.Verified key waveforms in Continuous Conduction Mode (CCM):

a.Inductor current

b.Diode voltage

3.Increased load resistance to observe Discontinuous Conduction Mode (DCM).



HARDWARE IMPLEMENTATION:

1.Built the Buck converter using discrete components and used TL494 as the PWM generator.

2.Observed real-time waveforms on an oscilloscope to validate:

a.Output voltage regulation

b.Diode switching

c.Inductor current shape

3.Fine-tuned the duty cycle through TL494 to achieve the desired output voltage for different load conditions.



PCB DESIGN:

1.Designed a custom PCB layout tailored for the Buck converter circuit.

2.Soldered and tested the complete system on the fabricated PCB board to ensure reliable operation under various input and load conditions.



CHALLENGES FACED:

Soldering Issues: Precise soldering was required. Excess solder bridged copper traces, which had to be manually corrected.

Driver Circuit Debugging: PWM output was distorted due to a faulty MOSFET driver. After replacing the IC and rechecking components, proper output was achieved.

Overcurrent & Heating: During main PCB testing, the circuit drew excessive current and the output capacitor overheated above 18V.


LEARNINGS:

Diode Voltage Spike: A spike at switch-off was observed across the diode—likely due to parasitic effects.

Importance of Driver IC: Driving the MOSFET without a proper driver resulted in distorted waveforms. A dedicated driver IC significantly improved switching clarity
