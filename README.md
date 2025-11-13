# BT_DOS_Attack 
**Python Version**

Script for demonstrating Bluetooth Denial-of-Service (DoS) behavior on vulnerable Bluetooth devices for **educational** and **cybersecurity research** purposes.

## Disclaimer
This project is developed for cybersecurity learning and academic research only.  
It demonstrates how Bluetooth devices may behave under high traffic load for the purpose of understanding wireless security weaknesses.

You may only use this script in:
- Controlled lab environments  
- On devices that you personally own  
- Or on devices where you have formal written permission to test

Any unauthorized use, disruption, or damage caused by operating Bluetooth DoS tests is strictly prohibited.  
The developer provides this software **without any warranty** and is **not responsible** for any misuse, damages, or legal consequences arising from its use.

## Installation

\`\`\`bash
$ sudo apt update
$ sudo apt install python3 python3-pip bluez bluez-tools
$ sudo git clone https://github.com/SOWNTHAR04/BT_DOS_ATTACK.git
$ python3 BT_DOS_ATTACK.py

## Note
This script works **only on Linux systems**.  
You must have the following Bluetooth utilities installed:
- l2ping
- hcitool

These are installed by default on **Kali Linux**.

## Tested on
- Kali Linux as attacker, Bluetooth Device as target  
- Raspberry Pi Zero W as attacker, Redmi Buds Lite as target

## Manual

### Target ID or MAC
Enter the ID or MAC address displayed after scanning.

### Packet Size
Size of the packets to be sent to the target.  
**600 bytes** is recommended for strong effectiveness.

### Threads Count
Number of simultaneous threads sending packets.  
Higher values increase the load on the target device.


## What Happens to the Target Device?
Based on real lab observations:
- The device may disconnect  
- The device may freeze temporarily  
- In some cases, the device automatically powers off  
- Bluetooth functionality may become unresponsive for a short period  

Behavior depends on device hardware and Bluetooth chipset.

## MIT License
MIT License

Copyright (c) 2025 

Permission is hereby granted, free of charge, to any person obtaining 
a copy of this software and associated documentation files (the "Software"), 
to deal in the Software without restriction, including without limitation 
the rights to use, copy, modify, merge, publish, distribute, sublicense, 
and/or sell copies of the Software, and to permit persons to whom the Software 
is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included 
in all copies or substantial portions of the Software.


