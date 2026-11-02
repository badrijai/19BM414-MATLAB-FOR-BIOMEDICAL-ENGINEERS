## EXPERIMENT 2: EEG Frequency Band Analysis

## AIM
To analyse EEG frequency content and calculate the power in standard EEG bands.

## INPUT
One EEG channel and its sampling frequency. Example: eeg_sample.mat containing eeg and fs = 256 
Hz.

## INPUT FILE / PARAMETERS
File name / model:  eeg_sample.mat

## THEORY / PRINCIPLE
EEG can be analysed in the frequency domain using power spectral density. The spectrum is divided 
into delta, theta, alpha, beta and gamma teaching bands, and numerical integration of PSD estimates the 
power in each band.

## PROCESSING FLOWCHART
<img width="892" height="250" alt="image" src="https://github.com/user-attachments/assets/5174beb5-f8c9-4582-a11b-b8a5a145a5ba" />

## PROCEDURE
1. Load the EEG channel.
2. Remove trend from the signal.
3. Estimate PSD using Welch's method.
4. Define the five frequency bands.
5. Integrate PSD inside each band.
6. Plot absolute and relative band power.
7. Identify the dominant band.

## OBSERVATION
1. Input file = eeg_sample.mat
2. Sampling frequency = 256.00 Hz
3. Signal duration = 30.00 seconds
4. Number of samples = 7680
5. PSD segments averaged = 14

## EEG FREQUENCY BAND RESULTS
1. Delta    Power = 457.692809 | Relative = 22.07%
2. Theta    Power = 201.964913 | Relative = 9.74%
3. Alpha    Power = 1245.939437 | Relative = 60.07%
4. Beta     Power = 126.266577 | Relative = 6.09%
5. Gamma    Power = 42.213408 | Relative = 2.04%

1. Total calculated band power = 2074.077145
2. Dominant frequency band = Alpha
3. Dominant band power = 1245.939437
4. Dominant relative power = 60.07%

## FIGURE 1 - RAW EEG
<img width="773" height="623" alt="Figure 1 2 - Raw EEG" src="https://github.com/user-attachments/assets/cfc84690-7fb3-4422-9f8e-e2dac9feeed8" />

## FIGURE 2 - DETRENDED EEG
<img width="773" height="623" alt="Figure 2 2 - Detrended EEG" src="https://github.com/user-attachments/assets/ef8f8fcc-2577-4b60-8868-89bcdbe6ba02" />

## FIGURE 3 - EEG PSD
<img width="778" height="623" alt="Figure 3 2 - EEG PSD" src="https://github.com/user-attachments/assets/7b7454c3-402a-4c3d-aec3-b460c544a5d5" />

## FIGURE 4 - ABSOLUTE EEG BAND POWER
<img width="768" height="623" alt="Figure 4 2 - Absolute EEG Band Power" src="https://github.com/user-attachments/assets/d95de7c0-dfb5-4975-9a75-8032426c6cd8" />

## FIGURE 5 - RELATIVE EEG BAND POWER
<img width="745" height="623" alt="Figure 5 2 - Relative EEG Band Power" src="https://github.com/user-attachments/assets/e1fd500a-da6a-42b9-9e5e-cc7c41bec5e6" />

## RESULT
The experiment was performed successfully using MATLAB. The input was processed according to the 
stated method and the expected biomedical output was obtained.
