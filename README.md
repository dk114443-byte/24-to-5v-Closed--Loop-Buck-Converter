# 24V to 5V Closed-Loop Buck Converter

## Project Overview
This project focuses on the design and simulation of a DC-DC buck converter that steps down a 24V DC input to a regulated 5V DC output using LTspice.

A PI-based feedback controller and PWM generation circuit are used to control the output voltage.

## Design Specifications

| Parameter | Value |
|---|---:|
| Input Voltage | 24V DC |
| Input Test Range | 18V–30V |
| Target Output Voltage | 5V DC |
| Rated Output Current | 1A |
| Rated Output Power | 5W |
| Switching Frequency | 100kHz |
| Inductor | 150µH |
| Output Capacitor | 22µF |
| Input Capacitor | 47µF |
| Load Resistance | 5Ω |

## Working Principle

The buck converter uses high-frequency switching to reduce the input DC voltage.

The PWM signal controls the switching element. The inductor and capacitor filter the switched voltage to produce a DC output.

The PI controller compares the feedback voltage with the reference voltage and adjusts the PWM duty cycle.

## Tools Used
- LTspice
- Microsoft Word
- GitHub

## Project Files
- `Buck_Converter.asc` – LTspice circuit schematic.
- `Buck convertor Design Calculations.docx` – Design calculations.
- Simulation screenshots – Input, output and PWM waveforms.

## Simulation Results

| Test Condition | Observed Output |
|---|---:|
| 24V input, 5Ω load | Approximately 4.7V |
| 18V input, 5Ω load | Approximately 4.7V |
| 30V input, 5Ω load | Approximately 4.69V |
| 24V input, 10Ω load | Approximately 4.56V |

Note: These are simulation observations. The design has not yet achieved exact 5V regulation under all tested conditions.

## Future Improvements
- Replace the ideal switching element with a MOSFET model.
- Implement an op-amp-based PI controller.
- Add a suitable MOSFET gate driver.
- Design a PCB using KiCad.
- Build and test a hardware prototype.

## Author
Dinesh Kumar V

Electrical and Electronics Engineering
