# Atrin GPON Network Configuration - Huawei MA5608T

Welcome to the Atrin Project configuration repository! This project documents the setup of a Huawei MA5608T OLT for a residential GPON network serving 340 units with FTTH internet and dual SIP telephony lines.

## Overview
This repository contains the configuration for a Huawei MA5608T Optical Line Terminal (OLT) deployed in the Atrin Project, Mashhad, Iran. Each of the 340 units is equipped with a Huawei HG8245H ONT, providing high-speed internet and two VoIP lines. The network uses 1:16 splitters and connects to the ISP via a port-based uplink.

- **Device:** Huawei MA5608T
- **Units:** 340
- **Services:** FTTH (Internet), SIP (2 VoIP lines per unit)
- **ONT Model:** Huawei HG8245H
- **Splitter Ratio:** 1:16
- **Uplink:** Port-based to ISP
- **Deployment Date:** January 2020

## Files
- **`atrin_config_5608T.txt`**: Main configuration file for the Atrin Project
  - VLANs: 1000 (FTTH), 2000 (SIP)
  - Traffic Profiles: 1Gbps for FTTH, 6Mbps for SIP
  - DBA Profiles: Dynamic 1Gbps (FTTH), Fixed 4Mbps (SIP)
  - ONT Setup: Supports 340 HG8245H units with 2 POTS + 1 ETH

## Features
- **Scalable FTTH:** 1Gbps internet shared across 340 units.
- **Dual VoIP Lines:** 4Mbps fixed bandwidth per unit for reliable telephony.
- **Efficient Design:** Utilizes 1:16 splitters across 16 GPON ports.
- **ISP Integration:** Seamless port-based uplink connectivity.

## Usage
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/sepakosystem/GPON.git
2. Apply Configuration:

 . Copy atrin_config_5608T.txt to your OLT via a terminal (e.g., PuTTY).
 . Paste and execute the commands.
3. Verify:

 . Run display current-configuration on the OLT to confirm settings.
   Prerequisites
 . Huawei MA5608T OLT
 . Huawei HG8245H ONTs (340 units)
 . 1:16 GPON splitters (approx. 16 units)
 . Terminal access (SSH/Telnet)

 Contributing
Feel free to fork this repository and submit pull requests with enhancements. Suggestions for optimizing bandwidth, VLANs, or ONT profiles are appreciated!

Contact
GitHub: sepakosystem
