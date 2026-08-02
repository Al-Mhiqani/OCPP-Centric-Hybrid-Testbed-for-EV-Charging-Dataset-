# Dataset README: OCPP-Centric EVCI Security Dataset

## Overview

This dataset provides realistic, semantically rich Electric Vehicle Charging Infrastructure (EVCI) network traffic captured under both benign and adversarial conditions. Generated using a hybrid testbed combining physical hardware and virtual simulation, it is designed for developing and benchmarking protocol-centric Intrusion Detection and Prevention Systems (IDPS) tailored to the Open Charge Point Protocol (OCPP 1.6 and 2.0).

---

## Key Features

* **Features:** 55+ features extracted across multiple layers.
* **Feature Scope:**
* **Semantic Message Fields:** High-level OCPP payload information.
* **Finite-State Machine (FSM) Transitions:** Operational state changes of chargers and sessions.
* **Timing Metrics:** Inter-packet arrival times and message sequence latencies.
* **Payload Complexity:** Encoded payload structures and byte distributions.
* **Network-Level Characteristics:** Transport and IP layer metadata.


* **Protocol Coverage:** Standardized based on official **OCPP 1.6** and **OCPP 2.0** specifications.
* **Realism:** Includes stealthy, context-driven anomalies alongside standard attacks.

---

## Testbed Architecture

Data was collected using a  hybrid testbed integrating:

* Real OCPP-compliant chargers (EVSE)
* Physical EVSE testing hardware
* Simulated Electric Vehicles (EVs)
* Central System / Charging Station Management System (CSMS) controllers

---

##  Attack Scenarios Included

The dataset models both baseline operational traffic (benign) and adversarial scenarios, including:

1. **Authentication Spoofing:** Unauthorized identity emulation and session hijacking.
2. **Man-in-the-Middle (MiTM) Interception:** Eavesdropping and relay attacks on unsecured protocol streams.
3. **Protocol Manipulation:** Unauthorized message modification, replay attacks, and state-violating sequence injections.
4. **Stealth Anomalies:** Sophisticated, low-rate contextual exploits designed to bypass traditional threshold-based detection.

---

## Citation & Publication

If you use this dataset in your research, please cite the corresponding paper:

```bibtex
@article{ocpp_evci_dataset_2026,
  title     = {A Novel OCPP-Centric Hybrid Testbed and Dataset for EV Charging Infrastructure Security Threats Feasibility Testing},
  journal   = {IEEE Xplore},
  doi       = {10.1109/11335665},
  url       = {https://ieeexplore.ieee.org/document/11335665}
}

```
