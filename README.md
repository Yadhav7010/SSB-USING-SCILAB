# SSB-T1-C12-EVEN
AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS NEEDED:

.Computer with i3 Processor

.SCI LAB

ALGORITHM:

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x)=sin(x) or any other function.
Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.
Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
Display Results: Output the computed mean variance and Cross Correlation
PROCEDURE:

1.Refer Algorithms and write code for the experiment.

2.Open SCILAB in System

3.Type your code in New Editor

4.Save the file

5.Execute the code If any Error, correct it in code and execute again

6.Verify the generated results

PROGRAM:
```
clc;
clear;
close;
Am=18.1;
Ac=36.2;
fm=646;
fc=6460;
fs=56700;
wm=2*3.14*fm;
wc=2*3.14*fc;
t=0:1/fs:2/fm;
m1=Am*cos(wm*t);
m2=Am*cos(1.57-(wm*t));
subplot(4,1,1);
plot(t,m1);
c1=Ac*cos(wc*t);
c2=Ac*cos(1.57-(wc*t));
subplot(4,1,2);
plot(t,c1);
s1=c1.*m1;
s2=c2.*m2;
Slsb=s1+s2;
subplot(4,1,3);
plot(t,Slsb);
Susb=s1-s2;
subplot(4,1,4);
plot(t,Susb);

```
OUTPUT GRAPH:
<img width="1920" height="1200" alt="Screenshot 2026-03-22 145922" src="https://github.com/user-attachments/assets/0beb777d-3ac4-4954-91d2-c1f2b17cf471" />


RESULT:

