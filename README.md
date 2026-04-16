# 📚 Smart Library Kiosk

An automated library management system built with **Arduino Uno**, **RFID RC522**, and an **IR sensor**. Students scan their RFID cards to check in/out of the library, and books are issued or returned through the same kiosk — with a live web dashboard and automatic Excel logging.

> Built as a college mini-project · Prototype · Hardware + Software

---

## ✨ Features

- 🪪 **Student check-in / check-out** via RFID card or fob scan
- 📖 **Book issue and return** system with IR sensor confirmation
- ⏱️ **10-second return window** with countdown timer
- 🚫 **Unknown tag detection** — unregistered cards are blocked
- 📊 **Live web dashboard** showing real-time activity feed and stats
- 📋 **Auto Excel logging** — every scan is saved to a `.xlsx` file via Python
- 🔔 Status feedback through Serial monitor

---

## 🛠️ Hardware Used

| Component | Quantity |
|---|---|
| Arduino Uno | 1 |
| RFID RC522 Module | 1 |
| IR Obstacle Sensor | 1 |
| MIFARE Classic 1K Cards | As needed |
| MIFARE Classic 1K Key Fobs | As needed |
| Jumper Wires | As needed |

---

## 💻 Software & Libraries

| Tool / Library | Purpose |
|---|---|
| Arduino IDE | Uploading firmware to Arduino |
| Python 3 | Serial reading + Excel logging |
| `MFRC522` | Arduino RFID library |
| `pyserial` | Python serial communication |
| `openpyxl` | Excel file writing |
| Chrome / Edge | Web dashboard (Web Serial API) |

---

## 📤 Serial Output Format

The Arduino sends structured data over Serial at **9600 baud**, parsed by both the Python logger and the web dashboard:

```
TYPE:CHECKIN
Name    : Rahul Sharma
Roll no : 21BCS045
Status  : Checked In

TYPE:BOOKISSUE
Name    : Priya Mehta
Roll no : 21BCS032
Book    : Data Structures
BookID  : B-104
Status  : Book Issued
```

---


## 👥 Team

| Name |
|---|
| Ved Joshi |
| Swanandi Bhange |
| Ashutosh Bapat |
| Parth Birari |
| Maitreyee Dabhadkar |
| Ishan Waichal |
| Shreeya Jagtap |

**Department of Computer Science & Engineering**
Marathwada Mitra Mandal's College of Engineering · 2025–26

---

## ⚖️ Intellectual Property & Research Notice

**⚠️ RESEARCH IN PROGRESS:** This project, including its hardware architecture, logic flow, and integrated methodology, is part of an ongoing academic research study. 

**All rights reserved.** No part of this repository may be reproduced, distributed, or used for commercial or academic publications without explicit prior permission from the authors. This public documentation serves as a timestamped record of original work for peer-review purposes.

---

## 🏷️ Topics

`arduino` `rfid` `library-management` `iot` `python` `embedded-systems` `attendance-system` `arduino-uno` `mfrc522` `web-serial-api`

---

<p align="center">Made with ❤️ by Team Smart Library · MMCOE</p>
