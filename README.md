# AuctionApp  
[![Made with Kotlin](https://img.shields.io/badge/Made%20with-Kotlin-blueviolet?logo=kotlin)](https://kotlinlang.org/)  
[![Android Studio](https://img.shields.io/badge/Built%20with-Android%20Studio-brightgreen?logo=androidstudio)](https://developer.android.com/studio)  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  

An Android app for managing auction items, bids, and results — built with **Kotlin**, **ZXing QR-code scanning**, and a **cloud-based database**.

---

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Architecture & Tech Stack](#architecture--tech-stack)
4. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
   - [Running](#running)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

---

## Overview
**AuctionApp** streamlines the auction process for organizers and participants.  
It allows organizers to:
- **Scan QR codes** for auction items using the device camera  
- **Record and track bids** in real time  
- **Upload and sync data** to a cloud-based database (e.g. [MotherDuck](https://motherduck.com/))  
- **View spending summaries** and calculate total funds raised  

This app was built as a practical, resume-ready project demonstrating mobile development, database interaction, and QR integration.

---

## Features
- 📷 **QR Code Scanning** — powered by [ZXing](https://github.com/zxing/zxing)  
- 💸 **Bid Tracking** — each auction item maintains its own bid history  
- ☁️ **Cloud Integration** — syncs to a cloud database (MotherDuck / BuckDB)  
- 📊 **Dashboard Summary** — view total raised and per-user spending  
- 🧩 **Modular Kotlin Codebase** — modern Android architecture patterns (MVVM, Coroutines, etc.)

---

## Architecture & Tech Stack
| Layer | Technology / Tool |
|-------|--------------------|
| **Frontend (UI)** | Android XML layouts, Jetpack Components |
| **Language** | [Kotlin](https://kotlinlang.org/) |
| **QR Integration** | [ZXing Library](https://github.com/zxing/zxing) |
| **Database** | Cloud-based (e.g., [MotherDuck](https://motherduck.com/), [BuckDB](https://buckdb.com/)) |
| **Build System** | Gradle |
| **IDE** | [Android Studio](https://developer.android.com/studio) |

---

## Getting Started

### Prerequisites
- [Android Studio](https://developer.android.com/studio) installed  
- Android device or emulator  
- Configured cloud database (MotherDuck, BuckDB, etc.)  
- Camera permission enabled for QR scanning  

### Installation
```bash
git clone https://github.com/Reigns-Liu/AuctionApp.git
