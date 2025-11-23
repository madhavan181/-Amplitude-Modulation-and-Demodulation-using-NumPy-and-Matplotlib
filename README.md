Demodulation-using-NumPy-and-Matplotlib

__Aim__: 

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. 

__Apparatus Required__: 

Software: Python with NumPy and Matplotlib libraries 
Hardware: Personal Computer 

__Theory__: 

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting 
information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of 
the message signal. The general form of an AM signal is: 


__Algorithm__:
1. Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency. 
2. Generate Time Axis: Create a time vector for the signal duration. 
3. Generate Message Signal: Define the message signal as a cosine wave. 
4. Generate Carrier Signal: Define the carrier signal as a cosine wave. 
5. Modulate Signal: Apply the AM formula to obtain the modulated signal. 
6. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

__Program__:

```
import numpy as np
import matplotlib.pyplot as plt
Am-6.1
fm=486 
Ac=12.2
fc=4860 
fs=48600
t=np.arange(0, 2/fm, 1/fs)
m=Am*np.cos(2*3.14*fm*t) 
plt.subplot(3,1,1)
plt.plot(t,m)
c=Ac*np.cos(2*3.14*fc*t)
plt.subplot(3,1,2) plt.plot(t,c)
s=(Ac+m)*np.cos(2*3.14*fc*t) 
plt.subplot(3,1,3)
plt.plot(t,s)
```

__Tabulation__:

<img width="1156" height="825" alt="image" src="https://github.com/user-attachments/assets/c2d1dd9b-dd6f-4ba0-a78e-3f180806fccd" />


 __Output__:

![WhatsApp Image 2025-11-19 at 12 13 47_491c0fc5](https://github.com/user-attachments/assets/2bb48cb0-5216-4288-bd34-0f45bf09f282)


 __Result__:
Thus the AM Modulation is generated using python and the output is verified.

