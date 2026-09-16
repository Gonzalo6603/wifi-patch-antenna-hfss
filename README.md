# Wi-Fi Patch Antenna Simulation in Glass using Ansys HFSS

Simulation study of 2.4 GHz microstrip patch antennas integrated with glass substrates using Ansys HFSS.

The project evaluates how the dielectric environment affects antenna performance by comparing different configurations based on resonance frequency, reflection coefficient (S11), gain, directivity, and radiation pattern.

## Project Overview

Modern buildings increasingly use glass in walls and facades, which can affect wireless signal propagation and antenna behavior.

This project investigates the electromagnetic impact of integrating Wi-Fi patch antennas with glass by comparing three configurations:

1. Patch antenna on FR4 in air
2. Patch antenna on glass in air
3. Patch antenna on FR4 embedded in glass

Two antenna geometries were evaluated:

- Circular patch antenna
- Rectangular patch antenna

## Tools

- Ansys HFSS
- Electromagnetic simulation
- Microstrip patch antenna design
- 2.4 GHz Wi-Fi band

## Simulation Parameters

The models were simulated using:

- Open boundary conditions
- Coaxial port excitation
- Adaptive mesh refinement
- Frequency sweep around the 2.4 GHz Wi-Fi band

The main evaluated parameters were:

- Resonance frequency
- Reflection coefficient (S11)
- Maximum gain
- Directivity
- Radiation pattern

## Key Results

### Rectangular Patch Antenna

| Configuration | Resonance Frequency | S11 Minimum | Maximum Gain |
|---|---:|---:|---:|
| FR4 in air | 2.49 GHz | -26.27 dB | 7.24 dBi |
| Glass in air | 2.14 GHz | -7.70 dB | 3.25 dBi |
| FR4 embedded in glass | 2.495 GHz | -29.40 dB | 6.66 dBi |

The glass substrate produced a significant shift in resonance frequency and a reduction in antenna gain.

The FR4 antenna embedded in glass preserved performance closer to the original FR4 configuration, showing that the integration method strongly affects electromagnetic behavior.

### Circular Patch Antenna

| Configuration | Resonance Frequency | S11 Minimum | Maximum Gain |
|---|---:|---:|---:|
| FR4 in air | 2.418 GHz | -29.11 dB | 3.07 dBi |
| Glass in air | 2.179 GHz | -11.00 dB | 3.97 dBi |
| FR4 embedded in glass | 2.139 GHz | -31.98 dB | 2.60 dBi |

## Engineering Insights

The simulations showed that the dielectric environment has a strong influence on antenna behavior.

Key observations:

- Glass can shift the antenna resonance frequency.
- Changes in dielectric properties affect impedance matching.
- Gain and radiation patterns vary depending on how the antenna is integrated with glass.
- Antenna geometry may need to be retuned when changing the surrounding dielectric material.

These results highlight the importance of considering material properties during antenna integration in architectural environments.

## Limitations

This project was based entirely on electromagnetic simulation.

No physical prototype or experimental antenna measurements were performed.

Therefore, the results should be interpreted as simulation-based evidence rather than experimental validation.

## Future Work

Possible extensions of the project include:

- Retuning antenna dimensions to restore resonance at 2.4 GHz
- Parametric optimization of patch geometry
- Evaluation of different glass thicknesses
- Experimental fabrication and validation
- Comparison between simulated and measured S11
- Analysis of radiation efficiency

## Repository Structure

```text
wifi-patch-antenna-hfss/
│
├── README.md
├── report/
│   └── technical-report.pdf
├── figures/
│   ├── circular-patch/
│   └── rectangular-patch/
├── results/
│   ├── s11/
│   ├── gain/
│   └── radiation-patterns/
└── hfss/
    └── simulation-files/
```

## Authors

- Gonzalo Vargas Huamán
- Diego Uchasara Huarachi

**Electronic Engineering**  
Universidad de Ingeniería y Tecnología (UTEC)

## Academic Context

Originally developed as part of an Electronic Engineering integration project at UTEC.

The repository has been reorganized as a technical portfolio project focused on electromagnetic simulation and antenna performance analysis.
