# STM32F411 Discovery ADC Continuous Conversion

![STM32F411](https://img.shields.io/badge/STM32F411-Discovery-blue)
![ADC](https://img.shields.io/badge/ADC1-Continuous_Conversion-green)

Read potentiometer values using ADC1 in continuous conversion mode.

## Features
- **Continuous 12-bit ADC** readings
- **PA0 Analog Input** for potentiometer
- **High-Speed Sampling**: 480-cycle sample time
- **96MHz System Clock** (HSI-based PLL)

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
