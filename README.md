# AM-USING-PYTHON
---

### Aim:

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries.

---

### Apparatus Required:

- Software: Python with Numpy and Matplotlib libraries.
- Hardware: Personal Computer.

---

### Theory:

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:

   $$ s(t) = [A_c + A_m cos(2\pi f_m t)] cos(2\pi f_c t)$$

---

### Algorithm:

1. Initialize Parameters: Set the values for carrier frequency, message frequency and sampling frequency.
2. Generate Time Axis: Create a time vector for a signal duration.
3. Generate Message Signal: Define the message signal as a cosine wave.
4. Generate Carrier Signal: Define the carrier signal as a cosine wave.
5. Plot the Signals: Use Matplotlib to plot the message signal, carrier  signal and modulated signal.

---

### Program:

```py
import numpy as np
import matplotlib.pyplot as plt
Am=4.5
fm=260
Ac=9.4
fc=2600
fs=26000
t= np.arange(0, 3/fm, 1/fs)

m=Am*np.cos(2*3.14*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)

c=Ac*np.cos(2*3.14*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)

s=(Ac+m)*np.cos(2*3.14*fc*t)
plt.subplot(3,1,3)
plt.plot(t,s)
```

---

### Output Waveform:

<img width="721" height="511" alt="image" src="https://github.com/user-attachments/assets/3bf2b451-c733-44dc-aadb-60466a1b8cac" />

---

### Tabular Column:

![WhatsApp Image 2025-11-24 at 20 17 46](https://github.com/user-attachments/assets/ee8129d8-4b8e-4fac-a14e-518dd3be35a2)

![WhatsApp Image 2025-11-24 at 20 18 09](https://github.com/user-attachments/assets/26a04c9c-937e-45f9-b86d-ff18a9f83869)



---

### Result:

The message signal, carrier signal and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
