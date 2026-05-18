# ICS/OT Home Lab

A clean, minimalist, and utilitarian industrial security simulation platform built completely using free and open-source infrastructure.

## Lab Architecture

This repository contains execution data and setup notes tracking a multi-tier industrial control simulation environment. The deployment implements a core logical controller, dual SCADA/HMI interfaces, and an isolated infrastructure simulation to assess operational technology security primitives.

## Technology Stack

* **OpenPLC Engine** — PLC logic simulation running inside Docker.
* **FUXA** — Lightweight web-based SCADA visualization layer running inside Docker.
* **Ignition Maker** — Industry-standard enterprise SCADA engine hosted within a Windows 11 environment.
* **pyModbus Core** — Industrial protocol framework used to validate unauthenticated payload manipulation vectors.
* **Wireshark Engine** — Deep packet inspection and protocol monitoring tool.

## Key Learning Objectives

* Analyze structural design flaws within the legacy Modbus/TCP specification.
* Establish interface boundaries linking enterprise and lightweight HMIs to real-time industrial runtimes.
* Demonstrate supervisory-bypass attacks by injecting unauthenticated commands directly into controller registers.
* Inspect industrial data transmissions to isolate reconnaissance patterns from malicious modification commands.
* Map emulated lab attacks directly to legendary industrial incidents including Stuxnet and the Oldsmar water treatment exploit.

## Technical Documentation

Detailed build steps, network routing considerations, script samples, and protocol analysis profiles are centrally tracked in the [Technical Writeup (NOTES.md)](NOTES.md).

## Infrastructure Specifications

| Node | Operating System / Environment | Core Resources |
| :--- | :--- | :--- |
| **Host System** | EndeavourOS (Arch-based Linux) | Intel i5 \| 16GB RAM \| 1TB SSD |
| **Attacker Node** | Ubuntu (Isolated LAN workstation) | Bare-Metal Integration |
| **Graphics Processing** | Not Required | Headless Optimization |

---
*Built for documenting research and foundational exploration in ICS/OT systems engineering and infrastructure resilience.*
