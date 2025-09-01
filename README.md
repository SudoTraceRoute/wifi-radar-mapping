# 2D WIFI-Signal-Radar-mapping
 📡 A 2D radar-style mapping of surrounding WiFi signals using a custom-built 2.4GHz Modular Parabolic Dish Antenna. 
 This project is a practical test to evaluate and demonstrate the functionality and directional 
 performance of the antenna created previously, all info's are in repository: https://github.com/SudoTraceRoute/2.4GHz-Modular-Parabolic-Dish-Antenna

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Setup & Installation](#setup--installation)
- [Basic Aircrack-ng Commands](#basic-aircrack-ng-commands)
- [Screenshots](#screenshots)
- [Comparison: Directional vs Omnidirectional](#comparison-directional-vs-omnidirectional)
- [Known Limitations](#known-limitations)
- [License](#license)

---

## 📡 Project Overview

The goal of this project is to map WiFi signals surrounding an apartment using a highly directional 2.4GHz parabolic dish antenna. This "radar-style" scan visually presents the strength and distribution of WiFi networks when scanned with:

- A **custom-built parabolic dish antenna** (directional)
- A **standard omnidirectional antenna**

By comparing the resulting maps, this project demonstrates the effectiveness of the parabolic antenna in terms of range, directionality, and signal isolation.

---

## ✨ Features

- 2D radar-style map of WiFi networks in the environment
- Comparison between custom **parabolic** and **omnidirectional** antennas
- Visual legend of signal strengths
- Uses free, open-source tools (e.g., `aircrack-ng`) for scanning
- Screenshots of mapping process and results included

---

## ⚙️ Setup & Installation

### Requirements

- Linux OS (tested on Debian-based distros)
- `aircrack-ng` installed
- Compatible WiFi adapter (tested with: **WiFi Nation WN-H3**)
- Your custom-built parabolic antenna  
  [See build instructions here](https://github.com/SudoTraceRoute/2.4GHz-Modular-Parabolic-Dish-Antenna)

### Installation

- sudo apt update
- sudo apt install aircrack-ng


---

Connect the parabolic antenna to your network adapter, and you're ready to begin scanning.

🧪 Basic Aircrack-ng Commands

These steps allow you to put your wireless adapter into monitor mode for scanning WiFi signals.

1. Identify your wireless interface
iwconfig


Look for something like wlan0.

2. Enable monitor mode
sudo airmon-ng start wlan0


This will likely create a new interface like wlan0mon.

3. Start scanning
sudo airodump-ng wlan0mon


Let it run and capture the visible WiFi signals. You can rotate the antenna between scans to simulate a directional sweep.

📸 During the scan process, take screenshots for later inclusion in your radar map visualization.

---

### 🖼️ Screenshots

Screenshots of the scanning process and the resulting radar maps are included in the screenshots/ folder.


### 🔍 Comparison: Directional vs Omnidirectional

This project includes scans made using both:

 Custom parabolic antenna (directional)

 Default omnidirectional antenna

By comparing the results:

Directional antenna shows stronger signals in its narrow field of view.

Omnidirectional antenna captures more signals but at lower average strength.

---

### ⚠️ Known Limitations

Due to the constraints of free/open-source software used for generating the radar maps:

The signal map and legend do not always correspond 1:1.

Some strong signals may appear in the legend but not on the map.

Some weaker or out-of-range signals may be inconsistently represented.

Mapping accuracy depends heavily on scan duration, rotation angle consistency, and software interpretation.

📌 These limitations are acknowledged and may be addressed in future updates or with better software solutions.

---

### 📝 License

This project is licensed under the MIT License.
See the LICENSE
 file for details.

---

### 👨‍🔧 Author

Made by SudoTraceRoute

---

### Check out the original antenna project here:
🔗 2.4GHz Modular Parabolic Dish Antenna
