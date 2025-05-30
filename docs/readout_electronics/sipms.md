# PHOTODETECTORS

## MOVE AWAY FROM PMT
Photo Multiplier Tubes (PMTs) were the main choice for photodetectors before SiPMs [@el_ouaridi_detection_2024]
This is because of their [@el_ouaridi_detection_2024]:

- high gain
- low noise
- fast response time

SiPMs began to be the favorable over PMTs because of their [@el_ouaridi_detection_2024]:

- fragility
- large volumes
- high operating voltage
- sensitivity to magnetic fields

## SIPMS

SiPMs are made up of an array of SPADs. The amount of SPADs that are triggered creates a current signal that is proportional to the amount of scintillation light that hit the SiPM. However, if there is more scintillation photons than SPADs then the proportionality of the output current is lost [@enlow_state_art_2023]

### HOW DO THEY WORK?

### BENEFITS OVER PMTs

- More compact [@enlow_state_art_2023]
    - one-to-one coupling with scintillator pixels increases light collection while maintaining spatial resolution [@el_ouaridi_detection_2024;@daube-witherspoon_scanner_2021;@daube-witherspoon_scanner_2021]
    - increases geometric freedom
- Insensitive to magnetic fields [@el_ouaridi_detection_2024;@enlow_state_art_2023]
- High gains equivalent to PMTs [@el_ouaridi_detection_2024]
- High detection efficiency [@daube-witherspoon_scanner_2021]
- Relatively low cost [@daube-witherspoon_scanner_2021]

### TYPICAL COMMERCIALLY AVAILABLE SIPM PARAMETERS

| Parameter               | Standard Values             |
|-------------------------|-----------------------------|
| SiPM Widths (mm)        | 1, 3, 4, 6                  |
| Array Sizes (Pixels)    | 4, 16, 64, 144              |
| Microcell Sizes (µm)    | 10, 20, 35                  |


### SiPM ARRAYS

A SiPM array is a set of SiPMs that is arranged on a single PCB with a single pin connector that facilitates the connection between many SIPMs and the readout electronics.

#### COMMERCIAL
Companies like Broadcom, Hammamatsu and Onsemi populate PCBs with their SiPMs to create square SiPM arrays of varying sizes.

Advantages:

- Very little development time.
- Makes open-source detector design more accessible to others.
- Reliability
- Manufacturer support
- Producers of SiPMs have control over the manufacturing allowing them to create arrays maximized active area

Disadvantages:

- Standard sizes that limit geometric freedom
- Not all available SiPMs have a corresponding commercial SiPM array which limits you SiPM choice
- Standard pin connectors that may require adapter boards to connect to chosen acquisition hardware

#### CUSTOM

An alternative to buying a commercial SiPM array is to design a custom PCB and populate the PCB with the SiPM of choice.

Advantages:

- Control over mechanical footprint provides geometric freedom. (e.g non-square arrays)
- Increases SiPM choice
- Opportunity to explore different light sharing schemes as a means to reduce the amount of SiPMs and thus cost.

Disadvantages:

- Long development times.
- Decreased availability to other interested parties.
- Manufacturing complexities.
- More costly unless SiPMs are bought at scale.
- Varying availability of individual SiPMs across distributors

Cost of an individual SiPM is dependent on the amount of SiPMs bought and the package type they are sold in. SiPMs can be bought in a Tape Reel (min 3000) or on a Tape (min 1). Price per SiPM is much cheaper for TR but have to buy 3000. Some distributors buy a TR and cut them to customers desired number (price per SiPM varies based on amount cut from the original TR).

#### COMMERCIAL VS CUSTOM COST

### SIZE