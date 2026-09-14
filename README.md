<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/baremetal-logo.png"
       alt="BareMetal Logo"
       width="380">
</p>

<h1 align="center">BareMetal</h1>

<p align="center">
  <b>Smart India Hackathon 2026</b>
  &nbsp;·&nbsp;
  Problem Statement <b>SIH26026</b>
  &nbsp;·&nbsp;
  Team ID <b>119910</b>
</p>

<h3 align="center">TRINETRA</h3>

<p align="center">
  <i>Modular Railway Threat Screening System</i>
</p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=Fh-CTrcxgO4&t=3s">
    <img src="https://img.shields.io/badge/▶%20Watch%20Full%20Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white"
         alt="Watch Full Demo on YouTube">
  </a>
  <img src="https://img.shields.io/badge/Status-Prototype-yellow?style=for-the-badge"
       alt="Status: Prototype">
  <img src="https://img.shields.io/badge/Platform-ESP32--C3-blue?style=for-the-badge"
       alt="Platform: ESP32-C3">
</p>

---

## Table of Contents

* [About Trinetra](#about-trinetra)
* [Problem Statement](#problem-statement)
* [Proposed Solution](#proposed-solution)
* [3D Model Showcase](#3d-model-showcase)
* [Prototype Demonstration](#prototype-demonstration)
* [Online Simulation](#online-simulation)
* [Website Demonstration](#website-demonstration)
* [Key Features](#key-features)
* [System Architecture](#system-architecture)
* [Prototype Details](#prototype-details)
* [Tech Stack](#tech-stack)
* [Project Workflow](#project-workflow)
* [Why Trinetra](#why-trinetra)
* [Team](#team)
* [License](#license)

---

## About Trinetra

**Trinetra** is a modular railway security screening concept designed to detect and flag potential **narcotics and explosive threats** across railway environments — including platforms, parcel offices, checkpoints, and unattended baggage areas.

The system is built around a common sensing and processing architecture that can be deployed in multiple physical configurations.

### Core Concept

> **One sensing brain. Three deployment configurations. One unified security workflow.**

Trinetra combines embedded sensing, multi-sensor fusion, threat visualization, and human verification into a modular railway security platform.

---

## Problem Statement

> **Development of Mobile (Quadruped)/Handheld Device/System for Real-Time Detection of Narcotics and Explosives across Indian Railways.**

The challenge is to develop a practical security system capable of assisting railway personnel in identifying potential threats in real time while remaining adaptable to different operational environments.

---

## Proposed Solution

Trinetra addresses this challenge by separating the **threat-sensing system** from its physical form factor.

The same core sensing and processing module can be deployed as:

* **Mobile robotic platform** — patrol-based screening across large station areas
* **Handheld screening device** — portable screening by security personnel
* **Fixed screening node** — continuous monitoring at designated checkpoints

All three configurations share the same underlying sensing and processing architecture.

Sensor inputs are processed through an **ESP32-C3**, combined using sensor-fusion logic, and presented through an interactive dashboard.

Potential threats are then routed for **human-in-the-loop verification**, ensuring that automated screening supports the operator rather than replacing human judgement.

---

## 3D Model Showcase

<p align="center">
  <b>Trinetra — Modular Deployment Concepts</b>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/3dmodel.gif"
       alt="Trinetra 3D Models — Robot, Handheld Device and Fixed Node"
       width="100%">
</p>

<p align="center">
  <i>
    3D visualization of the three proposed Trinetra deployment configurations:
    mobile robotic platform, handheld screening device, and fixed screening node.
  </i>
</p>

---

## Prototype Demonstration

<p align="center">
  <b>System Overview & Prototype Walkthrough</b>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/trigif.gif"
       alt="Trinetra Prototype Demonstration"
       width="100%">
</p>

<p align="center">
  <i>
    A visual walkthrough of the Trinetra concept, prototype hardware,
    sensor fusion, and threat-screening workflow.
  </i>
</p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=Fh-CTrcxgO4&t=3s">
    <img src="https://img.shields.io/badge/▶%20Watch%20Full%20Video%20on%20YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"
         alt="Watch Full Video on YouTube">
  </a>
</p>

---

## Online Simulation

<p align="center">
  <b>Trinetra — Online Hardware & Sensor Simulation</b>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/simulation.gif"
       alt="Trinetra Online Simulation"
       width="100%">
</p>

<p align="center">
  <i>
    Online simulation demonstrating sensor inputs, embedded processing,
    sensor fusion, and threat-screening behaviour.
  </i>
</p>

---

## Website Demonstration

<p align="center">
  <b>Trinetra — Interactive Security Dashboard</b>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/vahnivesh/Trinetra-BareMetal/main/website.gif"
       alt="Trinetra Website Demonstration"
       width="100%">
</p>

<p align="center">
  <i>
    Interactive dashboard showcasing sensor readings, threat classification,
    screening status, and human-in-the-loop verification.
  </i>
</p>

---

## ◆ Key Features

| Feature                            | Description                                                                 |
| ---------------------------------- | --------------------------------------------------------------------------- |
| **Modular Deployment**             | Robot, handheld, and fixed-node configurations from one core sensing module |
| **Multi-Sensor Fusion**            | Combines THz proxy readings with gas-sensor inputs                          |
| **Threat Screening**               | Demonstrates screening logic for potential narcotics and explosives         |
| **Interactive Dashboard**          | Displays sensor readings, threat classification, and screening status       |
| **Human-in-the-Loop Verification** | Operator review before any final decision                                   |
| **ESP32-C3 Prototype**             | Embedded sensing and processing reference architecture                      |
| **Scalable Architecture**          | Same sensing intelligence can support multiple physical deployments         |

---

## System Architecture

```text
                    ┌───────────────────────┐
                    │    Railway Environment│
                    │ Platforms / Checkpoints│
                    │ Parcel / Baggage Areas │
                    └───────────┬───────────┘
                                │
                ┌───────────────┼───────────────┐
                │               │               │
                ▼               ▼               ▼
        ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
        │ Mobile Robot │ │   Handheld   │ │  Fixed Node  │
        │   Platform   │ │    Device    │ │   Screening  │
        └──────┬───────┘ └──────┬───────┘ └──────┬───────┘
               │                │                │
               └────────────────┼────────────────┘
                                ▼
                    ┌───────────────────────┐
                    │      THz Sensing      │
                    │         Proxy         │
                    └───────────┬───────────┘
                                │
                    ┌───────────▼───────────┐
                    │      Gas Sensors      │
                    │   Chemical Signatures │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │       ESP32-C3        │
                    │ Sensor Fusion & Edge  │
                    │      Processing       │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   Threat Assessment   │
                    │   & Classification    │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   Interactive Web     │
                    │      Dashboard        │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │    Human Operator     │
                    │ Verification & Final  │
                    │       Decision        │
                    └───────────────────────┘
```

---

## Prototype Details

The current implementation is a **proof-of-concept prototype** built to demonstrate the proposed Trinetra architecture and workflow end-to-end.

### Embedded System

* **ESP32-C3** — embedded processing and sensor orchestration
* **THz sensing proxy** — simulation of material-screening behaviour
* **Gas sensors** — simulation of chemical signature detection
* **Sensor-fusion logic** — combines multiple sensor inputs
* **Threat assessment** — generates a screening result for operator review

### Software Layer

* Interactive web dashboard
* Real-time sensor visualization
* Threat classification display
* Screening status indicators
* Human verification interface
* Online hardware/sensor simulation

---

## Tech Stack

| Layer               | Technology                           |
| ------------------- | ------------------------------------ |
| **Microcontroller** | ESP32-C3                             |
| **Sensing**         | THz sensing proxy + Gas Sensors      |
| **Processing**      | Embedded Sensor-Fusion Logic         |
| **Interface**       | Interactive Web Dashboard            |
| **Simulation**      | Online Hardware & Sensor Simulation  |
| **3D Design**       | 3D CAD / Model Visualization         |
| **Deployment**      | Mobile Robot / Handheld / Fixed Node |

---

## Project Workflow

```text
             ┌─────────────────┐
             │ Railway Object  │
             │ / Area Screened │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Sensor Inputs   │
             │ THz + Gas       │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │   ESP32-C3      │
             │ Edge Processing │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Sensor Fusion   │
             │ & Threat Score  │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │   Dashboard     │
             │ Visualization   │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Human Operator  │
             │   Verification  │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Final Screening │
             │     Action      │
             └─────────────────┘
```

---

## Why Trinetra?

### Modular

The same sensing architecture can be deployed across different physical platforms.

### Scalable

Additional screening units can be introduced without redesigning the complete detection architecture.

### Operator-Centric

The system provides decision support while keeping the human operator in the loop.

### Adaptable

Different railway environments can use different configurations depending on operational requirements.

### Real-Time

Embedded processing enables rapid interpretation of sensor inputs and immediate dashboard feedback.

---

## Team

<h3 align="center">Team BareMetal</h3>

<p align="center">
  Building practical, modular security technology for smarter railway environments.
</p>

<p align="center">
  <b>Smart India Hackathon 2026</b><br>
  Problem Statement: SIH26026<br>
  Team ID: 119910
</p>

---

## License

This project is submitted as part of **Smart India Hackathon 2026** under **Problem Statement SIH26026**.

---

<p align="center">
  <b>TRINETRA</b>
  <br>
  <i>Observe. Detect. Verify.</i>
</p>
