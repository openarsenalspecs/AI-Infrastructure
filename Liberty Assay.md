# Liberty Assay

**From Composition to Compensation — Verified.**

Liberty Assay is an open-source, modular precious-metal assay and payout system that analyzes jewelry, determines metal composition, separates recoverable materials, and pays users based on real-time market value — all through a transparent, auditable process.

This system is designed as **open infrastructure**, not a proprietary kiosk. Every subsystem is modular, inspectable, and replaceable.

---

## Core Features

### 🔬 Automated Assay System
- Non-destructive XRF spectroscopy for metal composition analysis
- Karat estimation with alloy detection (gold, silver, platinum, mixed metals)
- Calibration system for industrial-grade measurement accuracy

### 🤖 AI Vision & Material Classification
- On-device AI models for gemstone detection (diamond, sapphire, CZ, glass)
- Jewelry structure recognition (prong, bezel, channel, glue-set)
- Fraud detection (plating, tungsten cores, hollow pieces)
- Fully offline inference (no cloud dependency)

### 🛠 Robotics Disassembly Module
- CNC-style precision motion system (X/Y/Z gantry)
- Automated tool changer for micro-cutting and extraction
- Vacuum pickup system for gemstone recovery
- Path planning generated from AI vision output

### 🔥 Melt & Refining System
- Induction furnace with closed-loop temperature control
- Inert gas support for oxidation reduction
- Automated crucible handling and pour system
- Post-melt bead formation for verification assay

### 💰 Real-Time Pricing Engine
- Multi-source commodity price aggregation
- Median-based price validation system
- Purity-adjusted payout calculation
- Timestamped valuation snapshots for auditability

### 💳 Payment & Settlement Layer
- Instant payout via ACH, debit rails, or stablecoin (optional)
- Fully logged transaction history
- Exportable digital receipt with assay breakdown
- KYC/AML compliance hooks (configurable by deployment)

### 📊 Audit Ledger System
- Append-only event-based transaction log
- Full process replay capability per transaction
- Exportable audit bundles for compliance and transparency
- Local-first data integrity model

### 🧩 Modular Architecture
- Independent system modules (replaceable and swappable)
- Event-driven communication via MQTT/NATS
- ROS2-based robotics orchestration
- Rust-based safety-critical core logic

---

## Tech Stack

### Hardware Layer
- Industrial edge PC (x86 fanless recommended)
- NVIDIA Jetson Orin Nano (AI inference + vision)
- STM32 / ESP32 microcontrollers (real-time control)
- CNC gantry system (open-frame robotics)
- Induction furnace with PID control loop
- XRF spectroscopy module (OEM or integrated unit)
- Precision multi-stage weighing system

### Software Layer
- Rust (core orchestrator + safety systems)
- Python (AI, vision, orchestration services)
- ROS2 (robotics control system)
- PyTorch → ONNX → TensorRT (AI inference pipeline)
- MQTT or NATS (inter-module communication)
- Flutter (kiosk UI)
- React (web admin dashboard fallback)
- SQLite / append-only event store (audit ledger)

---

## System Architecture
```text
User Intake UI
↓
Workflow Orchestrator (Rust)
↓
────────────────────────────
| Vision Module |
| Spectroscopy Module |
| Robotics Module |
| Melt Module |
| Pricing Module |
| Payment Module |
────────────────────────────
↓
Audit Ledger + Export Layer
```

Each module operates independently and communicates through a structured event bus.

---

## How to Build

### 1. Clone the Repository
Download the full system and initialize submodules:

- UI layer
- orchestrator-core
- vision-module
- robotics-module
- melt-module
- pricing-engine
- audit-ledger

---

### 2. Set Up Hardware Stack

Minimum prototype configuration:
- Jetson Orin Nano (AI + vision)
- Industrial PC (system orchestrator)
- CNC gantry frame (modified 3-axis)
- Induction furnace (closed-loop controlled)
- XRF scanner module
- Load cell weight system

---

### 3. Install Core Software Dependencies

- Install ROS2 for robotics coordination
- Install Rust toolchain for orchestrator core
- Install Python 3.11+ for AI modules
- Install PyTorch + ONNX runtime + TensorRT
- Configure MQTT/NATS message broker

---

### 4. Deploy Modules

Each module runs independently:

- Vision module → processes intake scans
- Spectroscopy module → reads composition data
- Robotics module → executes extraction paths
- Melt module → handles refining workflow
- Pricing module → calculates real-time value
- Payment module → executes payout

---

### 5. Configure Event Bus

All modules communicate through structured events:

- `intake.created`
- `scan.completed`
- `composition.analyzed`
- `stones.removed`
- `melt.completed`
- `valuation.generated`
- `payment.executed`

---

### 6. Run Workflow Orchestrator

The orchestrator enforces:

- State transitions
- Safety interlocks
- Module sequencing
- Audit log generation

No melting or payout can occur without full validation chain completion.

---

### 7. Launch Kiosk UI

- Flutter app for touchscreen deployment
- Real-time assay visualization
- Transparent payout breakdown display
- Receipt generation and export

---

## Security & Safety Requirements

- Independent hardware safety cutoff system
- Thermal runaway protection for furnace module
- Tamper detection enclosure sensors
- Encrypted transaction logging
- Fail-safe motion stopping system (hardware-level override)

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/libertyassay/](https://roxanneardary.com/libertyassay/)  

---

## License & Notice Requirements

Liberty Assay is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Project Philosophy

Liberty Assay is built on one principle:

> Physical value should be measurable, transparent, and independently verifiable.

No hidden pricing models.  
No proprietary assay logic.  
No black-box valuation systems.

Just composition → verification → compensation.

---
