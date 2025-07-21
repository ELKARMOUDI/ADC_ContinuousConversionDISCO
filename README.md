# STM32F411 Discovery ADC Continuous Conversion

![STM32F411](https://img.shields.io/badge/STM32F411-Discovery-blue)
![ADC](https://img.shields.io/badge/ADC1-Continuous_Conversion-green)

<img src="https://github.com/user-attachments/assets/1c5f149e-c97a-43a6-8326-1c8ed19d3a00" width="400" alt="DBD9D6B7-A318-48B5-8A7A-C28830C08B7C">

<img src="https://github.com/user-attachments/assets/2877509b-9267-4273-860d-7d6bcf11042c" width="400" alt="B5A23937-EAF1-4FA0-B2F3-AAF176D0EEAD">



Read potentiometer values using ADC1 in continuous conversion mode.

## Features
- **Continuous 12-bit ADC** readings
- **PA0 Analog Input** for potentiometer
- **High-Speed Sampling**: 480-cycle sample time


## Hardware Setup
| Component | Connection | Discovery Pin |
|-----------|------------|---------------|
| Potentiometer | VCC → 3.3V | - |
| | GND → GND | - |
| | WIPER → PA0 | CN5 pin 12 (A0) |

## Technical Details
### ADC Configuration 
```c
Clock: 24MHz (48MHz PCLK2 / 2)
Channel: ADC1_IN0 (PA0)
Sampling Time: 480 ADC cycles
Mode: Continuous conversion
