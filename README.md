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
<img width="918" height="516" alt="Screenshot 2026-01-27 135514" src="https://github.com/user-attachments/assets/dc3e936f-ab9a-4689-8cdc-cad3c1db56b0" />

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
| S.No | Input Signal    | Frequency        | Expected Output                                        | Practical Observation (Proteus)                         |
| ---- | --------------- | ---------------- | ------------------------------------------------------ | ------------------------------------------------------- |
| 1    | Sine wave       | Low (≈100 Hz)    | Small amplitude cosine wave, output leads input by 90° | Output is small, phase lead clearly observed            |
| 2    | Sine wave       | Medium (≈500 Hz) | Increased output amplitude, still leading by 90°       | Output amplitude increases, clean waveform              |
| 3    | Sine wave       | High (≈1 kHz)    | Large output amplitude (∝ frequency)                   | Output amplitude much higher, slight distortion visible |
| 4    | Square wave     | Medium           | Sharp spikes at rising and falling edges               | Spikes observed at transitions                          |
| 5    | Triangular wave | Medium           | Square wave output                                     | Nearly square waveform obtained                         |

## Waveforms
<img width="1920" height="1080" alt="Screenshot 2026-01-27 135455" src="https://github.com/user-attachments/assets/1c3ff548-6cc3-43ae-8e35-66340b14cc6c" />

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
1. What is a differentiator? 
ANS: A differentiator is an op-amp circuit in which the output voltage is proportional to the rate of change of the input voltage.
2. Write the output equation of differentiator. 
ANS: Vout​=−RCdVin/dt​​
3. Why is output leading input? 
ANS: Because the output depends on the rate of change of the input, the output responds faster than the input signal, causing it to lead in phase.
4. What happens at very high frequency?
ANS: The gain becomes very high, which may cause noise amplification and instability.
5. What is practical differentiator?
ANS: A practical differentiator is a modified differentiator circuit that includes additional resistor and capacitor to limit high-frequency gain and improve stability.

