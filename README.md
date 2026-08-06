---
title: "Home"
nav_exclude: true
permalink: /
---

# IoT autopsy

This project documents my hands-on experience pentesting IoT devices. The  goal is to develop and deepen my practical embedded security skills by understanding how these embedded devices work from a security perspective.

## Pentested devices

Each assessed device shall have its own self-contained directory, which contains all relevant documentation, supporting evidence, and findings. The table below details the assessed devices in this project.

| Device | Description | Total Findings | Device Image |
|:------:|:-----------:|:--------------:|:------------:|
| [TP-Link Archer C7](./tp-link-archer-c7-v2/tp-link-archer-c7-v2.md) | Wireless Dual Band Gigabit Router | 39 | <img src="./tp-link-archer-c7-v2/img/target.png" width="200"> |
| [TP-Link Tapo C210](./tp-link-tapo-c210-v2/tp-link-tapo-c210-v2.md) | Home Security Wi-Fi Camera | In progress | <img src="./tp-link-tapo-c210-v2/img/target.jpg" width="200"> |

## Penetration test report structure

Every penetration test performed on a device is documented and organised into the following parts:

|      # | Part name   | Content description |
|:------:|:-----------:|---------------------|
| 1      | **Executive summary** | High level overview of the conducted assessment. Summary table with identified findings. |
| 2      | **Scope** | Target device details, features, and tested functionalities/interfaces. |
| 3      | **Technical assessment** | Full technical documentation of all performed tests. Includes used commands, obtained logs, and observations. The guideline methodology followed in this part is detailed in the next section.|
| 4      | **Findings** | Individual finding files detailing each identified vulnerability or observation, including severity rating, CVSS score, description, and remediation guidance. |
| 5      | **Appendix** | Supporting artifacts referenced throughout the assessment, including firmware binaries, capture files, scripts, and raw logs. |

## Technical assessment methodology

Each technical assessment aims to follow a consistent methodology based on embedded penetration testing practices. The main phases applied to each device are:

1. **Open-Source Intelligence (OSINT)**

      - Collect and analyse vendor documentation
      - Gather third-party knowledge regarding publicly disclosed vulnerabilities

2. **Hardware inspection**

      - Inspect the device's PCB
      - Identify major hardware components and their vulnerabilities

3. **Debug interface discovery**

      - Locate and validate debug interfaces (such as JTAG and UART)
      - Assess debug interface activity

4. **Firmware extraction and analysis**

      - Extract firmware from relevant components
      - Analyse filesystem layouts and reverse engineer binaries and other configurations

5. **System hardening assessment**

      - Obtain internal access to the device via shell
      - Perform dynamic analysis of the running system

6. **External interface analysis**

      - Identify all user facing interfaces and protocols
      - Perform directed attacks on each of these

The phases above serve as a guide rather than a rigid checklist. Since each device is different, assessments will vary accordingly. Some phases may not be applicable, and device-specific testing may introduce phases not listed here. Furthermore, failed attempts and dead ends are documented intentionally as they are considered an essential part of the learning process.

## Disclaimer

**All information in this project is strictly for educational purposes.** All conducted tests and attacks are performed on devices personally owned by the author. 
