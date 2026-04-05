# SSB-SC

---

## AIM:
To write a program for mean, variance and cross correlation in SCILAB and verify the output.

---

## EQUIPMENTS NEEDED:
- Computer with i3 Processor  
- SCI LAB  

---

## ALGORITHM:

- Define the Function: Specify the function to simulate  
- Generate Sample Points: Decide range and number of points  
- Evaluate the Function: Compute values at sample points  
- Compute Mean, Variance and Cross Correlation  
- Display Results  

---

## PROCEDURE:

1. Refer Algorithms and write code  
2. Open SCILAB in System  
3. Type code in New Editor  
4. Save the file  
5. Execute the code  
6. If any error, correct and execute again  
7. Verify the generated results  

---

## PROGRAM
```scilab
clc;
clear;
close;

Am = 18.1;
Ac = 36.2;
fm = 646;
fc = 6460;
fs = 56700;

wm = 2*3.14*fm;
wc = 2*3.14*fc;

t = 0:1/fs:2/fm;

m1 = Am*cos(wm*t);
m2 = Am*cos(1.57-(wm*t));

subplot(4,1,1);
plot(t,m1);

c1 = Ac*cos(wc*t);
c2 = Ac*cos(1.57-(wc*t));

subplot(4,1,2);
plot(t,c1);

s1 = c1.*m1;
s2 = c2.*m2;

Slsb = s1 + s2;
subplot(4,1,3);
plot(t,Slsb);

Susb = s1 - s2;
subplot(4,1,4);
plot(t,Susb);
```

---

## OUTPUT GRAPH:
<img width="1920" height="1200" src="https://github.com/user-attachments/assets/0beb777d-3ac4-4954-91d2-c1f2b17cf471" />

---

## TABULATION:
<img width="1280" height="896" src="https://github.com/user-attachments/assets/53398b24-4b0c-44c8-acee-158ae197ccf2" />

---

## RESULT:
Thus the mean, variance, and cross-correlation were computed using SCILAB and the results were verified successfully.
<img width="1080" height="458" alt="image" src="https://github.com/user-attachments/assets/5d377831-baee-4642-91db-53cb605fae60" />

