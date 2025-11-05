AuctionApp

An Android app to manage auction items, bids and results — built with Kotlin, ZXing QR-code scanning, and a cloud-based database.

Table of Contents

Overview

Features

Architecture & Tech Stack

Getting Started

Prerequisites

Installation

Running

Usage

Project Structure

Contributing

License

Contact

Overview

AuctionApp is designed to streamline the workflow of organizing auctions. It allows an organizer to:

Scan QR codes of auction items via the mobile-device camera

Track bids in real time

Upload data to a cloud‐based database (e.g., MotherDuck)

View individual bidder spend and calculate total funds raised

This project serves as your first mobile app build and is a strong addition for your resume: it demonstrates full-stack thinking, mobile UI, database interaction, and QR-code integration.

Features

QR-code scanning of items using ZXing

Bid tracking: each auction item gets bid entries and updates

Cloud integration: upload bids and item state to a remote database

Organizer dashboard: view summary of spending per bidder & total raised

Clean Kotlin architecture, modular code, and use of modern Android Studio tooling

Architecture & Tech Stack

Platform: Android (minimum SDK version as defined in build.gradle)

Language: Kotlin

QR Code library: ZXing

Database / Backend: Cloud-based (e.g., MotherDuck or BuckDB)

Build system: Gradle (see build.gradle, gradle.properties, etc.)

Dependencies & tools: Android Studio, Kotlin Coroutines/Flow (if used), UI architecture patterns (MVVM, etc.)

Version control: Git & GitHub

Getting Started
Prerequisites

Android Studio installed on your development machine

Android device or emulator

Valid cloud-database setup (you’ll need to configure database credentials or endpoint)

QR Code scanning permissions (camera, etc.)

Installation

Clone the repository:

git clone https://github.com/Reigns-Liu/AuctionApp.git


Open the project in Android Studio.

Review local.properties (e.g., for SDK paths) and ensure the correct Android SDK is installed.

Configure backend/database credentials (you may need to modify a config file or constants in code).

Sync Gradle and ensure all dependencies resolve.

Running

Start the app on an emulator or connected Android device.

Grant camera permissions when prompted (for QR-code scan).

Use the “Scan Item” feature to scan a QR code of an auction item.

Enter bids or view current bids.

Upload data to the cloud and check dashboard summary to view total fund-raising results.

Usage

For Organizers: Use the app to manage the entire auction flow—from item QR-code scanning, to bid entry, to results summary.

For Developers: This codebase can be extended to support livestream bidding, push notifications, user authentication, item image upload, or integration with payment gateways.

Project Structure

Here’s a high-level overview of the main directories and files:

/app
  ├─ src/main/java/com/yourpackage/
      ├─ ui/           ← UI components (Activities/Fragments)  
      ├─ data/         ← Data layer (models, repository, database)  
      ├─ scan/         ← QR-code scanning logic (ZXing integration)  
      ├─ viewmodel/    ← ViewModel classes for MVVM architecture  
  ├─ src/main/res/     ← Resources (layouts, strings, images)  
build.gradle          ← App-level build settings  
gradle.properties     ← Global Gradle properties  
README.md             ← This file  
.gitignore            ← Files & folders ignored by git  

Contributing

Contributions are very welcome. To contribute:

Fork the repository

Create a new branch (git checkout -b feature/YourFeature)

Commit your changes (git commit -m 'Add some feature')

Push to your branch (git push origin feature/YourFeature)

Open a Pull Request on this repository

Please ensure your code adheres to the existing style and includes documentation/comments where appropriate.
