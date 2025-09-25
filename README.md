# FM-using-Python

Aim


To implement and analyze frequency modulation (FM) using Python's NumPy and Matplotlib libraries. 

Apparatus Required

1.	Software: Python with NumPy and Matplotlib libraries
2.	Hardware: Personal Computer
  
Theory

Frequency Modulation (FM) is a method of transmitting information over a carrier wave by varying its frequency in accordance with the amplitude of the input signal (message signal). The frequency of the carrier wave is varied according to the instantaneous amplitude of the message signal. The general form of an FM signal is:



Algorithm


1.	Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and frequency deviation.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
5.	Generate FM Signal: Apply the FM modulation formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

Program
Am=4.2; 
fm=347;
Ac=8.4;
fc=3470;
fs=34700;
B=3.05;
t=0:1/fs:2/fm;
m=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,m);
c=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,c);
Efm=Ac*cos((2*3.14*fc*t)+(B*sin(2*3.14*fm*t)));
subplot(3,1,3);
plot(t,Efm);



Output Waveform
<img width="1801" height="981" alt="image" src="https://github.com/user-attachments/assets/f0dbcb59-bdd2-4b16-9563-d381011d236e" />



Tabular Column
![WhatsApp Image 2025-09-25 at 22 44 42_30e86acb](https://github.com/user-attachments/assets/b73b3c89-42cb-4051-9320-d34537fc446b)




Calculation




Result


The message signal, carrier signal, and frequency modulated (FM) signal will be displayed in separate plots. The modulated signal will show frequency variations corresponding to the amplitude of the message signal.
