# GEOMETRY

## STANDARD
The standard PET detector geometry is **insert diagram**

### MODULE

#### Number of Channels
Increasing solid angle coverage of a detector as a means of increasing sensitivity typically means increasing the number of SiPMs and total volume of scintillation material which increasing the cost of the detector [@daube-witherspoon_scanner_2021]. 

#### Scintillator Length

- Increasing the length of the scintillator increases transit time which decreases timing resolution [@enlow_state_art_2023]

#### Scintillator Thickness

### RING DIAMETER

The average ring diameter for commercial PET scanners is 75 - 90cm [@daube-witherspoon_scanner_2021]. One can increase the solid angle coverage of a detector with the same amount of scintillation material by reducing the ring diameter [@daube-witherspoon_scanner_2021]. This is clearly described with the equation for solid angle coverage:

$$
\Omega = \frac{A}{r^2}
$$

Where $A$ is the total cross sectional area of the detector modules perpendicular to the rings radius and $r$ is the ring radius. If we do not add any new modules to the ring, meaning $A$ remains constant while $r$ decreases then the solid angle coverage, $\Omega$ increases. This is a great way to increase the sensitivity of a detector without increasing the cost. This however, does not come without its disadvantages.

#### Clinical applications

Decreasing the ring diameter reduces clinical applications of the PET scanner to single organ imaging [@daube-witherspoon_scanner_2021;@enlow_state_art_2023]. This is typically brain imaging. 

#### Decreased effective sensitivity

While a decreased ring diameter increases the the solid angle coverage which increases the sensitivity of the detector, there are also other factors that it induces that reduce the effective sensitivity of the scanner. A decreased diameter increases the number of random and scattered events which decreases the number of true events and thus the sensitivity[@daube-witherspoon_scanner_2021]. With each SiPM contributing to a larger portion of the solid angle coverage comes an increase in activity at each SiPM which increases the probability of event pileup and may saturate readout electronics. This leads to loss of events and thus sensitivity.

#### Decreased Spatial Resolution

The angle subtended by coincident pair scintillator pixels becomes larger as the ring diameter decreases. This means that as the ring diameter becomes smaller the exact location of the line of responses between scintillator pixels becomes more ambiguous and reduces the spatial resolution of the scanner. This is best described in the diagram, **insert diagram**. 

If constrained by the number of electronic readout channels and a need for one-to-one coupling. Compensating for this effect means decreasing the width of the SiPMs and scintillator pixels and maintaining the total number of scintillator pixels. This reduces the total solid angle coverage which reduces the sensitivity of the scanner. This simultaneously reduces the cost of the scanner but the significant loss in sensitivity does not justify this cost saving. 

If one is not limited by the number of readout channels, then to compensate for this loss in spatial resolution without a degradation in sensitivity, one may consider taking the same amount of scintillation material and slicing it into thinner scintillator pixels. In order to maintain one-to-one coupling, one must decrease the width of the SiPMs and increase the total number of SiPMs and readout channels. This drastically increases the cost of the scanner.

Thus, to mitigate the effects of decreased spatial resolution due to a decreased ring diameter, one must make a choice between an increased cost or a decreased sensitivity. This choice is often determined by the developers circumstances.

Ignoring this reduction in spatial resolution and simply treating it as a side effect of a decreased cost is a solution that still needs to be investigated. The question is whether not reducing the scintillator pixel width in order to maintain sensitivity and reduce cost degrades the final image enough to justify utilizing the above solutions. 

#### Parallax Error

Annihilation events that occur at the center of the ring produce photons that enter the scintillator pixels at the faces opposite to those coupled to the SiPMs (the square face). Annihilation events that occur towards the edge of the ring produce photons that enter scintillator pixels at their lateral sides. The angle subtended by the lateral sides of scintillator pixels is much larger than that of the square faces. This means that the exact position of the line of responses is far worse for events occurring towards the edge of the ring, reducing the spatial resolution of the final image. This effect is best describe using a diagram, as seen in, **insert diagram**. This effect is commonly known as parallax error. The amount of events occurring towards the edge of the edge of the ring increases as the ring diameter decreases, depending on the subject being imaged. Thus, as the ring diameter becomes smaller, degradations in spatial resolution due to parallax error becomes more prominent. [@daube-witherspoon_scanner_2021;@enlow_state_art_2023].

### AXIAL LENGTH
Most scanners have a standard axial length of 15-26cm [@el_ouaridi_detection_2024;@daube-witherspoon_scanner_2021]. To create a full body image, the patient is displaced along the axis to image the entire body. This requires 8-10 overlapping bed positions for 10-20 minutes at 370-555 MBq of FDG [@daube-witherspoon_scanner_2021]. A large percentage of the photons are lost. Thus, there has been a growing interest in long axial FOV scanners as a means to increase sensitivity [@el_ouaridi_detection_2024]. 

#### Advantages of Long AFOV [@el_ouaridi_detection_2024]

- reduction in acquisition time
- dynamic whole-body imaging
- parametric imaging

The huge downside of a long AFOV scanning is that it drastically increases the cost [@el_ouaridi_detection_2024]. This increase in cost has pushed the industry leaders to start optimizing for lower cost. These cost saving strategies can then be implemented in an ultra-low-cost short AFOV scanner. Some of the methods being explored include reducing the length of scintillator pixels by half, using sparsely filled detectors and reverting back to BGO [@el_ouaridi_detection_2024].

## OTHER

### Planer

## MODULE POSITIONING