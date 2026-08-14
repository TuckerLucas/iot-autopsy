---
title: "Home"
nav_exclude: true
permalink: /
---

# IoT autopsy

This project documents my hands-on security analysis of IoT devices, with the goal of developing and deepening my practical embedded security skills by understanding how these devices work from a security perspective.

Each device assessment shall have its own self-contained directory, containing all relevant documentation, supporting evidence, and findings.

## Assessed devices

| Device Image | Device | Description | Total Findings |
|:------:|:-----------:|:--------------:|:------------:|
| <img src="./tp-link-archer-c7-v2/img/target.png" width="200">| [TP-Link Archer C7](./tp-link-archer-c7-v2/tp-link-archer-c7-v2.md) | Wireless Dual Band Gigabit Router | 39  |
| <img src="./tp-link-tapo-c210-v2/img/target.jpg" width="200">| [TP-Link Tapo C210](./tp-link-tapo-c210-v2/tp-link-tapo-c210-v2.md) | Home Security Wi-Fi Camera | In progress  |

## Assessment structure

Every assessment performed on a device is documented and organised into the following parts:

|      # | Part name   | Content description |
|:------:|:-----------:|---------------------|
| 1      | **Executive summary** | High level overview of the conducted assessment. Summary table with identified findings. |
| 2      | **Scope** | Target device details, features, and tested functionalities/interfaces. |
| 3      | **Technical assessment** | Full technical documentation of all performed tests. Includes OSINT, hardware inspection, debug/programming interface discovery, firmware reverse engineering, system hardening analysis, and external interface exploitation. |
| 4      | **Findings** | Individual finding files detailing each identified vulnerability or observation, including severity rating, CVSS score, description, and remediation guidance. |
| 5      | **Appendix** | Supporting artifacts referenced throughout the assessment, including firmware binaries, capture files, scripts, and raw logs. |

**Note:** The technical assessment methodology serves as a guide rather than a rigid checklist. Since each device is different, assessments vary accordingly. Some phases may not be applicable, and device-specific testing may introduce additional phases.

## Disclaimer

**All information in this project is strictly for educational purposes.** All conducted tests and attacks are performed on devices personally owned by the author. 
