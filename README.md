# DSBSC


EX NO: 2	DSB-SC-AM MODULATOR AND DEMODULATOR

AIM:

To write a program to perform DSBSC modulation and demodulation using SCI LAB and study its spectral characteristics

EQUIPMENTS REQUIRED

•	Computer with i3 Processor
•	SCI LAB

Note: Keep all the switch faults in off position

Algorithm:

1.	Define Parameters:
•	Fs: Sampling frequency.
•	T: Duration of the signal.
•	Fc: Carrier frequency.
•	Fm: Frequency of the message signal.
•	Amplitude: Maximum amplitude of the message signal.
2.	Generate Signals:
•	Message Signal: A sinusoidal signal that will be modulated.
•	Carrier Signal: A high-frequency sinusoidal signal used for modulation.
3.	DSBSC Modulation:
•	Modulated Signal: Multiply the message signal by the carrier signal to produce the DSBSC signal.
4.	DSBSC Demodulation:
•	Multiplication: Multiply the modulated signal by the carrier signal to get the product of the message signal with itself (i.e., the original message signal plus high-frequency components).
•	Low-pass Filtering: Apply a Butterworth low-pass filter to remove the high- frequency components and recover the original message signal.
5.	Visualization:
Plot the message signal, carrier signal, DSBSC modulated signal, and the recovered signal after demodulation.
PROCEDURE

•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
 
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated waveform using Tabulation and Model Waveform

Model Waveform

<img width="703" height="679" alt="image" src="https://github.com/user-attachments/assets/e7c7c7f8-ccf2-41ac-b1f3-325989941a6f" />

Program
Ac=15.2; 
fc=3300; 
Am=7.6; 
fm=330; 
fs=50000; 
t=0:1/fs:2/fm; 
Wm=2*3.14*fm; 
Wc=2*3.14*fc; 
Em=Am*sin(2*3.14*fm*t); 
subplot(3,1,1); 
plot(t,Em); 
Ec=Ac*sin(2*3.14*fc*t); 
subplot(3,1,2); 
plot(t,Ec); 
Edsbsc=((Am/2)*cos((Wc-Wm)*t))-((Am/2)*cos((Wc+Wm)*t));
subplot(3,1,3); 
plot(t,Edsbsc);

Output Graph
<img width="1649" height="861" alt="Screenshot 2025-09-24 200035" src="https://github.com/user-attachments/assets/ddc8d20e-4ffb-4e7a-839a-713dd963cdb3" />



## Tablular Column
![WhatsApp Image 2025-11-13 at 08 36 54_ce320193](https://github.com/user-attachments/assets/6b9e0856-1b46-48bd-b1a9-de5623d9ba07)

## calculation
![WhatsApp Image 2025-11-13 at 08 43 10_9c76c08b](https://github.com/user-attachments/assets/854ea289-5078-47af-a052-94f6e4dad195)

Result

Thus the DSB-SC-AM Modulation and Demodulation is generated.

