# DR-003 — Development Board Selection

**Document ID:** DR-003  
**Status:** Approved  
**Date:** July 19, 2026  
**Author:** Miller Sykes

## 1. Purpose

Select the initial STM32 development board for Project Aegis.

## 2. Requirements

The selected board shall:

- Use an STM32 microcontroller.
- Include an integrated debugger and programmer.
- Provide access to UART, SPI, I²C, CAN, ADC, DAC, and timer peripherals.
- Support STM32CubeIDE and the STM32Cube software ecosystem.
- Provide enough processing capability for future control, telemetry, sensor-processing, and RTOS development.
- Allow external hardware expansion.
- Remain reasonably priced and readily replaceable.

## 3. Candidates Considered

### NUCLEO-G474RE

**Advantages**

- Arm Cortex-M4 processor operating at up to 170 MHz
- Floating-point and DSP support
- Strong analog, timer, and communication peripherals
- CAN FD support
- Integrated ST-LINK debugger and programmer
- Arduino Uno V3 and ST morpho expansion connectors
- Well suited for control and sensor-processing applications

**Disadvantages**

- More complex than an entry-level STM32 board

### NUCLEO-F446RE

**Advantages**

- Mature and widely used STM32 platform
- Strong documentation and community support
- Integrated ST-LINK debugger and programmer
- Good general-purpose peripheral set

**Disadvantages**

- Older microcontroller family
- Less capable analog and control-oriented peripheral set than the STM32G474RE

### NUCLEO-H563ZI

**Advantages**

- High processing capability
- Large memory and extensive peripherals
- Suitable for advanced embedded applications

**Disadvantages**

- Greater cost and complexity
- More capability than required for the initial project phases
- Less appropriate for learning foundational concepts before moving to higher-performance devices

## 4. Decision

Project Aegis will use the **STM32 NUCLEO-G474RE** as its initial development board.

## 5. Rationale

The NUCLEO-G474RE provides the best balance of professional relevance, processing capability, peripheral support, expansion capability, and cost.

Its STM32G474RE microcontroller provides sufficient performance for sensor acquisition, telemetry, control systems, fault monitoring, communication protocols, and future RTOS development. The integrated ST-LINK debugger and programmer eliminates the need for a separate debugging probe, while the Arduino Uno V3 and ST morpho connectors provide convenient access to external hardware.

The board provides enough capability to support long-term project growth without introducing the unnecessary complexity of a higher-performance STM32H5 or STM32H7 platform. ST currently lists the NUCLEO-G474RE as an active, volume-production product. :contentReference[oaicite:0]{index=0}

## 6. Revision History

| Version | Date | Description |
|---|---|---|
| 1.0 | July 19, 2026 | NUCLEO-G474RE selected as the initial development board. |
