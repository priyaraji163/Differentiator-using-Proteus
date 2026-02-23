## Experiment No: 3
DIFFERENTIATOR USING OP-AMP (μA741)
## Aim
To design and simulate a Differentiator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the rate of change of input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Capacitor C = 0.01 µF
•	Resistor Rf = 10 kΩ
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="574" height="376" alt="DA" src="https://github.com/user-attachments/assets/30b846b5-99de-4c9b-8b5e-4a1320e78061" />

## Connection Details:
•	Input signal → Capacitor (C) → Inverting terminal (Pin 2)
•	Feedback resistor (Rf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
A Differentiator circuit produces an output voltage proportional to the rate of change of input voltage.
## Working Principle:
•	When input changes rapidly → output amplitude increases
•	When input is constant → output is zero
•	Output is inverted
## Procedure
1.	Open Proteus software.
2.	Select μA741, capacitor, resistor, signal generator, and CRO.
3.	Connect circuit in differentiator configuration.
4.	Apply ±15V power supply.
5.	Set input sine wave (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
S.No 	         Input Signal	              Frequency	            Expected  Output	            Practical Observation
<img width="963" height="276" alt="image" src="https://github.com/user-attachments/assets/8d943f76-a55c-4bcb-9560-8ecd4c187b80" />

## Waveforms
•	Sine input → Cosine output (90° phase shift)
•	Square input->  Positive & negative spikes
•	Triangular input → Square wave
<img width="1373" height="846" alt="DA-CosSine" src="https://github.com/user-attachments/assets/9ee16c6d-07b3-458f-b66c-943f7d50edd5" />
<img width="1381" height="850" alt="DA-SSW" src="https://github.com/user-attachments/assets/2057774a-57d4-4117-8cb7-fdd0d9e75a6e" />
<img width="1375" height="841" alt="DA-TR" src="https://github.com/user-attachments/assets/b6c64750-c3a8-4966-bcd4-5581a2caecc8" />



## Result
The Differentiator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the rate of change of input voltage.
The circuit behaves as a differentiator.
## Conclusion
•	Output depends on frequency.
•	Output leads input by 90° (for sine input).
•	Higher frequency → Higher output amplitude.
•	Used in wave shaping and signal processing applications.
## Viva Questions
1.	What is a differentiator?
A differentiator is an op-amp circuit that produces an output voltage proportional to the rate of change (derivative) of the input voltage.
It differentiates the input signal with respect to time.
2.	Write the output equation of differentiator.
Vout=-Rc dVin/dt
3.	Why is output leading input?
Differentiation of a sine wave results in a cosine wave.
Since cosine leads sine by 90°, the output of a differentiator leads the input by 90°.
Therefore, output is phase-shifted +90° (for sinusoidal input).
4.	What happens at very high frequency?
At very high frequency:
Capacitive reactance 
𝑋c=1/2*3.14*fC​becomes very small.
Gain increases.
Circuit amplifies high-frequency noise.
Output may become unstable.
Oscillations may occur.
So, ideal differentiator is not stable at high frequency.
5.	What is practical differentiator?
A practical differentiator is a modified differentiator circuit that includes:
A small resistor in series with the input capacitor.
A small capacitor in parallel with the feedback resistor.
These components:
Limit high-frequency gain.
Reduce noise.
Improve stability.

