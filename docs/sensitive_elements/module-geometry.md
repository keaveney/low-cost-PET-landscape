# MODULE GEOMETRY

## Pixelated Arrays
Most detectors are made with long thin pixellated scintillators coupled to photodetectors at their extremities [@el_ouaridi_detection_2024]. All the pixels are optically separated using some reflective material [@el_ouaridi_detection_2024].

The spatial resolution of a pixellated detector module is related to the width of the pixellated crystal and is often estimated to be half the width of a single scintillator pixel [@enlow_state_art_2023]. 

### Advantages

### Disadvantages

- variation in scintillation light collection efficency [@el_ouaridi_detection_2024;@enlow_state_art_2023]
- variations in light transmit time to detector [@el_ouaridi_detection_2024]
- light undergoes various reflections within scintillator array [@el_ouaridi_detection_2024]
- increases parallax effects [@el_ouaridi_detection_2024]

#### Scintillator Length

- Increasing the length of the scintillator increases transit time which decreases timing resolution [@enlow_state_art_2023]

#### Scintillator Thickness

These disadvantages can be mitigated by optimizing reflector and lateral surface finishes of scintillator pixels [@el_ouaridi_detection_2024]

### Coupling Ratio
The typical approach is to have a one-to-one ratio between the number of SiPMs and scintillator pixels. Meaning that each SiPM reads the light from a single scintillator pixel. Some designs take the approach of coupling more than one scintillator pixel to a single SiPM [@pizzichemi_new_2016;@wang_development_2022;@wang_evaluation_2021;@zatcepin_improving_2020-1;@pizzichemi_light_2019]. The light output by a scintillator pixel is spread across multiple SiPMs via a light guide [@daube-witherspoon_scanner_2021]. The center of the light distribution across the affected SiPMs determines the scintillator pixel that the original 511keV photon interacted with [@el_ouaridi_detection_2024]. This method is known as Anger Logic and is borrowed from older PET detectors that used large PMTs coupled to scintillator arrays [@daube-witherspoon_scanner_2021] 

The benefit of coupling multiple smaller scintillator pixels to a single SiPM is that you decrease the width of the scintillator pixels without requiring more smaller SiPMs to read them out. One could also maintain the scintillator pixel width and increase the SiPM size to reduce the number of SiPMs and readout channels while maintaining the same amount of scintillation material, reducing cost and maintaining sensitivity [@daube-witherspoon_scanner_2021]. While larger SiPMs are slightly more expensive than smaller SiPMs, reading out some fixed number and width of scintillator pixels with less larger SiPMs is more cost effective than with more smaller SiPMs. As the scintillator width becomes increasingly small, one-to-one coupling becomes increasingly more difficult due to mechanical tolerances, which puts a physical limit on the minimum scintillator pixel width for one-to-one coupling. An increased coupling ratio reduces this minimum width.

This approach does not come without its problems. The light collection at each SiPM is reduced and the signals present at each SiPM is much smaller [@daube-witherspoon_scanner_2021]. These effects may lead to lost events and a decrease in sensitivity. The amount of SiPMs that are affected by a single event increases, which increases the likelihood of pileup and may lead to lost events, decreasing the sensitivity [@daube-witherspoon_scanner_2021].

## Monolithic Arrays
A continuous thick block of scintillation material is coupled to an array of SiPMs on one of its 6 sides.

### Advantages

- Good sensitivity [@el_ouaridi_detection_2024]
- Innate DOI encoding via light distribution [@el_ouaridi_detection_2024;@enlow_state_art_2023]
- High intrinsic spatial resolution [@el_ouaridi_detection_2024]
- Lower manufacturing cost [@el_ouaridi_detection_2024]

### Disadvantages

- Sophisticated algorithms and calibration required [@el_ouaridi_detection_2024;@enlow_state_art_2023]
- Each deposited 511keV photon triggers every SiPM which can quickly overwhelm the acquisition hardware and cause pileup. Lost events.
- The spatial resolution degrades as teh length of the monolithic block increases [@enlow_state_art_2023]. Need to balance spatial resolution with sensitivity.

There has been success cutting guides into monolithic blocks using lasers to create optical barriers that guide light over the photosensors to mitigate these disadvantages [@enlow_state_art_2023]
