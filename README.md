# 🛡️ Adaptive Runtime Hardware Threat Detection Engine (ARHTDE)
### A Standalone ASIC Security IP for Industrial IoT Systems using Verilog HDL, Cadence Genus & Cadence Innovus

<p align="center">

![ASIC](https://img.shields.io/badge/ASIC-Design-blue)
![Verilog](https://img.shields.io/badge/Verilog-HDL-orange)
![Cadence](https://img.shields.io/badge/Cadence-Genus%20%7C%20Innovus-red)
![RTL](https://img.shields.io/badge/RTL-Synthesizable-success)
![Technology](https://img.shields.io/badge/Technology-180nm-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

</p>

---

# 📌 Project Overview

Adaptive Runtime Hardware Threat Detection Engine (ARHTDE) is a **standalone hardware security ASIC Intellectual Property (IP)** designed to protect Industrial Internet of Things (IIoT) systems against runtime hardware attacks.

Unlike traditional software-based monitoring techniques, ARHTDE performs **real-time hardware monitoring** by continuously observing processor activities such as instruction execution, memory transactions, and control-flow behavior. It computes a cumulative runtime threat score, logs detected attacks, and automatically transitions the system into a secure operating mode whenever malicious activity exceeds a programmable threshold.

The complete project has been implemented using an industry-standard ASIC flow:

- **RTL Design:** Verilog HDL
- **Functional Verification:** Testbenches
- **Logic Synthesis:** Cadence Genus
- **Physical Design:** Cadence Innovus
- **Technology Node:** 180 nm CMOS

---

# 📖 Table of Contents

- Project Motivation
- Problem Statement
- Objectives
- Novelty
- Key Features
- System Architecture
- ASIC Design Flow
- RTL Modules
- Repository Structure
- Physical Design Flow
- Results
- Future Scope
- Author

---

# 🚀 Motivation

Industrial IoT devices are increasingly deployed in mission-critical applications such as:

- Smart Manufacturing
- Automotive Electronics
- Medical Devices
- Defense Systems
- Aerospace
- Smart Grid Infrastructure

These systems continuously exchange sensitive information and are vulnerable to runtime attacks including:

- Illegal instruction execution
- Unauthorized memory access
- Malicious control-flow modification
- Hardware Trojan activation
- Runtime privilege escalation

Software-only security introduces latency and consumes processor resources. Therefore, there is an increasing demand for **dedicated hardware security engines** capable of monitoring system behavior independently of software execution.

ARHTDE addresses this challenge by implementing a reusable hardware security IP that can be integrated into future System-on-Chip (SoC) platforms.

---

# ❗ Problem Statement

Modern Industrial IoT systems rely heavily on software-based security mechanisms that are susceptible to latency, processor overhead, and evolving attack strategies. Existing hardware security implementations often focus on detecting only a single class of attacks, making them insufficient for comprehensive runtime protection.

This project proposes the design of a **Standalone Adaptive Runtime Hardware Threat Detection Engine (ARHTDE)** capable of monitoring processor activities in real time, detecting multiple classes of security violations, computing an adaptive threat score, logging attack information, and generating secure operating modes through dedicated hardware logic.

The complete RTL is synthesized and physically implemented using **Cadence Genus** and **Cadence Innovus**, demonstrating a full RTL-to-layout ASIC design flow.

---

# 🎯 Objectives

- Design a synthesizable hardware security IP using Verilog HDL.
- Monitor processor instruction execution.
- Detect abnormal memory transactions.
- Detect illegal control-flow behavior.
- Compute cumulative runtime threat scores.
- Log detected security events.
- Automatically activate secure operating mode.
- Generate interrupt requests for critical attacks.
- Complete RTL-to-GDSII ASIC implementation using Cadence tools.

---

# 💡 Novelty of the Project

Unlike conventional academic projects that focus on individual security mechanisms, ARHTDE integrates multiple runtime security functions into a **single reusable ASIC IP**.

### Key Novel Contributions

✅ Standalone Hardware Security IP

✅ Adaptive Runtime Threat Scoring

✅ Multi-Level Hardware Attack Detection

✅ Hardware-Based Memory Firewall

✅ Control Flow Integrity Monitoring

✅ Runtime Attack Logging

✅ Programmable Security Registers

✅ Automatic Secure Mode Controller

✅ Interrupt-Based Threat Notification

✅ Complete ASIC Physical Design using Cadence Genus & Innovus

---

# ⭐ Why This Project is Unique

Most student VLSI projects focus on:

- ALU Design
- Multipliers
- SRAM
- FIR Filters
- UART
- Low Power Techniques

ARHTDE goes beyond conventional digital circuits by implementing a **complete hardware security subsystem** capable of protecting embedded processors during runtime.

The project demonstrates expertise in:

- RTL Design
- Hardware Security
- ASIC Design Flow
- Logic Synthesis
- Physical Design
- Timing Analysis
- Power Planning
- Routing
- Design Optimization

making it suitable for semiconductor roles in ASIC Design, RTL Design, Physical Design, and Hardware Security.

---

# 🏗️ System Architecture

<p align="center">

<img src="docs/images/architecture.png" width="900">

</p>

```

It should look like:

```text
Processor Interface
        │
        ▼
Instruction Monitor
        │
        ▼
Memory Firewall
        │
        ▼
Control Flow Checker
        │
        ▼
Threat Score Engine
        │
        ▼
Attack Logger
        │
        ▼
Security Registers
        │
        ▼
Secure Mode Controller
        │
        ▼
Interrupt Controller
```

---
---



---

# 🧩 RTL Module Description

| Module | Description |
|----------|-------------|
| **instruction_monitor.v** | Detects illegal instruction execution and suspicious instruction patterns. |
| **memory_firewall.v** | Monitors memory transactions and detects unauthorized accesses. |
| **control_flow_checker.v** | Verifies branch and jump behavior to prevent control-flow attacks. |
| **threat_score_engine.v** | Computes a cumulative runtime threat score based on detected events. |
| **attack_logger.v** | Stores attack information for debugging and post-analysis. |
| **security_registers.v** | Contains programmable configuration registers and security thresholds. |
| **secure_mode_controller.v** | Activates secure operating mode when threat thresholds are exceeded. |
| **interrupt_controller.v** | Generates interrupt requests during critical security events. |
| **arhtde_top.v** | Top-level module integrating all security blocks. |

---

# ⚙️ ASIC Design Flow

The project follows a complete RTL-to-GDSII implementation flow using industry-standard EDA tools.

```text
Specification
      │
      ▼
RTL Design (Verilog HDL)
      │
      ▼
Functional Verification
      │
      ▼
Logic Synthesis (Cadence Genus)
      │
      ▼
Gate-Level Netlist
      │
      ▼
Floorplanning
      │
      ▼
Power Planning
      │
      ▼
Standard Cell Placement
      │
      ▼
Clock Tree Synthesis (CTS)
      │
      ▼
Routing
      │
      ▼
Post-Route Optimization
      │
      ▼
Timing Verification
      │
      ▼
GDSII Generation
```

---

# 🛠️ Tools & Technologies

| Category | Tool |
|------------|------|
| HDL | Verilog HDL |
| Verification | Testbench |
| Logic Synthesis | Cadence Genus |
| Physical Design | Cadence Innovus |
| Timing Constraints | SDC |
| Automation | TCL Scripts |
| Technology Node | 90 nm CMOS |

---

# 📸 Project Gallery

## System Architecture



<p align="center">
<img src="docs/images/architecture.png" width="900">
</p>

---

## RTL Hierarchy

```text
docs/images/rtl_hierarchy.png
```

<p align="center">
<img src="docs/images/rtl_hierarchy.png" width="850">
</p>

---

## Functional Simulation

```text
docs/images/simulation.png
```

<p align="center">
<img src="docs/images/simulation.png" width="900">
</p>

---

## Logic Synthesis (Cadence Genus)

```text
docs/images/genus.png
```

<p align="center">
<img src="docs/images/genus.png" width="900">
</p>

---

## Floorplan

<img width="1917" height="976" alt="SPECIFIED FLOORPLAN" src="https://github.com/user-attachments/assets/23856b21-48c7-4a0b-a4d2-0cdf6385d2ab" />


<p align="center">
<img src="docs/images/floorplan.png" width="900">
</p>

---

## Power Planning

<img width="1917" height="975" alt="POWER_RING_METAL 3 AND 4" src="https://github.com/user-attachments/assets/fedae23e-0158-4164-aa1a-31b33309a981" />


<p align="center">
<img src="docs/images/power_plan.png" width="900">
</p>

---

## Standard Cell Placement

<img width="1917" height="946" alt="Screenshot 2026-06-30 113046" src="https://github.com/user-attachments/assets/892737c0-13ea-46f7-87d7-624776ca2998" />


<p align="center">
<img src="docs/images/placement.png" width="900">
</p>

---

## Clock Tree Synthesis (CTS)

<img width="1067" height="645" alt="clk tree" src="https://github.com/user-attachments/assets/e4f8c800-64dd-46ac-af98-8db22fb476ab" />


<p align="center">
<img src="docs/images/cts.png" width="900">
</p>

---

## Routing

<img width="1901" height="960" alt="ROUTED" src="https://github.com/user-attachments/assets/d87a7683-5f91-4786-8148-feac1c8b3f70" />


<p align="center">
<img src="docs/images/routing.png" width="900">
</p>

---

## Final Layout

```text
docs/images/final_layout.png
```

<p align="center">
<img src="docs/images/final_layout.png" width="900">
</p>

---

# 🏆 Physical Design Highlights

✔ Complete RTL Development

✔ Functional Verification

✔ Logic Synthesis

✔ Timing Constraints

✔ Floorplanning

✔ Power Rings

✔ Power Stripes

✔ Standard Cell Placement

✔ Clock Tree Synthesis

✔ Global & Detailed Routing

✔ Physical Verification

✔ Timing Analysis

✔ Area Optimization

✔ Power Optimization

✔ Industry Standard ASIC Flow

---
---

# 📊 ASIC Implementation Results

The Adaptive Runtime Hardware Threat Detection Engine (ARHTDE) was successfully implemented using an industry-standard RTL-to-GDSII ASIC flow.

The implementation demonstrates a complete digital IC design cycle, including RTL development, functional verification, logic synthesis, floorplanning, power planning, placement, routing, and physical verification.

---

# 📈 Design Metrics

| Parameter | Value |
|------------|-------|
| Design Style | ASIC IP |
| RTL Language | Verilog HDL |
| Technology | 180 nm CMOS |
| Synthesis Tool | Cadence Genus |
| Physical Design Tool | Cadence Innovus |
| Clock Frequency | 100 MHz |
| Clock Period | 10 ns |
| Constraint Format | SDC |
| Automation | TCL Scripts |

> **Note:** Replace the values below with the actual values from your generated reports after synthesis and physical implementation.

| Report | Value |
|---------|------:|
| Standard Cells | XXXX |
| Total Cell Area | XXXX µm² |
| Total Power | XXXX µW |
| Dynamic Power | XXXX µW |
| Leakage Power | XXXX µW |
| Worst Negative Slack (WNS) | XXXX ns |
| Total Negative Slack (TNS) | XXXX ns |
| Maximum Frequency | XXXX MHz |

---

# 📋 Reports Generated

The following reports were generated during the implementation flow.

```text
reports/

area.rpt

power.rpt

timing.rpt

qor.rpt

congestion.rpt

post_route_timing.rpt
```

---

# 📌 Logic Synthesis

The RTL was synthesized using **Cadence Genus**.

### Synthesis Flow

```text
Read RTL

↓

Elaborate Design

↓

Apply SDC Constraints

↓

Generic Synthesis

↓

Technology Mapping

↓

Optimization

↓

Netlist Generation

↓

Area Report

↓

Timing Report

↓

Power Report

↓

QoR Report
```

---

# 📌 Physical Design

The synthesized netlist was imported into **Cadence Innovus**.

The following implementation stages were completed:

✅ Floorplanning

✅ Power Ring Generation

✅ Power Stripe Insertion

✅ Standard Cell Placement

✅ Congestion Analysis

✅ Power Routing (sRoute)

✅ Global Routing

✅ Detailed Routing

✅ Design Verification

---

# 📐 Floorplanning Strategy

The design uses a **square floorplan** with optimized utilization to minimize routing congestion while maintaining timing performance.

| Parameter | Value |
|------------|------:|
| Aspect Ratio | 1.0 |
| Core Utilization | 70% |
| Core Margin | 8 µm |

---

# ⚡ Power Planning Strategy

The power delivery network was constructed using dedicated power rings and power stripes.

Features include:

- VDD / VSS Power Rings
- Horizontal Metal Routing
- Vertical Metal Routing
- Dedicated Power Distribution
- Special Routing (sRoute)

---

# 🏗️ Placement Strategy

The placement stage optimized:

- Cell Density
- Routing Congestion
- Wirelength
- Timing

Placement verification included:

```text
checkPlace

reportCongestion

verifyConnectivity
```

---

# 🔀 Routing Strategy

Routing was completed using NanoRoute.

Verification included:

- Global Routing
- Detailed Routing
- Geometry Verification
- Connectivity Verification

---

# 🛡️ Security Features Implemented

✔ Runtime Instruction Monitoring

✔ Memory Access Protection

✔ Control Flow Integrity Checking

✔ Adaptive Threat Scoring

✔ Attack Event Logging

✔ Secure Mode Activation

✔ Interrupt Generation

✔ Runtime Configuration Registers

---

# 🚀 How to Run the Project

## RTL Simulation

Compile the RTL:

```text
ncvlog *.v
```

Run Simulation:

```text
ncelab tb_arhtde
```

Launch Simulator:

```text
ncsim tb_arhtde
```

---

## Cadence Genus

Run synthesis:

```text
genus -files run.tcl
```

Outputs:

- Netlist
- Area Report
- Timing Report
- Power Report
- QoR Report

---

## Cadence Innovus

Launch Innovus:

```text
innovus
```

Restore Design:

```text
restoreDesign arhtde.enc
```

Implementation Flow:

```text
Floorplan

↓

Power Planning

↓

Placement

↓

Routing

↓

Verification
```

---

# 🎓 Skills Demonstrated

This project demonstrates practical knowledge in:

- RTL Design
- Verilog HDL
- Hardware Security
- ASIC Design Flow
- Logic Synthesis
- Static Timing Analysis
- Floorplanning
- Power Planning
- Standard Cell Placement
- Routing
- Design Rule Verification
- Cadence Genus
- Cadence Innovus
- TCL Automation
- SDC Timing Constraints

---

# 💼 Industry Applications

The proposed hardware security IP can be integrated into:

- Industrial IoT Systems
- Smart Manufacturing Controllers
- Automotive ECUs
- Medical Embedded Devices
- Aerospace Electronics
- Defense Systems
- Secure Embedded SoCs
- FPGA-based Security Platforms

---

---

# 🔬 Future Enhancements

The current implementation provides a modular and synthesizable hardware security IP. Future improvements can further enhance its capabilities for advanced embedded systems.

### Planned Enhancements

- Integration with RISC-V based SoCs
- Secure Boot Verification
- Hardware Trojan Classification
- AI-assisted Threat Prediction
- TrustZone-compatible Secure Partitioning
- Cryptographic Accelerator Integration
- FPGA Prototyping
- Multi-Core Processor Security Support
- Runtime Firmware Authentication
- Hardware Root of Trust

---

# 📖 Research Contribution

The Adaptive Runtime Hardware Threat Detection Engine (ARHTDE) demonstrates an integrated hardware-based approach for runtime security in Industrial IoT systems.

Unlike conventional student projects that focus on arithmetic units, communication protocols, or standalone digital circuits, this work introduces a dedicated security IP capable of:

- Monitoring runtime processor behavior
- Detecting abnormal hardware events
- Protecting memory transactions
- Validating control-flow execution
- Computing adaptive threat scores
- Logging attack information
- Generating secure operating modes

The design follows an industry-standard ASIC implementation methodology using Cadence Genus and Cadence Innovus, making it suitable as a reusable hardware security IP.

---

# 🌍 Real-World Applications

The proposed architecture can be integrated into:

- Industrial Automation Controllers
- Smart Factory Systems
- Automotive Electronic Control Units (ECUs)
- Medical Monitoring Devices
- Aerospace Electronics
- Defense Communication Systems
- Smart Grid Infrastructure
- Secure Embedded Processors
- Industrial Robotics
- Edge AI Hardware Platforms

---

# 🎯 Learning Outcomes

Through this project, the following ASIC design concepts were implemented and explored:

- RTL Design using Verilog HDL
- Hardware Security Architecture
- Modular Digital Design
- Functional Verification
- Constraint Development using SDC
- Logic Synthesis using Cadence Genus
- Timing Optimization
- Floorplanning
- Power Planning
- Standard Cell Placement
- Routing
- Physical Verification
- ASIC Physical Design Flow
- TCL Automation

---

# 📚 References

1. Cadence Genus Synthesis Solution User Guide
2. Cadence Innovus Implementation System User Guide
3. IEEE Transactions on VLSI Systems
4. RISC-V Privileged Architecture Specification
5. Industrial Internet Consortium (IIC) Security Framework
6. NIST Cybersecurity Framework
7. CMOS VLSI Design – Weste & Harris
8. Digital Integrated Circuits – Jan M. Rabaey

---

# 📂 Repository Highlights

- ✔ Synthesizable RTL Modules
- ✔ Complete Testbench
- ✔ Cadence Genus Flow
- ✔ Cadence Innovus Flow
- ✔ SDC Timing Constraints
- ✔ TCL Automation Scripts
- ✔ ASIC Physical Design
- ✔ Timing Reports
- ✔ Power Reports
- ✔ Area Reports
- ✔ Modular Hardware Security IP

---

# 📌 GitHub Topics

```text
asic
vlsi
verilog
rtl
hardware-security
industrial-iot
cadence
genus
innovus
physical-design
digital-design
eda
timing-analysis
hardware-firewall
soc
semiconductor
```

---

# 📄 License

This project is released under the **MIT License**.

Feel free to use the source code for educational and research purposes.

---

# 👩‍💻 Author

**Swathi Thiru**

Electronics and Communication Engineering (ECE)

Specialization:
- VLSI Design
- ASIC Physical Design
- RTL Design
- Hardware Security
- Industrial IoT


### ⭐ "Designing Secure Silicon for the Next Generation of Industrial IoT Systems."

</p>

---

## Repository Statistics

| Category | Details |
|-----------|----------|
| Design Language | Verilog HDL |
| RTL Modules | 9 |
| Testbenches | 1+ |
| Constraint Files | SDC |
| Automation | TCL |
| Synthesis Tool | Cadence Genus |
| Physical Design Tool | Cadence Innovus |
| Technology | 180 nm CMOS |
| Clock Frequency | 100 MHz |
| Design Flow | RTL → GDSII |

---

## Acknowledgements

This project was developed as part of an advanced VLSI ASIC Design and Physical Design learning journey. It demonstrates the complete RTL-to-Physical Design flow using industry-standard Cadence EDA tools and serves as a portfolio project showcasing practical ASIC implementation techniques for hardware security applications.
