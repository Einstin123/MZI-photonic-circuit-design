MZI photonic circuit design
Design and simulation of MZI photonics circuit.

Status 
The design is sent for OpenEBL call and is awaiting fabrication.

Overview
A Mach-Zehnder-Interferometer takes input of a light, splits it into two paths of different length then recombines them using a coupler. The travelling through different length wave introduces a phase difference.
In my design where two outputs were taken (same merged wave), the outputs followed Port 1: P₁ ∝ cos²(Δφ/2) and Port 2: P₂ ∝ sin²(Δφ/2) respectively.
This photonic component is used in sensors and photonic based neural networks.

My role
I designed MZI using Klayout and SiEPIC library. My main goal for the design was to create enough phase difference to study the results of transmission vs wavelength.
I used 3 grating couplers( one as laser and two as detector), Silicon waveguide in TE mode, and Y - Branch splitter & combiner.

Design specification
Wavelength-1550 nm
Armlength difference- 100.014 um.
Waveguide width- 500nm
Grating couplers: ebeam_gc_te_1550
Y-splitter: ebeam_y_1550
Y-recombiner: ebeam_bdc_te_1550

Layout
<img width="762" height="582" alt="MZI_Layout" src="https://github.com/user-attachments/assets/64107e69-67ae-4808-b407-2aeaf277d6a7" />
The top grating coupler is the laser, the bottom two receive the recombined light.

Simulation results
<img width="800" height="400" alt="Transmission_Wavelength for MZI" src="https://github.com/user-attachments/assets/ce01e257-78fc-4ddd-acb9-302196cd467f" />
Transmission result

Tools used
SiEPIC tools, Klayout, Lumerical

Status and Next steps
Design submitted to the openEBL call.
Once fabricated: experimental transmission results compared to the theoretical results.

