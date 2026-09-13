<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/baremetal-logo.png" alt="BareMetal logo" width="380">
</p>

<h1 align="center">BareMetal</h1>

<p align="center">
  <b>Smart India Hackathon 2026</b> &nbsp;·&nbsp; Problem Statement <b>SIH26026</b> &nbsp;·&nbsp; Team ID <b>119910</b>
</p>

<h3 align="center">TRINETRA</h3>
<p align="center"><i>Modular Railway Threat Screening System</i></p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=Fh-CTrcxgO4&t=3s">
    <img src="https://img.shields.io/badge/Watch%20Full%20Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch Full Video on YouTube">
  </a>
  <img src="https://img.shields.io/badge/Status-Prototype-yellow?style=for-the-badge" alt="Status: Prototype">
  <img src="https://img.shields.io/badge/Platform-ESP32--C3-blue?style=for-the-badge" alt="Platform: ESP32-C3">
</p>

---

## Table of Contents

- [About Trinetra](#about-trinetra)
- [Problem Statement](#problem-statement)
- [Proposed Solution](#proposed-solution)
- [Prototype Demonstration](#prototype-demonstration)
- [Key Features](#key-features)
- [System Architecture](#system-architecture)
- [Prototype Details](#prototype-details)
- [Tech Stack](#tech-stack)
- [Team](#team)
- [License](#license)

---

## About Trinetra

**Trinetra** is a modular railway security screening concept designed to detect and flag potential **narcotics and explosive threats** across railway environments — platforms, parcel offices, and unattended baggage points.

The system is designed to be deployed in three interchangeable configurations built around the same core sensing module:

| Configuration | Use Case |
|---|---|
| **Mobile robotic platform** | Patrol-based screening across large station areas |
| **Handheld screening device** | On-demand checks by security personnel |
| **Fixed screening node** | Continuous monitoring at checkpoints and entry gates |

The prototype demonstrates **multi-sensor fusion** using an **ESP32-C3** microcontroller, a **THz sensing proxy**, and **gas-sensor inputs**, paired with an interactive dashboard for threat visualization and **human-in-the-loop verification** — ensuring that no automated decision is acted on without operator sign-off.

## Problem Statement

Development of Mobile (Quadruped)/Handheld Device/System for Real-Time Detection of Narcotics and Explosives across Indian Railways.

## Proposed Solution

Trinetra addresses this by decoupling **threat sensing** from **physical form factor**. The same sensor-fusion "brain" can be mounted on a robot, held by hand, or fixed at a checkpoint — letting Railway Protection Force (RPF) teams choose the right configuration for a given location without redesigning the detection logic each time. A central dashboard aggregates readings across all deployed units and routes flagged events to a human operator for final verification before any escalation.

## Prototype Demonstration

<p align="center"><b>System Overview & Prototype Walkthrough</b></p>

<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/trigif.gif" alt="Trinetra — Modular Railway Threat Screening System" width="100%">
</p>

<p align="center"><i>A visual walkthrough of the concept, prototype hardware, sensor fusion, and screening workflow. Full video linked above.</i></p>

> **Note on images not rendering:** if you're viewing this file locally or on a fork/mirror, make sure both `baremetal-logo.png` and `trigif.gif` are actually committed to the `main` branch at the repo root. GitHub's raw CDN also caches aggressively — after replacing an image under the same filename, allow a few minutes (or hard-refresh) before it updates.

---

## Key Features

| Feature | Description |
|---|---|
| **Modular Deployment** | Robot, handheld, and fixed-node configurations from one core sensing module |
| **Multi-Sensor Fusion** | Combines THz proxy readings with gas-sensor chemical signatures |
| **Threat Screening** | Demonstrates classification logic for narcotics and explosives |
| **Interactive Dashboard** | Live sensor readings, threat classification, and screening status |
| **Human-in-the-Loop Verification** | Operator review required before any final decision |
| **ESP32-C3 Prototype** | Embedded sensing and processing reference architecture |

## System Architecture

```
 ┌───────────────┐     ┌───────────────┐
 │  THz Sensing  │     │  Gas Sensors  │
 │     Proxy     │     │  (Chemical)   │
 └───────┬───────┘     └───────┬───────┘
         │                     │
         └─────────┬───────────┘
                    ▼
          ┌───────────────────┐
          │      ESP32-C3      │
          │  Sensor Fusion &   │
          │  Edge Processing   │
          └─────────┬──────────┘
                    ▼
          ┌───────────────────┐
          │  Dashboard (UI)    │
          │  Threat Visualiz., │
          │  Status Display    │
          └─────────┬──────────┘
                    ▼
          ┌───────────────────┐
          │  Human Operator    │
          │  Verification &    │
          │  Final Decision    │
          └───────────────────┘
```

## Prototype Details

The current implementation is a **proof-of-concept prototype** built to demonstrate the proposed Trinetra architecture and workflow end-to-end. It integrates:

- **ESP32-C3** — embedded processing and sensor orchestration
- **THz sensing proxy** — simulates material-screening behavior
- **Gas sensors** — simulate chemical signature detection
- **Sensor-fusion logic** — combines multiple inputs into a single threat score
- **Interactive dashboard** — visualization layer for operators

## Tech Stack

<!-- Fill in with your actual stack -->
- **Hardware:** ESP32-C3, THz sensing proxy module, gas sensor array
- **Firmware:** C / C++ (Arduino / ESP-IDF)
- **Dashboard:** _(e.g. React / Flask / Node.js — update with your actual stack)_
- **Communication:** _(e.g. Wi-Fi / MQTT / BLE — update as applicable)_

## Team

**Team BareMetal** — Smart India Hackathon 2026, Team ID 119910

<!-- Add team member names and roles here -->

## License

<!-- Add your chosen license, e.g. MIT, Apache-2.0 -->
This project is submitted as part of Smart India Hackathon 2026 under Problem Statement SIH26026.
