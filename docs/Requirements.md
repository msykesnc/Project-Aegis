# Project Aegis — System Requirements

**Status:** Draft  
**Date:** July 19, 2026  
**Author:** Miller Sykes

## 1. Purpose

This document defines the initial system requirements for Project Aegis. These requirements will guide hardware selection, software architecture, testing, and future development.

## 2. System Overview

Project Aegis shall be a modular embedded systems platform for learning and demonstrating professional embedded engineering through aerospace-inspired applications.

## 3. Functional Requirements

**FR-001:** The system shall read data from multiple digital and analog sensors.

**FR-002:** The system shall process sensor data in real time.

**FR-003:** The system shall communicate with a host computer for configuration, debugging, and telemetry.

**FR-004:** The system shall support structured data logging.

**FR-005:** The system shall provide visible system-status and fault indications.

**FR-006:** The system shall support modular hardware expansion.

**FR-007:** The system shall support deterministic periodic tasks and control loops.

**FR-008:** The system shall detect and report defined hardware and software faults.

## 4. Non-Functional Requirements

**NFR-001:** Firmware shall use a modular architecture.

**NFR-002:** Hardware-dependent code shall be separated from application logic where practical.

**NFR-003:** Major engineering decisions shall be documented.

**NFR-004:** Source code and documentation shall be maintained in version control.

**NFR-005:** Requirements shall be verifiable through inspection, testing, or demonstration.

**NFR-006:** The system shall be designed for maintainability and future expansion.

**NFR-007:** The repository shall be understandable by another engineering student or embedded engineer.

## 5. Constraints

**CON-001:** The project shall remain budget-conscious.

**CON-002:** Early development shall use commercially available development boards and modules.

**CON-003:** The project shall be developed primarily by one engineer.

**CON-004:** The system is educational and shall not be represented as certified or safety-critical avionics.

**CON-005:** New features shall not be added at the expense of engineering understanding or documentation.

## 6. Planned Future Capabilities

The architecture should allow future support for:

- An RTOS
- CAN communication
- Multiple microcontrollers
- Wireless telemetry
- Custom PCBs
- Additional sensor modules
- Closed-loop control systems
- More advanced diagnostics and fault handling

## 7. Revision History

| Version | Date | Description |
|---|---|---|
| 0.1 | July 19, 2026 | Initial system requirements draft |
