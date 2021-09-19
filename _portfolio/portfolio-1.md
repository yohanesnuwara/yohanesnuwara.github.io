---
title: "Distributed Acoustic Sensing for Seismic Monitoring in Chiba, Japan"
excerpt: "Y. Nuwara¹, T. Miyoshi¹, Z. Xue¹, T. Hashimoto¹, T. Nakajima¹<br>¹Research Institute of Innovative Technology for the Earth, Kyoto, Japan<br><br>Full DAS optical fiber record of an earthquake occurring in the Bōsō Peninsula in 20 February 2020 at 06:33 UTC+0<br><img src='https://user-images.githubusercontent.com/51282928/133879799-2d7a276d-7e0a-42b0-b4e9-8593cc79374c.png'>"
collection: portfolio
---

This project was done in RITE during the COVID-19 pandemic of 2021. I was involved in the CO2 Storage Group led by Dr. Ziqiu Xue. In August, I was given the opportunity to [present this research]() in a workshop organized by the Incorporated Research Institutions for Seismology (IRIS) in USA. It was expected that our research could set a new direction for utilizing DAS to monitor seismic activities in Japan. 

Three DAS optical fiber cables were installed down-hole; two cables are straight cables in a 250-meter well and 880-meter well, and one cable is helical in the 250-meter well. Figure below shows the vertical section of our installed cables and Silixa iDAS interrogator in Chiba. Notice there is a difference between cables installed in the 250-meter and 880-meter well. For the straight (STC) and helical cables (HWC) in the 250-meter well, they were installed along the cement (thus denoted as STC250 and HWC250). For the straight cable in the 880-meter well, it was installed behind casing (thus denoted as HWC880).

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133917561-3dd01572-8bfd-4bcc-b4dd-28dc9d429816.png" alt="drawing" width="500"/>
</p>

With DAS, we recorded continuous seismic records of natural earthquakes. At least, we could identify different wave types in the record as shown below.

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133917640-7fd6d8e7-cbe9-419e-a370-a8308f85a876.png" alt="drawing" width="500"/>
</p>

First, we compared the waveform response of each of the three DAS configurations (STC250, HWC250, and HC880) to the natural earthquakes. Shown below are the waveform displays of each DAS. There is a small difference between the straight cables STC250 and BC880, but notice less occurrence of multiples in BC880 as shown by the yellow arrow. The straight cables show stronger and clearer amplitude response but noisier compared to the helical cable HWC250.   

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133917570-31478991-a945-46df-810c-27ac0b8a6330.png" alt="drawing" width="400"/>
</p>

We zoomed in the portion of the records that show P-wave arrival as shown in the two figures below. The noise at near-surface appears in STC250 and BC880 at depth below 50 m. The characteristics of this noise are very strong amplitudes, low frequency, and random. This is likely the noise caused by the strong amplification of ground motion. The HWC250 does not show this noise too much at the same depth. However, notice the amplitude reduction in the HWC250 record between depth of 30 and 80 meter. The cause of this reduction is still unknown. 

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133892087-79dec62a-b4ef-499e-b022-ba2e8886b940.png" alt="drawing" width="600"/>
</p>

Next, we implemented automated picking technique to pick P-wave and S-wave arrivals using four methods; Kurtosis, Short-Term Average/Long-Term Average (STA/LTA), Akaike Information Criterion (AIC), and Short-Time Fourier Transform (STFT). In general, we favored STA/LTA method because the computation is speedy. Later we found that Kurtosis and AIC result more peaking values at the arrivals and their ability to distinguish the upgoing and downgoing arrivals although they take longer time to compute. STFT is able to identify P-wave and S-wave arrivals comparably fast because it is based on frequency-based Fourier transform. Shown below are the results of STA/LTA and STFT for automated PS picking.

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133892106-f109d92d-ec0a-4a5b-af00-e46a42d85747.png" alt="drawing" width="600"/>
</p>

We made a waterfall plot of frequency vs. depth with spectral amplitude as color to identify different types of noise in the data. Shown below is the waterfall plot for each DAS. We could identify at least four key frequencies; ~5 Hz is background noise, ~10 and ~15 Hz are the signals (P or S), and ~30 Hz is completion noise. We also found an interesting observation of unique stripe patterns forming acute angle in the f-z plot which exists in shallow part of BC880. Our interpretation is that this noise is likely caused by poorly cemented (completion) part of the well. Therefore, the shallower part of below 400 m appears to be poorly cemented. In addition, there are horizontal stripes which are likely the optical noise. 

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133892140-c2dad67e-9500-46a2-b89f-cab22584925d.png" alt="drawing" width="600"/>
</p>

Finally, we found an interesting observation on the dependence of DAS detectability on azimuth and incidence angle, as shown in the figure below. It is evident that DAS can detect natural earthquakes with magnitude down to 0.8! Interestingly, the 0.8-magnitude record has weaker amplitude of P-wave arrival than larger 1.3 and 1.4-magnitude. When we plotted in the azimuth-incidence angle polar plot and correlated with the map of the Japanese Bōsō Peninsula, the 0.8-magnitude earthquake is located in azimuth near 270 degrees (in Kujukuri) and the larger earthquakes are in azimuth near 0 degree (in Bōsō). The difference in azimuthal dependency is most likely caused by the velocity anisotropy in the subsurface. 

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/133918585-ed873173-8bc4-4c8b-938c-117d06314ffa.png" alt="drawing" width="600"/>
</p>
