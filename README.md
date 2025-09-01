# WIFI-Radar-mapping
 📡 A 2D radar-style mapping of surrounding WiFi signals using a custom-built 2.4GHz Modular Parabolic Dish Antenna. 
 This project is a practical test to evaluate and demonstrate the functionality and directional 
 performance of the antenna created in a previous repository: https://github.com/SudoTraceRoute/2.4GHz-Modular-Parabolic-Dish-Antenna

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

```bash
sudo apt update
sudo apt install aircrack-ng
