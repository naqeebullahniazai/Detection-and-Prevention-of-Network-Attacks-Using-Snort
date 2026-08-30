# Detection and Prevention of Network Attacks Using Snort

## Overview

This project presents a collaborative Snort-based IDS/IPS framework designed for the detection, analysis, prevention, and automated response to network attacks.

The system combines multiple Snort sensing nodes, centralized event correlation, machine-learning-assisted security analysis, OpenCanary deception, distributed response, and a real-time Streamlit security dashboard.

The project was developed as a controlled cybersecurity laboratory prototype in the Department of Network Engineering, Faculty of Computer Science, Kabul Polytechnic University.

## Key Features

- Collaborative intrusion detection using multiple Snort sensors
- Centralized security event correlation
- Machine-learning-assisted attack analysis using Random Forest V3
- OpenCanary deception and honeypot integration
- Real-time security monitoring dashboard
- Automated distributed attack blocking
- Adaptive block duration and automatic unblocking
- Support for multiple concurrent attackers
- Internal and external attack testing
- Centralized incident visibility

## Machine Learning Model

The project uses a Random Forest V3 model for behavior-based classification.

The model classifies network behavior into:

- NORMAL
- ATTACK

The operational response layer uses three security decisions:

- ALLOW
- MONITOR
- BLOCK

## Model Evaluation

| Metric | Result |
|---|---:|
| Accuracy | 95.47% |
| Precision | 100.00% |
| Recall | 93.25% |
| F1-Score | 96.51% |
| False Positives | 0 |
| False Negatives | 11 |

The final dataset contains 243 cleaned behavioral records:

- 163 ATTACK records
- 80 NORMAL records

## Tested Attack Scenarios

The system was evaluated against several controlled attack scenarios:

- Port Scanning
- SSH Brute Force
- Telnet Brute Force
- ICMP Flooding
- HTTP/Web Attack Behavior
- Concurrent Multi-Attacker Scenarios

## Technologies Used

- Snort IDS/IPS
- Python
- Linux / Ubuntu
- Kali Linux
- Random Forest
- Scikit-learn
- Streamlit
- OpenCanary
- Wireshark
- EVE-NG
- VMware Workstation
- Networking and TCP/IP technologies

## System Architecture

The project combines three distributed Snort sensing nodes with a centralized security management and analysis system.

The central node performs:

Detection → Correlation → Security Analysis → Decision → Distributed Response → Recovery → Monitoring

Architecture diagrams and screenshots will be available in the `docs` and `screenshots` directories.

## Research Paper

A complete research paper describing the architecture, methodology, experimental evaluation, results, limitations, and future work is included in this repository.

## Authors

**Naqeebullah Niazai**  
**ZafarKhan Armani**

Department of Network Engineering  
Faculty of Computer Science  
Kabul Polytechnic University  
Kabul, Afghanistan

**Academic Supervisor:** Abdul Shakoor Azimi

## Research Scope

This project was developed and evaluated in a controlled laboratory environment for academic and cybersecurity research purposes.

It is intended to demonstrate collaborative intrusion detection, intelligent security analysis, deception, automated response, and centralized monitoring.

## Disclaimer

All attack scenarios were conducted only inside an authorized laboratory environment.

This repository is intended for educational, defensive cybersecurity, and research purposes.
