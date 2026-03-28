## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Resistor R = 10 kΩ
•	Capacitor Cf = 0.01 µF
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="603" height="376" alt="Screenshot 2026-02-25 135456" src="https://github.com/user-attachments/assets/8e982210-31c8-4910-b50b-213e06d98c32" />

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)
•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal
•	Output is inverted
•	Output depends on time
For Sine Wave Input:
•	Output lags input by 90°
•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
| **S.No** | **Input Signal** | **Frequency** | **Expected Output**          | **Practical Observation**                |
| -------- | ---------------- | ------------- | ---------------------------- | ---------------------------------------- |
| 1        | Square wave      | 100 Hz        | Positive and negative spikes | Sharp spikes at rising and falling edges |
| 2        | Triangular wave  | 100 Hz        | Square wave                  | Square wave obtained                     |
| 3        | Sine wave        | 100 Hz        | Cosine wave                  | Phase-shifted sine wave observed         |
| 4        | Square wave      | 1 kHz         | Higher amplitude spikes      | Narrow and sharper spikes observed       |
| 5        | Sine wave        | 1 kHz         | Higher amplitude cosine wave | Output amplitude increased               |

## Waveforms
<img width="756" height="472" alt="Screenshot 2026-02-25 135522" src="https://github.com/user-attachments/assets/92dda498-a4a7-4226-b893-8d5366c56cc5" />
<img width="756" height="472" alt="Screenshot 2026-02-25 135510" src="https://github.com/user-attachments/assets/2845be46-cbe2-4246-b6ed-29eb337edc0b" />
<img width="756" height="462" alt="Screenshot 2026-02-25 135533" src="https://github.com/user-attachments/assets/37f96248-3a75-4947-bb68-0d3b3e5295c0" />

## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.
## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions
1. What is an integrator circuit?
An integrator circuit is an op-amp based circuit in which the output voltage is proportional to the time integral of the input voltage. It is commonly implemented using an operational amplifier with a resistor at the input and a capacitor in the feedback path.

2. Write the output equation of integrator.
   The output voltage of an ideal integrator is given by
             Vo​=−RC1​∫Vi​dt
   
3. Why does output lag input?
The output of an integrator lags the input because integration introduces a phase shift of −90°, which is due to the charging and discharging behavior of the capacitor in the feedback path.

4. What happens at very low frequency?
At very low frequencies or DC input, the capacitor behaves like an open circuit, causing the output voltage to increase continuously and drive the op-amp into saturation.

5. What is practical integrator?
A practical integrator is an improved integrator circuit in which a resistor is connected in parallel with the feedback capacitor to limit the gain at low frequencies and prevent saturation.
4. What happens at very high frequency?
ANS: The gain becomes very high, which may cause noise amplification and instability.
5. What is practical differentiator?
ANS: A practical differentiator is a modified differentiator circuit that includes additional resistor and capacitor to limit high-frequency gain and improve stability.

