## EXPERIMENT 1: ECG Noise Removal and QRS Detection

## AIM:
To remove noise from an ECG signal and detect QRS complexes using MATLAB.

## INPUT
One ECG waveform and sampling frequency. Example: ecg_sample.mat containing ecg and fs = 360 
Hz.

## INPUT FILE / PARAMETERS
File name / model: ecg_sample.mat

## THEORY / PRINCIPLE
ECG contains characteristic P, QRS and T waves and may be contaminated by baseline wander, power
line interference and high-frequency noise. A band-pass filter is used to emphasize QRS energy. 
Differentiation, squaring and moving-window integration further enhance the QRS complexes before 
peak detection.

## PROCESSING FLOWCHART
<img width="772" height="218" alt="image" src="https://github.com/user-attachments/assets/a149772e-473f-40fe-91b3-7718fb9f247c" />

## PROCEDURE
1. Load the ECG and inspect its duration and amplitude.
2. Remove the DC component.
3. Design and apply a 5–15 Hz Butterworth band-pass filter.
4. Differentiate and square the filtered ECG.
5. Apply a 150 ms moving-window integration.
6. Detect QRS candidates using minimum height and minimum distance.
7. Calculate RR intervals and estimated heart rate.

## OBSERAVATION
1. Sampling frequency = 360 Hz
2. Signal duration = 10.00 seconds
3. Original simulated heart rate = 75 bpm
4. Detected QRS candidates = 12
5. Mean RR interval = 0.7980 seconds
6. Estimated heart rate = 75.19 bpm

## FIGURE 1 - RAW ECG
<img width="767" height="623" alt="Figure 1 - Raw ECG" src="https://github.com/user-attachments/assets/dc0ef296-46b2-42b9-8e23-627017c2c7e8" />

## FIGURE 2 - FILTERED ECG
<img width="767" height="623" alt="Figure 2 - Filtered ECG" src="https://github.com/user-attachments/assets/54d8c172-6892-4b2f-9f5c-f6ca0e151b18" />

## FIGURE 3 - QRS ENHANCEMENT
<img width="743" height="624" alt="Figure 3 - QRS Enhancement" src="https://github.com/user-attachments/assets/f2225313-4a16-4d36-ba78-c477fda84674" />

# FIGURE 4 - QRS DETECTION
<img width="767" height="623" alt="Figure 4 - QRS Detection" src="https://github.com/user-attachments/assets/81024c6d-055f-4767-8aec-6910f4c79d08" />

## RESULT
The experiment was performed successfully using MATLAB. The input was processed according to the 
stated method and the expected biomedical output was obtained.



