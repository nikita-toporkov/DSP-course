 # Lecture 02 – Sampling and Aliasing

## Task 1 – Objective

Sampling of a signal is one of the basics concepts of DSP. There is no perfect Sampling Frequency for all use cases. We have to balance between memory usage (for high Fs) and limits defined by Nyquist theorem (for low Fs). Purpose of this work to simulate range of sampling frequencies to see how they affect sampled signal.

## Task 2 – Nyquist Analysis

Theorem is simple: minimal Fnyquist must be at least 2*Fs_max

For 10 Hz sine wave 2*10 = 20 Hz Fs_min 
For minimally recognisable speach ranged 20-4000 Hz, Fs_min = 2 * 4000 = 8 kHz
Most common sampling frequancies for multimedia quality audio nowdays are 48 kHz and 44.1 kHz, which means that highest frequency that can be reconstructed without aliasing error. 

## Task 3 – Results

Fs = 15 Hz: Sampling lower Fs_nyquist_min - resampled signal points are placed randomly - reconstruction impossible

Fs = 20 Hz: Sampling at Fs_nyquist_min Signal can be recostructed, but there is phase uncertainity (we dont know if signal is shifted for Pi radians.)

Fs = 25 Hz: Sampling at Fs higher than Fs_nyquist_min Signal phase and form can be reconstructed.

Fs = 50 Hz: Sampling at Fs higher than Fs_nyquist_min Signal phase and form can be reconstructed.

Fs = 100 Hz: Sampling at Fs higher than Fs_nyquist_min Signal phase and form can be reconstructed.

## Task 4 – Aliasing Discussion

Aliasing occurs when Fs is lower than Fs_nyquist_min, which causes signal to appear lower frequency.

## Task 5 – Engineering Recommendation

minimal twice as F_signal_max, in reality higher 1,3 - 1,5 * F_signal_max

## Task 6 – AI Usage

AI tools used to generate Matlab code.

Prompts - task description.

Code verified before running. 

Tool: embedded in Matlab copilot.

README fully writen by human, no spellcheck