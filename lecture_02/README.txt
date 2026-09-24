downsampling_7kHz.mlx - live script that shows how downsampling works. LOWER VOLUME BEFORE RUNNING!
downsampling_gong_handel.mlx works the same, but uses built-in Matlab sounds.

1. Which sampling frequencies represented the 7 kHz signal correctly?

    Accordin to Nyquist  theorem, sampling frequency must be at least twice higher as the highes frequency of the signal. Therefore 7kHz signal can be represented correctly with lowes sampling frequency of 14kHz.

2. When did the 7 kHz signal appear as another frequency?

    If the sampling rate is lower than 14kHz alliasing causes pitch to shift. 

3. What happened when the Nyquist frequency became lower than 7 kHz?

    Aliasing error happens.

4. Did the aliased signal sound different?

    It has pitch shifted down and missing high frequency components.

5. Why can MATLAB not recover the original 7 kHz signal after aliasing?

    MATLAB cannot recover the original 7 kHz signal because aliasing permanently loses information during sampling. Once the sampling frequency is too low, the 7 kHz signal becomes indistinguishable from a lower-frequency alias, so MATLAB cannot determine which frequency was originally present.