# GEOMETRY

## STANDARD
The standard PET detector geometry is 

### MODULE

#### Number of Channels
Increasing solid angle coverage of a detector as a means of increasing sensitivity typically means increasing the number of SiPMs and total volume of scintillation material which increasing the cost of the detector [@daube-witherspoon_scanner_2021]. 

#### Scintillator Length

#### Scintillator Thickness

### RING DIAMETER

The average ring diameter for commercial PET scanners is 75 - 90cm [@daube-witherspoon_scanner_2021]. One can increase the solid angle coverage of a detector with teh same amount of scintillation material by reducing the ring diameter [@daube-witherspoon_scanner_2021]. This is clearly described with the equation for the solid angle coverage:

$$
\Omega = \frac{A}{r^2}
$$

Where $A$ is the total cross sectional area perpendicular to the rings radius of the detector modules and $r$ is the ring diameter. If we do not add any new modules to the ring and $A$ remains constant while $r$ decreases then the solid angle coverage, $\Omega$ increases. This is a great way to increase the sensitivity of a detector without increasing the cost.

This however, does not come without its disadvantages:

- Reduces clinical applications [@daube-witherspoon_scanner_2021;@enlow_state_art_2023]
- Increased detection of random and scattered events. Decreases the SNR. [@daube-witherspoon_scanner_2021]
- Degradations in spatial resolution due to parallax error. [@daube-witherspoon_scanner_2021;@enlow_state_art_2023]

### AXIAL LENGTH
Most scanners have a standard axial length of 15-26cm [@el_ouaridi_detection_2024;@daube-witherspoon_scanner_2021]. Patient is displaced along the axis to image the entire body. This requires 8-10 overlapping pbed positions for 10-290 minutes at 370-555 MBq of FDG [@daube-witherspoon_scanner_2021]. A large percentage of the photons are lost. There has been a growing interest in long axial FOV scanners [@el_ouaridi_detection_2024]. 

#### Advantages of Long AFOV [@el_ouaridi_detection_2024]

- reduction in acquisition time
- dynamic whole-body imaging
- parametric imaging

The huge downside of a long AFOV camera is that is drastically increases the cost [@el_ouaridi_detection_2024]. This increase in cost has pushed the industry leaders to start optimizing for lower cost. These cost saving strategies can then be implemented in an ultra-low-cost short AFOV scanner. Some of the methods being expplored include reducing the length of scintillator pixels by half, using sparsely filled detectors and reverting back to BGO [@el_ouaridi_detection_2024].

#### Pixelated Arrays
Most detectors are made with long thin pixellated scintillators coupled to photodetectors at their extremities [@el_ouaridi_detection_2024]. All the pixels are optically separated using some reflective material [@el_ouaridi_detection_2024].

##### Disadvantages

- variation in scintillation light collection efficency [@el_ouaridi_detection_2024]
- variations in light transmit time to detector [@el_ouaridi_detection_2024]
- light undergoes various reflections within scintillator array [@el_ouaridi_detection_2024]
- increases parallax effects [@el_ouaridi_detection_2024]
These disadvantages can be mitigated by optimizing reflector and lateral surface finishes of scintillator pixels [@el_ouaridi_detection_2024]

##### Coupling Ratio
The typical approach is to have a one-to-one ratio between the number of SiPMs and scintillator pixels. Meaning that each SiPM reads the light from a single scintillator pixel. Some design take teh approach of coupling more than one scintillator pixel to a single SiPM [@pizzichemi_new_2016;@wang_development_2022;@wang_evaluation_2021;@zatcepin_improving_2020-1;@pizzichemi_light_2019]. The light output by a scintillator pixel is spread across multiple SiPMs via a light guide [@daube-witherspoon_scanner_2021]. The center of the light distribution determines the scintillator pixel that the original 511keV photon interacted with [@el_ouaridi_detection_2024]. This method is known as Anger Logic and is borrowed from older PET detectors that used large PMTs coupled to scintillator arrays [@daube-witherspoon_scanner_2021] 

The benefit of coupling multiple smaller scintillator pixels to a single SiPM is that you decrease the thickness of the scintillator pixels without requiring more smaller SiPMs to read them out. While larger SiPMs are slightly more expensive than smaller crystals, reading out some fixed number and size of scintillator pixels with less larger SiPMs is more cost effective than with more smaller SiPMs. As the scintillator width becomes increasingly small, one-to-one coupling becomes increasingly more difficult due to mechanical tolerances.

#### Monolithic Arrays
A continuous thick block of scintillation material is coupled to an array of SiPMs on one of its 6 sides.

##### Advantages

- Good sensitivity [@el_ouaridi_detection_2024]
- Innate DOI encoding [@el_ouaridi_detection_2024]
- High intrinsic spatial resolution [@el_ouaridi_detection_2024]
- Lower manufacturing cost [@el_ouaridi_detection_2024]

##### Disadvantages

- Sophisticated algorithms and calibration required [@el_ouaridi_detection_2024]
- Each deposited 511keV photon triggers every SiPM which can quickly overwhelm the acquisition hardware and cause pileup. Lost events.

## OTHER

### Planer

## MODULE POSITIONING