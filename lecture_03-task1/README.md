# Discrete-Time Signal Operations and Convolution

## Q&A

### Which operation changed the signal amplitude?

Adding noise to original sine wave changed it's amplitude.

### How did the five-sample delay change the signal?

Five sample delay smoothed signal's, removed some noise by averaging values withing short 5-n length window. It has also taken some amplitude for n = 15.
What does the impulse response

### h[n] represent?

Impulse response 

### How did convolution change the noisy signal?

Moving Average filter is a type of convolution. Low pass filter that reduces high frequency noise and passing low frequency signal.

### What differences did you observe between the 5-point and 15-point filters?

Switching from 5 points to 15 points window moved Fcut_off closer to 0, which caused Signal amplitude reduction.

### Which filter removed more noise?

15-point filter as it reduced wider spectrum of noisy high frequencies.

### Did the longer filter remove or distort useful signal information?

Reduced amplitude.

### Which filter would you recommend for this signal? Explain your decision.

5 point filter, as it has not reduced signal's amplitude and removed noise.

### Give one real engineering application for moving-average filtering.

Signal noise reduction for audio application. Sensor readings. This filter is the easiest filter to implement. It also has Finite Impulse Response.