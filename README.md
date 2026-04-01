# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM:
DHATCHAYANI R 212224050006
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending of y(n)');
n1=b:1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')
% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')
% DISCRETE CROSS CORRELATED SIGNAL
out2=xcorr(x,y);
n3=a-m:1:length(out2)+a-m-1;
figure(4)
stem(n3,out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')
```

## OUTPUT:
<img width="1134" height="950" alt="image" src="https://github.com/user-attachments/assets/662ded2f-2132-4887-b17a-ebbaea6757e3" />
<img width="831" height="862" alt="image" src="https://github.com/user-attachments/assets/e30f326f-d10f-4b70-bb25-18245972798d" />


## RESULT:
![WhatsApp Image 2026-04-01 at 12 05 56 PM](https://github.com/user-attachments/assets/f157418b-8527-43d9-b3c2-6b33d829c993)


