# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 

```
clc;
clear;
clf;

xn = [1,2,3,4,4,3,2,1];
N = length(xn);
n = 0:N-1;

Xk = fft(xn);

disp("FFT output:");
disp(Xk);

K = 0:N-1;
magnitude = abs(Xk);
phase = atan(imag(Xk), real(Xk));

y = ifft(Xk);

subplot(2,2,1);
plot2d3(n, xn);
xtitle("Input Sequence", "n", "x(n)");

subplot(2,2,2);
plot2d3(K, magnitude);
xtitle("Magnitude Spectrum", "k", "|X(k)|");

subplot(2,2,3);x
plot2d3(K, phase);
xtitle("Phase Spectrum", "k", "Phase (radians)");

subplot(2,2,4);
plot2d3(n, real(y));
xtitle("Inverse FFT Output", "n", "x(n)");
```

### DFT FFT-ALGORITHM



### CALCULATIONS:

<img width="1280" height="1254" alt="WhatsApp Image 2026-11-10 at 2 02 44 PM" src="https://github.com/user-attachments/assets/d7f08d4d-26cf-43a0-a8ff-a82047b25d47" />

<img width="771" height="1280" alt="WhatsApp Image 2026-11-10 at 2 02 44 PM (1)" src="https://github.com/user-attachments/assets/fd97d96c-378e-44de-b06e-89d9ab270614" />

 <img width="773" height="1280" alt="WhatsApp Image 2026-11-10 at 2 02 44 PM (2)" src="https://github.com/user-attachments/assets/8aaa1c8b-7ae4-4077-a7bd-3e952835a275" />

<img width="801" height="1280" alt="WhatsApp Image 2026-11-10 at 2 02 44 PM (3)" src="https://github.com/user-attachments/assets/53282058-cd85-449b-9ead-a9b2c155b59b" />

### SAMPLE OUTPUT:

<img width="1599" height="1513" alt="WhatsApp Image 2026-11-10 at 11 00 31 AM" src="https://github.com/user-attachments/assets/3707be8e-f584-4d63-8a75-4a3d04bb9e87" />

### RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

