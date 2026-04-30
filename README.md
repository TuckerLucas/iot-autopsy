# Embedded Device Pentesting

## Overview

This repository documents my hands-on exploration and penetration testing of embedded devices, primarily consumer networking and IoT hardware.

The goal of this project is to:

- Develop and deepen my embedded pentesting skills
- Build a practical, well-documented learning archive
- Understand real-world hardware
- Practice structured methodology outside of CTF-style environments

## Scope

This project focuses on **real hardware** and is structured as a collection of **individual device assessments**. Each analyzed device has its own top-level directory with a self-contained penetration test, including documentation, notes, and supporting material such as photographs and captured output where applicable.

I aim to follow a methodology similar to professional embedded security assessments. Therefore, each device is approached in much the same manner, guided by the following methodology:

1. **Open-Source Intelligence (OSINT)**
   - Identify device model, hardware revision, FCC ID, and chipset
   - Collect and analyse vendor documentation and relevant datasheets

2. **Hardware Analysis**
   - Open the device and inspect the PCB
   - Identify major components (SoC, RAM, flash, peripherals...)

3. **Interface Discovery**
   - Locate and validate debug and communication interfaces (UART, JTAG, SPI, I2C...)

4. **Boot and Runtime Analysis**
   - Capture and analyze boot logs
   - Observe bootloader behavior and security controls
   - Assess access restrictions and debug protections

5. **Firmware Analysis**
   - Extract firmware where possible
   - Analyze filesystem layout, binaries, configurations, and scripts
   - Identify services, credentials, and update mechanisms

6. **Access and Exploitation**
   - Attempt authenticated or unauthenticated access
   - Identify misconfigurations, weaknesses, or vulnerabilities
   - Explore realistic attack paths where applicable

7. **Documentation**
   - Record findings clearly and reproducibly
   - Document dead ends, limitations, and lessons learned

It is likely that not every device will reach every stage. Failed attempts are documented intentionally and are considered an essential part of the learning process. The emphasis throughout is on trying to **understand how embedded devices actually work**.

## Disclaimer

This project is **not affiliated with or endorsed by any device manufacturer**. All analysis is performed on devices I personally own and is conducted strictly for **educational and research purposes**.
